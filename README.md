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
 3. There is a secondary account access option, allowing user to login by answering safety question they inputed when creating a password.
 4. Differentiates normal readers and editor accounts which would have an option to add articles if their account is authorized as a journalism club member. Viewers can only read. Editors have a feature of adding articles.
 5. Option to view past articles containing the author, title and its content.
 6. Option to choose the edition of newspapers the user wants to view, with articles grouped by the dates.



### Design statement???

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
### Test Plan
This is a list of step, table, or flow chart specifying the process for testing the solution with the inputs and expected outputs.

### Diagrams
System diagram, wireframe for the GUI, flow diagram, ER diagram for the database, and UML diagram for the OOP classes.

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
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/Project_3_appendex.png)

### Citations
[^1]:"Python." Wikipedia, Wikimedia Foundation, 12 Feb. 2023, https://en.wikipedia.org/wiki/Python. ↩

[^2]:"Why Choose Python." Python.org, Python Software Foundation, 12 Feb. 2023, https://www.python.org/about/gettingstarted/. ↩

[^3]:"Python for Data Science Handbook." O'Reilly, O'Reilly Media, Inc., 12 Feb. 2023, https://www.oreilly.com/library/view/python-for-data/9781491912126/ ↩

[^4]:Gupta, Kaustubh. “What Is KivyMD | Creating Android Machine Learning Apps Using KivyMD.” Analytics Vidhya, 30 June 2021, www.analyticsvidhya.com/blog/2021/06/creating-android-ml-app-kivymd/#:~:text=KivyMD%20is%20built%20on%20the. Accessed 13 Feb. 2023.
[^5]:“Kivy vs Flutter | Learn the Key Differences between Kivy and Flutter.” EDUCBA,  July 2021, www.educba.com/kivy-vs-flutter/.
[^6]:"SQL." W3Schools, 13 Feb. 2023, https://www.w3schools.com/sql/ ↩
