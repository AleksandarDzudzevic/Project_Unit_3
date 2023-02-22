# Project Unit 3: Journalism club application
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/project3.gif)

# Criterion A: Planning 
### Definition of the Problem
UWC ISAK Japan is a school that always strives to be more environmentally friendly, but due to high demand for copies of ISAK INSIDER articles every week, a lot of paper is being used to print them. This especially bothered Jonathan Wang Ye, who is considered by many, number one environmentalist at ISAK, probably even Japan. He is in urgent need for an UWC ISAK journalism club application which would store articles that ISAK INSIDER publishes every week in addition to storing articles from past weeks. He also demands the highest level of security due to the fact that this would be an official school app, so all the passwords must be encrypted, protecting data of app's users. Other than being more green, additional benefit of this app would be that it would nake articles available anywhere in the world, allowing fans and alumni of the school outside ISAK to enjoy it.
This way everyone would be able to enjoy ISAK INSIDER without hurting the environment by wasting paper in the process.

Who is the client?
Why is the product being developed

### Success criteria
 1. Option to create an account with a signup and login feature that allows usage of the application by validating password and username, not allowing identical usernames.
 2. Users' passwords are securly stored. 
 3. Differentiates normal readers and editor accounts which would have an option to add articles if their account is authorized as a journalism club member. Viewers can only read. Editors have a feature of adding articles.
 4. Option to add a picture inside of the article, allowing full expirience of digital newspapers.
 5. Option to view past articles containing the author, title, date, picture and its content.
 6. Option to choose the edition of newspapers the user wants to view, with articles grouped by the dates.



### Design statement
In order to satisfy client's needs, I will develop a journalism club application that will serve as a place where users could read ISAK Insider articles. The application will be developed using Python programming language and the Kivy MD library for the user interface design. The data for the journalism club applicaation will be stored using SQL. SQL is perfect for handling large quantity of data, such as weekly newspapers articles .Using SQL to store those will allow smooth operation and accurate data accessing as SQL has many features that allow access to a specific type of data needed, depending on the parameters entered, and all that is done very efficiently.

---

### Rationale for proposed solution
For this project the application will have login/signup system in order to distinguish journalism club editor accounts which would have the feature to add articles, so login in system is needed to allow this. And it will be a user friendly application in order for clients to use it without instruction needed, anywhere in the world. The application will also allow client to choose articles from previous weeks, which is a huge upgrade compared to previous hardcopy articles model. All of the content just one click away, anywhere in the world.

Considering the client's requests, I will design and develop this easy-to-use centralized application for managing UWC ISAK's journalism club articles. It will be designed and developed using Kivymd, Python, and SQlite.
#### Why Python?
**Python** is a versatile language and can be used for a wide range of applications, including web development, scientific computing, data analysis, artificial intelligence, and more. This versatility makes it a good choice for building a wide range of applications, including custom software.[^1] Python has a large and active community of users and developers. This means that there is a wealth of resources available to help you learn the language and build your application, as well as a large pool of talented developers who can contribute to your project.[^2] Python has a simple, intuitive syntax that makes it easy for new users to learn and for experienced developers to quickly pick up. This makes it a good choice for building applications quickly and with fewer bugs, as well as for prototyping new ideas.[^3]
#### Why KivyMD?
One of the main advantages of using **KivyMD** is that it allows developers to build applications that can run on multiple platforms, including Android, iOS, and Windows. This makes it an ideal choice when targeting wide & international audiance like ISAK's journalism club application would. KivyMD is designed to be user-friendly and intuitive, making it easy for developers of all skill levels to get started with creating their own applications, but also is very suitable for co-developing due to small number of variables used allowing easy interpretation and allowing easy extensibility of the application. This can help to save time and effort, allowing developers to focus on creating their app's functionality and features. KivyMD offers a wide range of customization options that allow developers to tailor their apps to meet the specific needs of their users. From changing the look and feel of the interface to adding custom animations, the library offers a variety of options to make an app truly unique.[^4]
When compared to another UI creating software such as Flutter, KivyMD has more advantage on some components like more supportive online community, user-friendliness but most importantly KivyMD is better as it can work with python coding language while Flutter cannot which therefore is more suitable in this project.[^5]
#### Why SQL?
**SQL** is designed to handle large amounts of data efficiently, making it an ideal choice for applications that need to store and manage a large amount of information. This makes it an ideal choice for applications that need to scale as they grow, as SQL databases can be easily expanded to meet the needs of the application. SQL databases allow for the storage of structured data, which can be easily queried and manipulated. This makes it easier to find the information you need, and to perform complex data analysis tasks. SQL databases are highly reliable, and offer features such as transaction management and data integrity to ensure that the data stored in the database remains accurate and up-to-date. This makes SQL an ideal choice for applications that need to store critical data that must be maintained even in the event of a power outage or other failure.[^6]

# Criterion B: Solution Overview 
### Diagrams
System diagram, wireframe for the GUI, flow diagram, ER diagram for the database, and UML diagram for the OOP classes.

### Test Plan

|Test Number| Test Type  | Target|Procedure|Expected Outcome|
|-----------|-----------|--------|-----------|------------------|
                                                                                                                                                                                                                                                                                                                                                                                                                         
Table 1:
>Shows the test plan containing information about testing done for this application. There are 3 different types of tests presented in the test plan which are unit test(to test one part of the program), integration test(to test the cooperation of different parts) and code review(to check the quality of code). Table shows description, steps to follow, and expected output with a goal to help user understand the process better.
### Record of tasks

|    | Planned Action                                        | Planned Outcome                                                                            | Design Cycle   | Time Estimate | Target Completion | Criteria |
|----|-------------------------------------------------------|--------------------------------------------------------------------------------------------|----------------|---------------|-------------------|----------|
| 1  | First meeting with client                             | To understand client problem and requirements                                              | Planning       | 10 minutes    | 10.2.2023           | A        |
| 2  | Write down success criteria                           | To list down the first success criteria                                                    | Planning       | 20 minutes    | 12.2.2023           | A        |
| 3  | Write problem definition                              | Have problem definition which will identify who client is and the product that client want | Planning       | 20 minutes        | 12.2.2023           | A        |
| 4 | Research and write rationale for proposed solution    | Finish rationale for proposed solution                                                     | Planning       | 2 hours       | 20 March          | A        |
| 5  | Update success criteria                               | List more success criteria and prepare for presentation to client                          | Planning       | 15 minutes    | 13.2.2023         | A        |
| 6  | Starts working on login and registration system       | Finish login and registration system with database                                         | Development    | 2 hours        | 14.2.2023         | C        |
| 7 | Working on password encryption                        | Using sha256 to encrypt password and check password in login and registration              | Development    |15 minutes| 14.2.2023          | C        |
| 8| Meet with client to  present the success criteria     | Present success criteria to client to get the approval                                     | Planning       | 30 minutes    | 21.2.2023         | A        |
| 9  | Create wireframe diagram                              | Wireframe diagram is ready to present to client as the first MVP                           | Design         | 40 minutes   | 22.2.2023          | B        |
| 10  | Create system diagram                                 | System diagram is done with details written on it                                          | Design         |  45 minutes       | 22.2.2023         | B        |
| 11 | Create welcome screen following the wireframe diagram | Have welcome screen ready                                                                  | Development    | 2 hours       | 22/23.2.2023           | C        |
| 12 | Present the wireframe and application to the client   | Get client's feedback on the wireframe and application                                     | Planning       | 10 minutes    |???          | A        |
| 13 | Make ER diagram                                       | ER diagram is created for both tables                                                      | Planning       | 30 minutes    | ???      | B        |

Table 2:
> Record of Task-:shows the planning and working process throughout the project. This includes: programming, documentation, client's meetings, and other  process from the start of the project to the due date. Table contains order, description, Planned Outcome, Design Cycle, Time Estimate, Target Completion, Criteria


# Criterion C: Development
### Existing tools
This refers to the software tools used during the development of the solution, and structures such as for loops, and bash commands
### Sources
When code was researched in the web, proper citation is used to give credit to the original author.
### Tools used:
1. OOP paradigm
2. KivyMD Library
3. Relational databases
4. SQLite, ORM
5. Hashing
6. csv.file data storing and reading

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

### Citations
[^1]:"Python." Wikipedia, Wikimedia Foundation, 12 Feb. 2023, https://en.wikipedia.org/wiki/Python. ↩

[^2]:"Why Choose Python." Python.org, Python Software Foundation, 12 Feb. 2023, https://www.python.org/about/gettingstarted/. ↩

[^3]:"Python for Data Science Handbook." O'Reilly, O'Reilly Media, Inc., 12 Feb. 2023, https://www.oreilly.com/library/view/python-for-data/9781491912126/ ↩

[^4]:Gupta, Kaustubh. “What Is KivyMD | Creating Android Machine Learning Apps Using KivyMD.” Analytics Vidhya, 30 June 2021, www.analyticsvidhya.com/blog/2021/06/creating-android-ml-app-kivymd/#:~:text=KivyMD%20is%20built%20on%20the. Accessed 13 Feb. 2023.
[^5]:“Kivy vs Flutter | Learn the Key Differences between Kivy and Flutter.” EDUCBA,  July 2021, www.educba.com/kivy-vs-flutter/.
[^6]:"SQL." W3Schools, 13 Feb. 2023, https://www.w3schools.com/sql/ ↩
