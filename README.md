# Project Unit 3: Journalism club application
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/project3.gif)

# Criterion A: Planning 
### Definition of the Problem
UWC ISAK Japan is a school that always strives to be more environmentally friendly, but due to high demand for copies of ISAK INSIDER articles every week, a lot of paper is being used to print them. This especially bothered Jonathan Wang Ye, who is considered by many, number one environmentalist at ISAK, probably even Japan. He is in urgent need for an UWC ISAK journalism club application which would store articles that ISAK INSIDER publishes every week in addition to storing articles from past weeks. He also demands the highest level of security due to the fact that this would be an official school app, so all the passwords must be encrypted, protecting data of app's users. Other than being more green, additional benefit of this app would be that it would nake articles available anywhere in the world, allowing fans and alumni of the school outside ISAK to enjoy it.
This way everyone would be able to enjoy ISAK INSIDER without hurting the environment by wasting paper in the process.


### Success criteria
 1. The application contains account registration and login feature using username email and adequate password.
 2. Differentiates normal readers and editor accounts which would have an option to add articles if their account is authorized as a journalism club member.Viewers can only read. Editors have a feature of adding articles.
 3. Application will have a feature to add an article and safely store it.
 4. Option to see image of the article, allowing full expirience of digital newspapers.
 5. Option to view past articles containing the author, title, and its content.
 6. Option to select multiple articles and read them one after another, just like in digital newspapers.
 7. Option to delete articles created by the user logged in.
 


### Design statement
I will design an aplication for Jonathan Wang Ye, UWC ISAK student. This will be a journalism club application and will serve to display Isak insider articles in digital format. It will be a desktop application, and will be developed in the one month period.

---

### Rationale for proposed solution
For the development of this project, I will use Python programming language, KivyMD library for the user interface, and SQL for the databases used in the application.

Considering the client's requests, I will design and develop this easy-to-use centralized application for managing UWC ISAK's journalism club articles. It will be developed using Python programming language, KivyMD library for the user interface, and SQL for the databases used in the application.
#### Why Python?
**Python** Python versatility allows a great cross platform development[^1] which is a neccesity for the application I will be developing. Python has a large and active community of users and developers. This means that there is a wealth of resources available to help you learn the language and build your application, as well as a large pool of talented developers who can contribute to your project.[^2] Python has a simple, intuitive syntax that makes it easy for new users to learn and for experienced developers to quickly pick up. This makes it a good choice for building applications quickly and with fewer bugs, as well as for prototyping new ideas.[^3]
#### Why KivyMD?
One of the main advantages of using **KivyMD** is that it allows developers to build applications that can run on multiple platforms, including Android, iOS, and Windows. This makes it an ideal choice when targeting wide & international audiance like ISAK's journalism club application would.It is also very suitable for co-developing due to small number of variables used allowing easy interpretation and allowing easy extensibility of the application. This can help to save time and effort, allowing developers to focus on creating their app's functionality and features. KivyMD offers a wide range of customization options that allow developers to tailor their apps to meet the specific needs of their users.[^4]
When compared to another UI creating software such as Flutter, KivyMD has more advantage on some components like more supportive online community, user-friendliness but most importantly KivyMD is better as it can work with python coding language while Flutter cannot which therefore is more suitable in this project.[^5]
#### Why SQL?
**SQL** is designed to handle large amounts of data efficiently. This makes it an ideal choice for applications that needs to scale as they grow such as this one, as SQL databases can be easily expanded to meet the needs of the application. SQL databases allow for the storage of structured data, which can be easily queried and manipulated. This makes it easier to find the information you need, and to perform complex data analysis tasks. SQL databases are highly reliable, and offer features such as transaction management and data integrity to ensure that the data stored in the database remains accurate and up-to-date.[^6]

# Criterion B: Solution Overview 
### Diagrams
flow diagram
### System Diagram
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/System%20Diagram%20Final.png)
Fig.1 shows the system diagram of the jounalism club application.

The application will run on Python and KivyMD. The application will ask for various inputs from the users. They will all be stored within a database using SQLite. All of this will be executed within the Pycharm application, which will then display the output on a screen.
### Wireframe Diagram
Final version
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/wireframediagram.jpg)

Fig.2 shows final wireframe diagram of the journalism club application
### ER Diagram 
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/finalerdiargam(3).png)
Fig.3 shows the ER diagram of the journalism club application

### UML Diagram
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/UML_Diagram_project3%20-%20UML%20Class%20(1).png.crdownload)
Fig. 4 shows UML diagram of the journalism club applicaton. This diagram presents all classes used in this project. There are 2 main parent classes: MDScreen and MDApp. All subclasses inherit methods and attributes from these parent classes, as indicated by the arrows in the diagram.
The database_worker class establishes connection to a SQLite3 database, searches for specific data needed, gets it, and closes the connection afterwards.

### Flow diagrams
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/Flow_diagram_registration_project3%20-%20Flowchart.png)
Fig. 5 shows the flow diagram of the method used for registration of a new account. It validates data entered for name, email, password and repeat password text fields, and if all credential requirements are met, the accoutn is successfully created and added into account database.

![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/Flow%20chart%202%20project%203.png)
Fig. 6 shows the flow diagram of the method read which used to view selected newspapers articles. It displays articles in the order of selection using popup screens.

![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/Flow%20diagram_update_project3.png)
Fig. 7 shows the flow diagram of the update method. This method serves to update the article table displayed in the read articles feature. This is so that when an article is deleted, it stops being displayed in the article table. This method is called everytime article/es is/are deleted so that the article table is reliable showing only relevent articles.
### Test Plan

|Test Number|Description|Test Type| Target|Procedure|Expected Outcome|
|-----------|-----------|--------|-----------|-----------------|----|
|1|Account registration system|Unit testing|Have a fully functional registration system that checks if the proper values are inputed in the email and password fields|(1) Run Project_3.py (2) Click the register button on the login screen (3) Input data on all the fields (4) After filling in all the fields create an account (5) Try to login with the new account too see if it exists now| After following the procedure, a user should be able to login using the credentials of the new account created|
|2|Reading articles|Unit Testing|Be able to read articles that are checked, after clicking the read article button|(1) after entering the read article feature, select desired articles by checking the box next to them (2) Click read article button in the bottom right corner (3)If you selected multiple by clicking outside of the popup screen, you will see the next selecte article and its content |Will have a working read article feature which allows users to read selected articles|
|3|Article adding/viewing|Integration testing|Have a functional system of adding an article, and viewing it|(1) Login using editor account (2) Go to add article option and add article by filling in all neccesarry fields (3) Go to read articles feature and see if the newly add article is visible in the article table | New article should be visible at the bottom of the article table|
|4|Article image url adding and image viewing|Integration testing|When creating an article and and adding its article image url, you can inpect the image when reading the article|(1) Upload a picture to the file conating the program (2)Sign in as an isak editor and go to add article option (3) Fill out neccesary fields to add an article and put in photos url. (4) Go to read aricle and selected newly added article. (5) Select read arrticle option. (6) Select view article photo option and check if the adequate photo is displayed|The article photo is accesable when reading selected article.|
|5|Delete and read article features code review |Code Review|Make the code behind read and delete functions understandable to possible future developers|(1) Check the code section which contains objects delete and read for any confusing variable names (2) Add comments next any non trivial coding procedures (3) Make any repetitive procedures into a loop| Code looks a lot more understandable now. Comments were added next to the more difficult parts of the code|
|6|Full Python Code Review|Code Review|The changed variable names and added comments will help the user to understand how the code functions|Check the Project_3.py file for any: (1) inadequate Variable names (2) missing comments (3) Repetition	and unefficient programming methods| The code is now easy to follow and allows future developers of it to modify it and use it efficiently .|                                                                                                                                                                                                                                                                                                                                                                                         

Table 1:
>Shows the test plan containing information about testing done for this application. There are 3 different types of tests presented in the test plan which are unit test(to test one part of the program), integration test(to test the cooperation of different parts) and code review(to check the quality of code). Table shows description, steps to follow, and expected output with a goal to help user understand the process better.
>
### Record of tasks

|    | Planned Action                                        | Planned Outcome                                                                            | Time Estimate | Target Completion | Criteria |
|----|--------------------------------------------------------------------------------------------|----------------|---------------|-------------------|----------|
| 1  | First meeting with client                             | To understand client problem and requirements                                              | 10 minutes    | 10.2.2023           | A        |
| 2  | Write down success criteria                           | To list down the first success criteria                                                    | 20 minutes    | 12.2.2023           | A        |
| 3  | Write problem definition                              | Have problem definition which will identify who client is and the product that client want | 20 minutes        | 12.2.2023           | A        |
| 4 | Research and write rationale for proposed solution    | Finish rationale for proposed solution                                                     |  1 hour 10 minutes       | 12.2.2023          | A        |
| 5  | Update success criteria                               | List more success criteria and prepare for presentation to client                          | 15 minutes    | 13.2.2023         | A        |
| 6  | Starts working on login and registration system       | Finish login and registration system with database                                           | 2 hours        | 14.2.2023         | C        |
| 7 | Working on password encryption                        | Using sha256 to encrypt password and check password in login and registration              | 15 minutes| 14.2.2023          | C        |
| 8| Meet with client to  present the success criteria     | Present success criteria to client to get the approval                                     |  30 minutes    | 21.2.2023         | A        |
| 9  | Create wireframe diagram                              | Wireframe diagram is ready to present to client as the first MVP                             | 40 minutes   | 24.2.2023          | B        |
| 10  | Create system diagram                                 | System diagram is done with details written on it                                           |  45 minutes       | 24.2.2023         | B        |
| 11 | Create welcome screen following the wireframe diagram | Have welcome screen ready                                                                    | 1 hour 30 minutes      | 24.2.2023           | C        |
|12| Create flow diagrams for parts of the code|Have finished 3 flow diagrams| 45 minutes| 24.2.2023|B|
|13| Add email validation and editor mode validation| Allow only email with @ sign and give editor access to users with @isakinsider.jp email ending|35 minutes| 24.2.2023|C|
| 14 | Present the wireframe and application to the client   | Get client's feedback on the wireframe and application| 10 minutes    |26.2.2023          | A        |
|16| Create the first version of article viewscreen| have a first vesion of the screen containing all the articles| 1 hour| 27.2.2023
| 17 | Make ER diagram                                       | ER diagram is created for both tables                                                          | 30 minutes    | 27.2.2023      | B        |
|18| Make a final Wireframe diagram| Finish with wireframe diagram that is up to clients requests, mentioned in the last meeting|15 minutes| 1.3.2023|B|
|19|Add a feature to delete an article    |Have a functioning feature that alows writer to delete its own article    |50 minutes      |1.3.2023  | C  |
|20| Add a feature to add articles as an editor    | be able to upload new articles, containing their author and title  | 40 minutes |1.3.2023  | C  |
|21| Update test plan   | Add 2 new testings performed (1 Unit and 1 code review)     |10 minutes      |1.3.2023  |B   |
|22|Finalize the integration of the add article and read article    |Be able to upload an artice and read it right away by clicking read article function      |30 min |2.3.2023  |C |
|23| Go back function from article screen | Have functioning buttons for going back to the main screen, for both editor and reader | 10 min  | 2.3.2023 |  C |
|24| Add popup alerts for logout and delete options | Have a first version of the popup alert or notification for the features mentioned | 35 min   | 4.3.2023 | C  |
|25|Improve popup functions | Modify popup functions by improving their appearance  |  15 min | 4.3.2023 | C  |
|26| Update test plan | Document two new tests performed ((1) integration of uploading an article and reading it afterwards (2) Code review of the new delete and read functions) |  10 min | 4.3.2023  | B  |
|27| Create a Popup screen containing the articles selected for reading| Have a first version of the reading function and the popup feature for articles selected for reading |  1 hour | 4.3.2023 |  C |
|28| Cite sources using MLA9 | Cite all sources used, in mla9 format  | 10min  | 5.3.2023 |  C |
|29| Add the image feature to articles | Have a function that shows the image of the article that has been selected | 1 hour 45 minutes | 6.3.2023  |  C |
|30|Make a UML diagram | Have a finsihed UML diagram, an accurate representation of all classes and object in the python code | 1 hour | 7.3.2023|B |
|31|Update test plan | Add last two tests (1 unit and one integration test)|15min| 7.3.2023| C| 
|32| Add techniques used| Have techniques used mentioned in Criteria C| 5 min| 7.3.2023| C|
|30| | | | | |
|30| | | | | |
|30| | | | | |
|30| | | | | |
|30| | | | | |

Table 2:
> Record of Task-:shows the planning and working process throughout the project. This includes: programming, documentation, client's meetings, and other  process from the start of the project to the due date. Table contains order, description, Planned Outcome, Design Cycle, Time Estimate, Target Completion, Criteria


# Criterion C: Development
### Existing tools
### Criteria number 1: The application contains account registration and login feature using username email and adequate password.
### Criteria number 2: Differentiates normal readers and editor accounts which would have an option to add articles if their account is authorized as a journalism club member.Viewers can only read. Editors have a feature of adding articles.
### Criteria number 3: Application will have a feature to add an article and safely store it.
### Criteria number 4: Option to see image of the article, allowing full expirience of digital newspapers.
### Criteria number 5: Option to view past articles containing the author, title, and its content.
### Criteria number 6: Option to select multiple articles and read them one after another, just like in digital newspapers.
### Criteria number 7: Option to delete articles created by the user logged in.


### Sources

Szabo, Gabor. "Python SQLite: Insert, Update and Delete Queries". Perl Maven. August 17, 2021, https://perlmaven.com/python-sqlite-insert-update-delete. Accessed February 21, 2023.

"KivyMD Card." KivyMD, 1.1.1, https://kivymd.readthedocs.io/en/1.1.1/components/card/. Accessed 1 Mar. 2023.

"Python String split() Method." W3Schools, Refsnes Data, https://www.w3schools.com/python/ref_string_split.asp. Accessed 2 Mar. 2023.

"Python String strip() Method." W3Schools, Refsnes Data, https://www.w3schools.com/python/ref_string_strip.asp. Accessed 2 Mar. 2023.

"KivyMD Text Field." KivyMD, 0.104.1, https://kivymd.readthedocs.io/en/0.104.1/components/text-field/index.html. Accessed 4 Mar. 2023.

Sandeep, S. "KivyMD Dialogs." The Python Code, 2021, https://www.thepythoncode.com/article/kivymd-dialogs-python. Accessed 4 Mar. 2023.

"KivyMD Dialog." KivyMD, 1.1.1, https://kivymd.readthedocs.io/en/1.1.1/components/dialog/index.html. Accessed 5 Mar. 2023.

### Techniques used:
1. Object Oriented Programming (OOP)( Classes, Inheritance)
2. Manipulating SQLite Database
3. Variables
4. For loops
5. If statements
6. Functions
7. Password Hashing
# Criterion D: Functionality 
### Format
A video demonstrating the testing for the success criteria.

Max. length 4 min
### Extensibility
The last 30s of the video should include a discussion of how the code is well organized so that future developers can extend it
### Appendex
#### CLIENT MEETING 1
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/Project_3_appendex.png)
#### CLIENT MEETING 2
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/clientmeetingfinal.jpg)

### Citations
[^1]:"Python." Wikipedia, Wikimedia Foundation, 12 Feb. 2023, https://en.wikipedia.org/wiki/Python. ↩

[^2]:"Why Choose Python." Python.org, Python Software Foundation, 12 Feb. 2023, https://www.python.org/about/gettingstarted/. ↩

[^3]:"Python for Data Science Handbook." O'Reilly, O'Reilly Media, Inc., 12 Feb. 2023, https://www.oreilly.com/library/view/python-for-data/9781491912126/ ↩

[^4]:Gupta, Kaustubh. “What Is KivyMD | Creating Android Machine Learning Apps Using KivyMD.” Analytics Vidhya, 30 June 2021, www.analyticsvidhya.com/blog/2021/06/creating-android-ml-app-kivymd/#:~:text=KivyMD%20is%20built%20on%20the. Accessed 13 Feb. 2023.
[^5]:“Kivy vs Flutter | Learn the Key Differences between Kivy and Flutter.” EDUCBA,  July 2021, www.educba.com/kivy-vs-flutter/.
[^6]:"SQL." W3Schools, 13 Feb. 2023, https://www.w3schools.com/sql/ ↩
