### RuleZ

## August 2020

For numerical input, ```.clearAnswer``` will set the value to '0'.  
This doesn't fully clear the answer, as '0' is still considered a value.  The user must manually delete the '0' for the QID to be considered clear.  
Basically, do not use ```.clearAnswer``` for numerical input.

## December 2019

### Standard RuleZ Writing Format
```
// Last Updated: {enter date}




//*******************************
// {NAME OF SECTION} - Begin
//*******************************

// {comments go here -->} If QID 1631 is answered Option 2, then disappear and clear answer to QID 1641.
ifQ(1631)
.answered(2)
.disappear(Q(1641))
.clearAnswer(Q(1641))

//*******************************
// {NAME OF SECTION} - End
//*******************************
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

 
 ## Documentation
 
 [RuleZ Documentation](https://sassierulez.wordpress.com/)
 
 [RuleZ Cause and Effect](https://www.sassieshop.com/site/z/rulez/index.php)
 
 


