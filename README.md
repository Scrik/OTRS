
# Contents
1. [ DEPLOYMENT AND USAGE](http://www.google.com)
1. [ CHANGE](http://www.google.com)
1. [ NEW LOOK AND FEEL](http://www.google.com)
1. [ FUTURE OF THE PROJECT](http://www.google.com)

___
# DEPLOYMENT AND USAGE

1. Copy Paste and overwrite all the files.
2. Change the used skin in OTRS admin SysConfig Panel.
3. Now each user can select the theme from his preferences Menu, by clicking on the name (usually top right corner).


*NOTE*: You won’t be able to use any other skin after applying this package. Take a backup of your files if you ever need to revert back to some other skin or need to update your OTRS version in the future.

___

# CHANGES

List of files in which changes were made
*	DTL files
   1. AgentFAQExplorer.dtl
   1. AgentNavigationBar.dtl
   1. CustomerTicketMessage.dtl
   1. Header.dtl
   1. Login.dtl
  
* JavaScript
  1. Core.Agent.js

* CSS
  1. Core.AgentTicketQueue.css
  1. Core.Default.css
  1. Core.Form.css
  1. Core.Header.css
  1. Core.OverviewSmall.css
  1. Core.Table.css
  1. default/Core.Header.css


####DTL FILES
* *AgentFAQExplorer.dtl*

   Fixing of irregular layout caused by the new Vertical Navigation Bar, removed line: 25 Clear Fix

* *AgentNavigationBar.dtl*

    Many changes were done to facilitate hiding the sidebar, introducing the arrow for indicating the collapse and expand functionalities of List Items, and moving the other list items down.

* *CustomerTicketMessage.dtl*
 
     Introduced more form fields.

* *Header.dtl*

    Changed logout icon.


*  *Login.dtl*

    Heavy changes made to the Agent login page.
Login.dtl has some if not many inline CSS styles which obviously is not recommended in usual situation but in this case it works out pretty fairly as no other file/DOM is supposed to adopt this style.
The footer was not removed as removing it for some absurd reason disabled the login button (why this happened is still not clear)
The original header of the page is now the footer.

####JAVASCRIPT
*  *Core.Agent.js*

    Commented out Lines 98-102 to disable the timer of a List Item drop down.

####CSS
*  *Core.Form.css*

    Fixed layout and indentation for forms which was ruined because of the new Login page.

*  *Core.Header.css*

    Modified colour attributes, Logout Button, Removed float, changed the Navigation bar to sidebar, Position Attributes, Position Attributes for Error message, changes to elements of sidebar to accommodate the changes made (Look and feel).

*  *Core.OverviewSmall.css*

    Removed Padding, Fixed Layout.

*  *Core.Table.css*

    Background and mouse hover highlight colour changed.

*  *Core.AgentTicketQueue.css*, *Core.Default.css*

    Minor layout changes as a result of making the side Navigation Bar.

___
# NEW LOOK AND FEEL

<img align="right" src="https://raw.githubusercontent.com/asabeeh18/OTRS/master/Report/Drop%20Down%20and%20dynamic.PNG">

The new Navigation bar is a sidebar which has many dynamic entities added to it.

Once a list Item is clicked it expands if it contains more elements.

It does not collapse until and unless it is manually done by the user 

This is unlike the previous behaviour in which the list collapses after a few seconds.

There is a small arrow head indicating the current state of the list:
   If the arrow head is pointing down is indicates that the list is expanded.
Arrow head pointing towards the right means it is currently collapsed.

On expansion of a list the other items move down to accommodate the sub list items.


___
<img align="right" src="https://raw.githubusercontent.com/asabeeh18/OTRS/master/Report/dynamic%20size.PNG">

The new Navigation Bar has dynamic size changing according to the text content. As can be seen from the previous and this image.

The currently selected page has the corresponding list Item a thin black border around it.


___




A slight pink color is added on a sub list item upon mouse hover 
![alt text](https://raw.githubusercontent.com/asabeeh18/OTRS/master/Report/Screenshot%20(328).png)
The whole Navigation Bar can be collapsed to the side increasing the workspace area.
This can be done by clicking on the double arrow on top of the Navigation Bar.
____



![alt text](https://raw.githubusercontent.com/asabeeh18/OTRS/master/Report/Login.PNG)
The new login page is completely revamped to give it a new feel and remove the excess unnecessary elements

Various other changes to match the new colour theme have been done. Ranging from the hover color on items in a list or in a table to changing the colour of the page header.
