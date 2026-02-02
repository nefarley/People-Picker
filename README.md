# People Picker - A PowerApps Project
This powerapp shows how to create a custom people picker. It shows the user's profile picture, and other information from active directory. This can also be used as an add-in for other applications, streamlining the process of allowing users to look-up others within their organization. Application and code are available for download. You will need to connect to your own/organizations active directory. 

Perform a search by the user's name, show the user's information, populate fields with the selected user's information.
<img width="1314" height="754" alt="image" src="https://github.com/user-attachments/assets/222bf5ed-45a8-4cdb-aab1-09779da462b4" />

# Overview of Implementation
I added a text input field for the search result, and added two buttons. one for activating the search dialog window and another for clearing the search result text input.<br>
<img width="833" height="478" alt="image" src="https://github.com/user-attachments/assets/7fa737e9-f84c-4680-976d-69936418c421" /><br><br>
Next I created the dialog search window. This will be the interactive search area for the user searching for a specific person.<br>
This search view contains a text input field that acts as the search bar, a gallery which contains the list of users when searching for a specific user, and an icon indicator that lets the user searching know if a specific user is available in their system (active directory).<br>
<img width="1305" height="743" alt="image" src="https://github.com/user-attachments/assets/2793f222-8219-4112-9434-8557880a6ec2" /><br><br>
Below is a result of a search for myself.<br>
This displays limited info as some information pulled from active directlry could be part of PII. The data chosen would be general informaiton available to see by any user within a company.
Employee Name<br>
Employee Department<br>
Employee Email<br>
Employee Job Title<br>
Employee Office Location<br>
(as an added bonus) Employee Photo<br>
<img width="1314" height="754" alt="image" src="https://github.com/user-attachments/assets/f939c2e8-08c4-46aa-873c-16d13719ab6f" /><br><br>
When selecting the specified user, a loading dialog window displays. I found this to be a nice feature as there can be times where data loading can lag. If and when that's the case, notifying the user of data loading is an exceptional and nice feature.<br>
<img width="1312" height="755" alt="image" src="https://github.com/user-attachments/assets/9eb49186-fa22-4e2d-be8b-fedc4b41d036" /><br><br>
Once the loading is complete, the data searched for is then loaded into the text field.<br>
<img width="1314" height="752" alt="image" src="https://github.com/user-attachments/assets/4c4efbdb-0f11-4a6f-b1fb-9c2298ad00b7" /><br><br>
As an option to try again, the user can clear the search result by clicking the "Clear Info" button.<br>
<img width="1309" height="742" alt="image" src="https://github.com/user-attachments/assets/8f678141-2807-4256-887c-6fa6c358ebad" /><br><br>
And the data has been cleared.<br>
<img width="1304" height="751" alt="image" src="https://github.com/user-attachments/assets/2513e8d8-f1cd-4a7f-a005-2d118c5244aa" />


