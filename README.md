# Project Tasks and Results
Some screenshots of my projects.

**Section 1: -**

**Task 1** - Recreate <https://www.javascripttutorial.net/sample/dom/countdown-timer/> , a website that does 2023 new year countdown. All the computations must be done only using JavaScript and CSS for page styling.

**Solution 1 -** The webpage was recreated in the local server (<http://127.0.0.1:5500/countdown_timer/index.html>, where countdown_timer is directory and index.html is the file name).

The calculations are done in JavaScript. This involving setting end time to ‘January 01 {current year + 1} 00:00:00’. This can be done using new Date() function and the current year can be obtained using new Date().getFullYear(). The remaining time is obtained by subtracting the current time from the end time. The difference is formatted to the required (days hours minutes seconds) format. If the remaining time is less than 0, counter is cleared and a new timer is started for the next year (current year + 1). If it is greater than 0, the remaining time or counter is displayed and updated every second (that is, remaining time is decremented every minute). If the remaining time is 0, a message - “Happy New Year {Year} “- is displayed. This message is hidden in all other cases.

Styling is down using CSS. Background image can be set to any image using “background-image: url(‘’);” and the font-size and other display features can be set as per requirement.

A screenshot of the final result is attached below:

![image](https://user-images.githubusercontent.com/107001929/188275781-528d2c74-875c-41c8-8169-762398c94cef.png)

                                 Figure 1: New Year Countdown Web page

**Task 2** - Create a web page to display current time as a clock using HTML, CSS and Javascript. Should be able to set Wake up time, lunch, nap and party time. An image and text will be displayed based on the set time/ selected time. Further add a button to make the current time as “party time”. Styling can be done as per interest.

**Solution 2 -** The source code is attached in Appendix - 1. The first section of the page consist of the current time which is updated every second using “setInterval()” function. The current time is displayed in the format: hours + “:” + minutes + “:” + seconds + “ “ + meridian + “!”. “meridian” is set to “AM” by default and if current hour is greater than or equal to noon (12), meridian is changed to “PM”. A drop down is given for the users to set Wake up time, lunch and nap time. Once the current time is in the range of the selected time, a respective message and image is displayed. If the current time is not within the range of any of the selected time, a default message based on current time and Image is displayed.

Further, a button namely “Party Time” is also included in the page to set the current time as the “part time” and the button text is changed to “Party Over!”. A specific message and image are displayed based on whether the text is “party time” or “party over”. Once the “party over” button is clicked the original message and image is displayed.

The screenshots below show two cases. One before clicking “party time”, and the one after clicking “party time”.

![image](https://user-images.githubusercontent.com/107001929/188275855-7b35cdc5-2c61-4939-8796-21766ee79671.png)

                                  Figure 2: Basic Web page outlook

![image](https://user-images.githubusercontent.com/107001929/188275867-bcbdf983-cc4e-4e1f-8825-cc84db3b0de0.png)

                        Figure 3: The image and message changes once "party time" button is clicked.

The below screenshot shows when the nap time range is changed to “4 PM - 5PM”. A similar change occurs when the other times are changed.

![image](https://user-images.githubusercontent.com/107001929/188275892-211738c4-6b2a-4ed8-b8dc-0478a810844c.png)

                         Figure 4: NapTime is changed to a different time Range

**Task 3** - Built a website with two web pages, namely HOME and Register, using mainly Bootstrap (v4) and it should meet the following requirements:

1.  The HOME page should consist of a:
-   Navigation Bar
-   Carousel Slide - at least 3 images in a slide show with previous and next button
-   The body of the page must consist a container that containers a button for collapsing images, the images must be displayed in a card structure. Container should also implement Popover, Tooltip, Accordion, a Table and Pagination to navigate from Home to Register Page.
1.  Register Page should consist of a:
-   Navigation Bar
-   A container implementing Form-group as the body.
-   The form should consist of First Name, Last Name, Email, Password, a check box selection, Radio Button selection, Drop down, Date picker, Range selector, a number input, file upload and a Text area with a default message. All the fields should have proper validations. The validations must be met before form submission.
-   Need not retain the submitted form data.
-   Pagination to redirect to HOME page.

**Solution 3 -** The web pages run on a local server ([http:127.0.0.1:5500/Bootstrap_Tutorial/index.html](http://127.0.0.1:5500/Bootstrap_Tutorial/index.html), where Bootstrap_Tutorial is the directory and index.html is the file name).

1.  HOME Page:

Below attached are various sections from the Home page.

The screenshot below shows a Navigation bar and a slide show. It is an automated slide show but can also be controlled using the “previous” arrow button and “next” arrow button. Clicking on “Register” in the Navigation bar will take to the next web page. The others in the list namely, “About”, “Training”, “Contact” doesn’t do anything.

![image](https://user-images.githubusercontent.com/107001929/188275909-bc03fc3d-01bb-401f-9069-d9ff5010f689.png)

                                   Figure 5: NavBar and Slide Show

The container section consists of a collapse section, Popover, ToolTip, a card structure with data toggle capability, table and Pagination.

![image](https://user-images.githubusercontent.com/107001929/188276004-1d150f24-ec00-4b30-b345-bb727ee6ba20.png)

                                    Figure 6: Container Section

The “Click Me” will collapse images which are in a Card Structure, the “Toggle popover” button will display some additional information about the text in the button. Th popover button can have any text value. Tooltip is mainly used to pop-up some small text when you hover over it. The text can be displayed on top, bottom, left or right. “Item \#1, \#2, \#3” are in a card structure and has the ability to expand one at a time. Clicking on “item \#1” will expand it but on clicking “item \#2”, “item \#1” will be collapsed and “item \#2” expanded (known as Accordion).

![image](https://user-images.githubusercontent.com/107001929/188276014-a74f5d8d-cb92-48cf-82e6-1af7bebbdd7f.png)

                      Figure 7: Collapsing, cards, popover and tooltip

The last section of the Home page includes the Table for displaying some data using Bootstrap and Pagination where “1” is for Home page (highlighted in the screenshot below) and “2” for Register Page. Programming for “Previous” and “Next” but is not included in this Task.

![image](https://user-images.githubusercontent.com/107001929/188276025-7311075a-21e2-4b83-9676-657fd42a893e.png)

                                 Figure 8: Table and Pagination

1.  Register Page

The form (as shown below) consist of all the necessary fields with proper validations. “2” in pagination is highlighted to indicate that it is the second web page and “Register” is navigation bar is also highlighted.

![image](https://user-images.githubusercontent.com/107001929/188276033-fdaefaa0-b5fd-4a45-9a3e-78fed7d5c1e7.png)

                                            Figure 9: Register Form

Few other tasks were also done as part of “Section 1” but, the above mentioned are the three main tasks used for the assessment.

**Section 2: -**

**Task 1** - Using Angular recreate the form structures in SMARTShip application by the company - Alpha Ori Technologies (as shown in screenshots below). Both the screenshot should be on the same page, where certain sections of the page is changed when drop-down value is changed from “12334” to “NEW WESSEL”.

![image](https://user-images.githubusercontent.com/107001929/188276063-81b95339-5776-4211-b113-2c1c3df2c5e8.png)

                     Figure 10: The original Form structure ("12334")

![image](https://user-images.githubusercontent.com/107001929/188276077-1e3084ed-f82d-47fb-8aa3-ff10f89d7aea.png)

                Figure 11: Form Structure changed when the selection is "NEW WESSEL"

Proper validations must be done and as shown in the screenshot, validation error must change the border color from white to red. On clicking “Save”, the data in the “formgroup” must be converted to JSON.

**Solution 1 -** Local server <http://localhost:4200/> is used to open the application on the browser. To open the application, navigate to the application folder in command prompt or terminal and use the command “ng serve --open” as shown in the screenshot below.

![image](https://user-images.githubusercontent.com/107001929/188276345-1ed0ca4e-b7bb-4213-ad1b-5081665b55c9.png)

                  Figure 12: Opening Angular application- formApp

The below screenshots show the form structure where the user enters vessel related information. For “New Wessel”, some key information like “Vessel IMD”, “Vessel Name”, “Vessel Type” etc is needed whereas for already existing Wessel (either “12334” Or “ADXAXASX”) these details are already available hence need to be removed from the form page and the user doesn’t have to enter them again.

Below are the screenshots for adding a New Wessel and for an existing Wessel but, both are part of the same “formgroup” or form structure.

![image](https://user-images.githubusercontent.com/107001929/188276351-9641705d-f9b3-4879-a95f-fc29952ed9c0.png)

                  Figure 13: formApp- New Wessel

![image](https://user-images.githubusercontent.com/107001929/188276357-78f2f54a-e655-4bdd-86c2-299888c3edf9.png)

                Figure 14: formApp - Existing Wessel

On clicking “Save” button, it will check for validations. If validations are not met, it will change the bottom border color from white to red. If all the validations (checks whether any required fields are empty and if not check whether the input is valid or as per requirement), the a JSON output is produced. This data can be stored in database or can be used for any other purpose. JSON format is the easiest way to transfer data from client-side to server- side. The generated JSON is displayed or logged in the console layout (as shown in the screenshot below).

![image](https://user-images.githubusercontent.com/107001929/188276371-009e8ec7-0ac8-4f85-ac7e-669e70192a08.png)

                   Figure 15: console layout with JSON data

**Task 2** - Implement the following:

-   Routing, Rest API with CRUD (create, read, update, delete) operation.
-   Lodash in Angular
-   Table filtering without using any additional Angular packages.
-   Parent/ Child component
-   Observables

**Solution 2 -**

Lodash is an open-source JavaScript utility library delivering consistency, modularity, performance and extras. Lodash helps programmers to write more concise and maintainable JavaScript. An example of some of the Lodash library functions, as shown in screenshot below (Figure 16), is down with the help of this [article](https://edupala.com/how-to-use-lodash-in-angular/).

Angular Routing - In a single-page application, you change what the user sees by showing or hiding portions of the display that correspond to particular components. rather than going out to the server to get a new page. As users perform application tasks, they need to move between the different views that you have defined.

To handle the navigation from one view to the next, you use the Angular Router. The Router enables navigation by interpreting a browser URL as an instruction to change to view.

The Routing section in the screenshot below (Figure 16), navigates to a different view of the section on clicking “Product Detail” link. The current view is “localhost:4200”, clicking “Product Detail” on a particular product will lead to “localhost:4200/emission/:productid”.

On clicking “Product Detail” (in Figure 16) corresponding to product name- “shoes”- it will navigate to a different view as shown in screenshot in Figure 17, where 3456788 is the “productid” for “shoes. The button “Go to List” will help to navigate back to original view (localhost:4200). The button “Contact List” (in Figure 16) will navigate to a different view (localhost:4200/contacts) which consist of CRUD operation (as shown in Figure 18). The data displayed in the table (in Figure 18) is stored in a local server (JSON Server). “New” button will help in adding new row to the table (create), “Edit” button will help to update a row, “View” button to Read a row contents in detail and finally, “Delete” button to remove a row from the table.

![image](https://user-images.githubusercontent.com/107001929/188276382-2bdc6395-9d2d-48e0-aee2-31b9e7ec97d0.png)

                     Figure 16: Routing and Lodash Implementation

![image](https://user-images.githubusercontent.com/107001929/188276389-9135889c-3149-4198-b2df-a02aaacebfbc.png)

                         Figure 17: Routing- A different View

![image](https://user-images.githubusercontent.com/107001929/188276396-287bd3f2-f627-49a9-b608-7f75f34d7efc.png)
                              
                              Figure 18: CRUD Operation

Table search is done on a normal table. It consists of three inputs and data binding is done using “[ngModal](https://appdividend.com/2022/01/19/angular-ngmodel/)”- helping to get the value entered in the HTML component. This value is further used to compare with the data in the Table. If a match is found, then only that data is returned to the template to be displayed.

![image](https://user-images.githubusercontent.com/107001929/188276414-ccdc13ab-5314-4ef3-9a33-59e248fde3f8.png)

                               Figure 19: Table Filtering

The below screenshots show how parent and child components interact with each other. It implements various methods used for the interaction.

![image](https://user-images.githubusercontent.com/107001929/188276422-c8728e4e-2642-4ff5-ac84-655f98ba80ac.png)

                            Figure 20: Parent/ Child Interaction - 1

The below screenshot is another example of Parent child interaction, without the need for navigating to a different view. The table content is edited on the same page or same view (localhost:4200).

![image](https://user-images.githubusercontent.com/107001929/188276549-9543522d-ce85-4d44-8c0e-38633cae743f.png)

                              Figure 21: Parent/ Child Interaction - 2

Finally, Reactive programming enables the data stream to be emitted from one source called **Observable** and the emitted data stream to be caught by other sources called **Observer** through a process called subscription. This Observable / Observer pattern or simple **Observer** pattern greatly simplifies complex change detection and necessary updating in the context of the programming. **RxJs** is a JavaScript Library which enables reactive programming in JavaScript. **Rxjs** provides lot of method to create **Observable** from common JavaScript Objects. Angular, make use od Rxjs library to implement Observable.

The below screenshot implements the concept of Observable and takes a number (n) as input and calculate sum of all numbers from 1 to n.

![image](https://user-images.githubusercontent.com/107001929/188276555-9c9476c2-48e1-452d-b0b9-80a8eef4cd5c.png)

                                Figure 22: Observable Implementation

With the above two tasks Section 2 was completed successfully.

**Section 3: -**

**Task 1**- Implement Rest API (get, post, put, delete) using NodeJs. Can use any database of choice.

**Solution 1 -** The solution requires connecting to a database, in this case MySql is used for data storage and retrieval. The NodeJs code used for database connection establishment, routing, MySql query for getting contents of MySql table, inserting, updating and deleting is also included in the NodeJS code folder. Any port number can be used for this. Localhost:3000/ will display a message “Ok” in JSON format.

The output was verified using POSTMAN. The screenshots for each operation is attached below:

![image](https://user-images.githubusercontent.com/107001929/188276563-7c6d4ddb-fb5a-43e1-9f6e-c482514bfb67.png)![](media/33d44e2b01e3c947533251ce4ec2d152.png)

                         Figure 23: GET operation- retrieves all the data from the database.

Similarly, data of a specific ID can also be retrieved using MySql query. The screenshot below demonstrates “POST” and “Delete” a row from the MySql table. Similarly, “PUT” operation (updating a particular row in the table) can also be done.

![image](https://user-images.githubusercontent.com/107001929/188276566-c4dfe0ce-7aa2-44ce-a796-e851e552b06f.png)

                                 Figure 24: POST Operation

![image](https://user-images.githubusercontent.com/107001929/188276577-0ba38ade-b285-4b3e-baaf-e01c3523b519.png)

                                Figure 25: Delete Operation

**Task 2**- Implement SignUp/ Login using Angular for Frontend Development and NodeJS for backend Development. A database of choice can be used to store user login credentials. Use a secret token (JSON web token) for authentication and “bcrypt” is used for credential comparison.

**Solution 2 -**

The signUp page requires some basic details as shown in screenshot below and “Sign Up” button will be enabled once all the fields are entered. 

![image](https://user-images.githubusercontent.com/107001929/188276585-c819ec9d-b0cc-4100-9c9e-f0fd5a6c8979.png)
      
                                    Figure 26: SignUp Page

Login/SignUp page - authentication is done using JWT and password is hashed before storing user details to database.

![image](https://user-images.githubusercontent.com/107001929/188276599-f012cb80-0560-4b72-9cbd-55901913941f.png)

                                    Figure 27: Login Page

View Page - On successful login, post details are displayed.

![image](https://user-images.githubusercontent.com/107001929/188276605-5ee9095e-bf65-4adb-bdf0-c2b67b0952a7.png)

                             Figure 28: Login Success and View Page

Add Page - Create new post and upload a file. Post title, body and filename is added to the database. File is saved in the server-side directory.

![image](https://user-images.githubusercontent.com/107001929/188276612-b899b9f6-f846-4fe0-8b8f-b2e87f41ecc2.png)

                                    Figure 29: Create Page

![image](https://user-images.githubusercontent.com/107001929/188276620-56bf882f-ab60-4361-bba1-e031e5f7bc94.png)

                                  Figure 30: Updated View Page

Edit Page - Can edit post title and body.

Delete Post - delete icon in view page is used to delete the entry from the database and to delete uploaded file from the server-side.

![image](https://user-images.githubusercontent.com/107001929/188276627-abb47484-693b-481b-a30a-004c8949e3d5.png)

                                       Figure 31: Edit Page

Technologies used: Angular, Nodejs

