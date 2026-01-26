# People Picker - A PowerApps Project
This powerapp shows how to create a custom people picker. It shows the user's profile picture, and other information from active directory. This can also be used as an add-in for other applications, streamlining the process of allowing users to look-up others within their organization.

Perform a search by the user's name, show the user's information, populate fields with the selected user's information.
<img width="1295" height="731" alt="image" src="https://github.com/user-attachments/assets/a281a347-e67f-4630-b4c1-03ea9ec6d5a6" />

# How to Implement...
add a Text Input or Text Label. Using a text input field would allow for the selected user's information to be submitted via form to a sharepoint list or collection.

<img width="828" height="476" alt="image" src="https://github.com/user-attachments/assets/240ad432-0b00-45bb-bfd9-db49bc4fd286" />

In the Default section, add a variable name. It'll throw an error message until you create/set the variable in later steps
<img width="1393" height="101" alt="image" src="https://github.com/user-attachments/assets/83c6f173-2f8e-4365-9471-4b7fa941572e" />

Updating the Hint Text field with content. I enjoy Star-Trek, so IYKYK...
<img width="1411" height="132" alt="image" src="https://github.com/user-attachments/assets/66cb5d9a-59b1-49fb-8c58-ab961054abe5" />

Add two buttons. One called Search Users and another called Clear Info.<br>
<img width="467" height="124" alt="image" src="https://github.com/user-attachments/assets/209790f6-5c99-4f2c-9bc4-ee25bdb1398a" />
<br>*Colorway can be anything you want.*

A quick overview so far<br>
<img width="833" height="478" alt="image" src="https://github.com/user-attachments/assets/7fa737e9-f84c-4680-976d-69936418c421" /><br>

Next, we're going to create the search<br>
<img width="1305" height="743" alt="image" src="https://github.com/user-attachments/assets/2793f222-8219-4112-9434-8557880a6ec2" /><br>
Before we create the search container, update the OnSelect property on the People Search Button with the following:<br>
<i>UpdateContext({<br>
    teamSearch:"",<br>
    empSearch: true<br>
});</i> <br><br>
 <b><i>*Background:</b> "The UpdateContext function to create a context variable, which temporarily holds a piece of information, such as the number of times the user has selected a button or the result of a data operation." - source: <a href="https://learn.microsoft.com/en-us/power-platform/power-fx/reference/function-updatecontext" target=
"_blank">UpdateContext Property</a></i><br>
<img width="1896" height="373" alt="image" src="https://github.com/user-attachments/assets/a8f07843-eea5-44c2-9743-d4618f22dbb7" /><br>

With the same energy, update the Clear Info OnSelect button with: <br>
<i>UpdateContext({employeeName:""});</i>
<img width="1896" height="339" alt="image" src="https://github.com/user-attachments/assets/c39cfe91-b6ba-4410-8c6c-d37ffd89ec47" /><br>




