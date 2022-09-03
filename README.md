# project-screenshots
Some screenshots of my projects.
# Tasks and Project Results

**Task 1** - Recreate <https://www.javascripttutorial.net/sample/dom/countdown-timer/> , a website that does 2023 new year countdown. All the computations must be done only using JavaScript and CSS for page styling.

**Solution 1 -** The webpage was recreated in the local server (<http://127.0.0.1:5500/countdown_timer/index.html>, where countdown_timer is directory and index.html is the file name).

The calculations are done in JavaScript. This involving setting end time to ‘January 01 {current year + 1} 00:00:00’. This can be done using new Date() function and the current year can be obtained using new Date().getFullYear(). The remaining time is obtained by subtracting the current time from the end time. The difference is formatted to the required (days hours minutes seconds) format. If the remaining time is less than 0, counter is cleared and a new timer is started for the next year (current year + 1). If it is greater than 0, the remaining time or counter is displayed and updated every second (that is, remaining time is decremented every minute). If the remaining time is 0, a message - “Happy New Year {Year} “- is displayed. This message is hidden in all other cases.

Styling is down using CSS. Background image can be set to any image using “background-image: url(‘’);” and the font-size and other display features can be set as per requirement.

A screenshot of the final result is attached below:

![](media/8fdf13aec23f47f002b431317655ccab.png)

Figure 1: New Year Countdown Web page

**Task 2** - Create a web page to display current time as a clock using HTML, CSS and Javascript. Should be able to set Wake up time, lunch, nap and party time. An image and text will be displayed based on the set time/ selected time. Further add a button to make the current time as “party time”. Styling can be done as per interest.

**Solution 2 -** The source code is attached in Appendix - 1. The first section of the page consist of the current time which is updated every second using “setInterval()” function. The current time is displayed in the format: hours + “:” + minutes + “:” + seconds + “ “ + meridian + “!”. “meridian” is set to “AM” by default and if current hour is greater than or equal to noon (12), meridian is changed to “PM”. A drop down is given for the users to set Wake up time, lunch and nap time. Once the current time is in the range of the selected time, a respective message and image is displayed. If the current time is not within the range of any of the selected time, a default message based on current time and Image is displayed.

Further, a button namely “Party Time” is also included in the page to set the current time as the “part time” and the button text is changed to “Party Over!”. A specific message and image are displayed based on whether the text is “party time” or “party over”. Once the “party over” button is clicked the original message and image is displayed.

The screenshots below show two cases. One before clicking “party time”, and the one after clicking “party time”.

![](media/9be5da3a98d81044cb9d9ed53706af29.png)

Figure 2: Basic Web page outlook

![](media/d38c14757907f7b4c6ea99efa5bef61e.png)

Figure 3: The image and message changes once "party time" button is clicked.

The below screenshot shows when the nap time range is changed to “4 PM - 5PM”. A similar change occurs when the other times are changed.

![](media/ed241eb558b741b1944100e3a309dbd5.png)

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

![](media/5e3359bb5ad84ec89b0d82df58f3dbdb.png)

Figure 5: NavBar and Slide Show

The container section consists of a collapse section, Popover, ToolTip, a card structure with data toggle capability, table and Pagination.

![](media/58d58036bcde05516cf66a3a68dd2f71.png)

Figure 6: Container Section

The “Click Me” will collapse images which are in a Card Structure, the “Toggle popover” button will display some additional information about the text in the button. Th popover button can have any text value. Tooltip is mainly used to pop-up some small text when you hover over it. The text can be displayed on top, bottom, left or right. “Item \#1, \#2, \#3” are in a card structure and has the ability to expand one at a time. Clicking on “item \#1” will expand it but on clicking “item \#2”, “item \#1” will be collapsed and “item \#2” expanded (known as Accordion).

![](media/83f87b0face464c56e0b9911e5ffe674.png)

Figure 7: Collapsing, cards, popover and tooltip

The last section of the Home page includes the Table for displaying some data using Bootstrap and Pagination where “1” is for Home page (highlighted in the screenshot below) and “2” for Register Page. Programming for “Previous” and “Next” but is not included in this Task.

![](media/94d57a69349950b4dd9660d49903c2f1.png)

Figure 8: Table and Pagination

1.  Register Page

The form (as shown below) consist of all the necessary fields with proper validations. “2” in pagination is highlighted to indicate that it is the second web page and “Register” is navigation bar is also highlighted.

![](media/5f78748baf57748db4a0d7d81a9be0da.png)

Figure 9: Register Form

Few other tasks were also done as part of “Section 1” but, the above mentioned are the three main tasks used for the assessment.

**Section 2: -**

**Task 1** - Using Angular recreate the form structure as shown in below attached screenshot. Both the screenshot should be on the same page, where certain sections of the page is changed when drop-down value is changed from “12334” to “NEW WESSEL”.

![](media/d747003c1a4c0cc0f1d8c19add4993ed.png)

Figure 10: The original Form structure ("12334")

![](media/3bdcc85bdc9a0e8db802b85a64f3004e.png)

Figure 11: Form Structure changed when the selection is "NEW WESSEL"

Proper validations must be done and as shown in the screenshot, validation error must change the border color from white to red. On clicking “Save”, the data in the “formgroup” must be converted to JSON.

**Solution 1 -** Local server <http://localhost:4200/> is used to open the application on the browser. To open the application, navigate to the application folder in command prompt or terminal and use the command “ng serve --open” as shown in the screenshot below.

![](media/f3edba9e1a3f351b186b009bab05c5fa.png)

Figure 12: Opening Angular application- formApp

The below screenshots show the form structure where the user enters vessel related information. For “New Wessel”, some key information like “Vessel IMD”, “Vessel Name”, “Vessel Type” etc is needed whereas for already existing Wessel (either “12334” Or “ADXAXASX”) these details are already available hence need to be removed from the form page and the user doesn’t have to enter them again.

Below are the screenshots for adding a New Wessel and for an existing Wessel but, both are part of the same “formgroup” or form structure.

![](media/9a54f4030856c46fea12f2e817c6e6d4.png)

Figure 13: formApp- New Wessel

![](media/fb5b1bbd901e423082e584a5aad20211.png)

Figure 14: formApp - Existing Wessel

On clicking “Save” button, it will check for validations. If validations are not met, it will change the bottom border color from white to red. If all the validations (checks whether any required fields are empty and if not check whether the input is valid or as per requirement), the a JSON output is produced. This data can be stored in database or can be used for any other purpose. JSON format is the easiest way to transfer data from client-side to server- side. The generated JSON is displayed or logged in the console layout (as shown in the screenshot below).

![](media/02ea00c52657389c3fae934f4e4e777c.png)

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

![](media/79c36a8b8c6f21b40f5aaedb82821071.png)

Figure 16: Routing and Lodash Implementation

![](media/53bba4250be3a5783c7266af6471f0c2.png)

Figure 17: Routing- A different View

![](media/72ef5c1b26b75f1651155d7e865961e9.png)

Figure 18: CRUD Operation

Table search is done on a normal table. It consists of three inputs and data binding is done using “[ngModal](https://appdividend.com/2022/01/19/angular-ngmodel/)”- helping to get the value entered in the HTML component. This value is further used to compare with the data in the Table. If a match is found, then only that data is returned to the template to be displayed.

![](media/15f609ce6508f51880e8ba300261b0f3.png)

Figure 19: Table Filtering

The below screenshots show how parent and child components interact with each other. It implements various methods used for the interaction.

![](media/c04b4589e929ae4bd915acd91fa212c5.png)

Figure 20: Parent/ Child Interaction - 1

The below screenshot is another example of Parent child interaction, without the need for navigating to a different view. The table content is edited on the same page or same view (localhost:4200).

![](media/966f21ad563a9165d46983fd3a9dc86d.png)

Figure 21: Parent/ Child Interaction - 2

Finally, Reactive programming enables the data stream to be emitted from one source called **Observable** and the emitted data stream to be caught by other sources called **Observer** through a process called subscription. This Observable / Observer pattern or simple **Observer** pattern greatly simplifies complex change detection and necessary updating in the context of the programming. **RxJs** is a JavaScript Library which enables reactive programming in JavaScript. **Rxjs** provides lot of method to create **Observable** from common JavaScript Objects. Angular, make use od Rxjs library to implement Observable.

The below screenshot implements the concept of Observable and takes a number (n) as input and calculate sum of all numbers from 1 to n.

![](media/90fa227cb46b032e3b98c0bf47f14ebd.png)

Figure 22: Observable Implementation

With the above two tasks Section 2 was completed successfully.

**Section 3: -**

**Task 1**- Implement Rest API (get, post, put, delete) using NodeJs. Can use any database of choice.

**Solution 1 -** The solution requires connecting to a database, in this case MySql is used for data storage and retrieval. The NodeJs code used for database connection establishment, routing, MySql query for getting contents of MySql table, inserting, updating and deleting is also included in the NodeJS code folder. Any port number can be used for this. Localhost:3000/ will display a message “Ok” in JSON format.

The output was verified using POSTMAN. The screenshots for each operation is attached below:

![](media/33d44e2b01e3c947533251ce4ec2d152.png)

Figure 23: GET operation- retrieves all the data from the database.

Similarly, data of a specific ID can also be retrieved using MySql query. The screenshot below demonstrates “POST” and “Delete” a row from the MySql table. Similarly, “PUT” operation (updating a particular row in the table) can also be done.

![](media/197952769a0283141be8f57e6b9a482e.png)

Figure 24: POST Operation

![](media/ed4ec2bce1c4884a0293df71c4d2e819.png)

Figure 25: Delete Operation

**Task 2**- Implement SignUp/ Login using Angular for Frontend Development and NodeJS for backend Development. A database of choice can be used to store user login credentials. Use a secret token (JSON web token) for authentication and “bcrypt” is used for credential comparison.

**Solution 2 -**

The signUp page requires some basic details as shown in screenshot below and “Sign Up” button will be enabled once all the fields are entered. ![](media/d69f75c64ddc61e36a834f5d367f9dc5.PNG) Figure 26: SignUp Page

Login/SignUp page - authentication is done using JWT and password is hashed before storing user details to database.

![](media/86e0976007b5377bce879e4adea4ca14.png)

Figure 27: Login Page

View Page - On successful login, post details are displayed.

![](media/d6dfd57044eea6b5439fdb5ad67e1c11.PNG)

Figure 28: Login Success and View Page

Add Page - Create new post and upload a file. Post title, body and filename is added to the database. File is saved in the server-side directory.

![](media/e9c4834e42f53bae5020456787a439ab.PNG)

Figure 29: Create Page

![](media/2a1c59e5a24277b1a3f861233248216f.PNG)

Figure 30: Updated View Page

Edit Page - Can edit post title and body.

Delete Post - delete icon in view page is used to delete the entry from the database and to delete uploaded file from the server-side.

![](media/8d5b6a5fb59003863defc50c5e5c9f77.PNG)

Figure 31: Edit Page

Technologies used: Angular, Nodejs

