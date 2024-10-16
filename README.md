### Announcements  

## September 2024  
If the error message [object Object] appears, fix by clearing the browser's cache.  

## August 2024  
Avoid using slashes ( / ) or apostrophes ( ' ) in file names.  

## January 2024
Added [Closed Location Guidelines](https://github.com/gfcrbg/RuleZ/wiki#closed-location-guidelines) to GitHub wiki.

## February 2023
Using ```.makeNotRequired``` will not affect points.  
Meaning, a 0/1 =! 0/0.  
It only makes a QID not require an answer.  
To circumvent point valuation, a QID must have its condition manually set in form settings.

## November 2022
Tested and discovered that a Presto import will trigger RuleZ.

## October 2022
RuleZ code-block to calculate date duration:  
__NOTE__:  Initially stored as milliseconds.  Must convert from initial format.  
```
ifQ(A)
.answered()
.andifQ(B)
.answered()
.sub(Q(B), Q(A))
.store(Q(C))
.divide(Q(C), 1000)
.store(Q(C))
.divide(Q(C), 24)
.store(Q(C))
.divide(Q(C), 60)
.store(Q(C))
.divide(Q(C), 60)
.store(Q(C));  
```

## April 2022
Recalcs do NOT trigger RuleZ.  
The shops must be updated to trigger RuleZ.  

## March 2022
New standard practice.  Always use logic controllers such as ```.andifQ() .andQ() .orifQ() .orQ()``` when more than one condition is utilized in a block of script.  

## June 2021
New standard practice.  Every code block must end with a semicolon.  This allows the error checker to identify code blocks that erroenously begin with a period.  Such as ```.ifQ()```.

## January 2021

Changed the naming convention of GitHub files to include Survey ID (SID).  
"[SID] -- [Survey Name]"

## September 2020

RuleZ-Hidden, (QIDs that are ```.disappear```), will now, by default, visibily hide from the user in Review view.  To show RuleZ-Hidden QIDs on said view, the follwing button must be toggled:  

![alt text](https://xhnmga.ch.files.1drv.com/y4mSXWkKVy5MWCNJONrnsKwRiX7rgp2YzVZiymzDrrT57Vv6XFwfzjuLrHHxxVynQj033eUH0CvUjmcDeXNbKaEiYUyACmHy1OO6gv6wdZB3B_OBuM-KQOP8z4XvnKUQq8WC4KBd4W4X9sakfftH9XHaILF5hMWiJfo6GZRTkbEbfRP3IcjGuBjDtyUX_UKhNfV_HUKJ-_aFTVqRk61V_valg?width=387&height=77&cropmode=none)  


Created a [RuleZ Wiki](https://github.com/gfcrbg/RuleZ/wiki).


## August 2020

For numerical input, ```.clearAnswer``` will set the value to '0'.  
This doesn't fully clear the answer, as '0' is still considered a value.  The user must manually delete the '0' for the QID to be considered clear.  
If the QID is conditional, use ```.notAnswered```.  

```
// Time Field -- If QID X is not answered Option Y, then disappear and clear answer to QID Z.
ifQ(X)
.notAnswered(Y)
.disappear(Q(Z)
.clearAnswer(Q(Z));
```

## October 2019

Transferred RuleZ from Gist to GitHub (repositories).  
Benfits of transferring to this platform:

- Better navigation
- Better file managment
- Search
- Version control
- Collaboration
- Export repositories

If you have any inquiries, ask IT personnel via email.

 _Greg Steelman
 gsteelman@realitybasedgroup.com_
 
 _IT it@realitybasedgroup.com_
 
If you have an issue or a request, submit an IT ticket via Salesforce.
 
 


