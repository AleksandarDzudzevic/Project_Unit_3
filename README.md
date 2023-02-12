# Project Unit 3: Journalism club application
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/project3.gif)

# Criterion A: Planning 
### Definition of the Problem
UWC ISAK Japan is a school that always strives to be more environmentally friendly, but due to high demand for copies of ISAK INSIDER articles every week, a lot of paper is being used to print them. This especially bothered Jonathan Wang Ye, who is considered by many, number one environmentalist at ISAK, probably even Japan. He is in urgent need for an UWC ISAK journalism club application which would store articles that ISAK INSIDER publishes every week in addition to storing articles from past weeks. He also demands the highest level of security due to the fact that this would be an official school app, so all the passwords must be encrypted, protecting data of app's users. Other than being more green, additional benefit of this app would be that it would nake articles available anywhere in the world, allowing fans and alumni of the school outside ISAK to enjoy it.
This way everyone would be able to enjoy ISAK INSIDER without hurting the environment by wasting paper in the process.

Who is the client?
Why is the product being developed

### Success criteria
#### 1. Option to create an account with a signup and login feature that validates password and username not allowing the same username twice.
#### 2. Secure password storing in the database, using hashing encryption
#### 3. Allow different accounts to access the same database that stores articles.
#### 4.Differentiates normal readers and editor accounts which would have an option to add articles if their account is authorized as a journalism club member.
#### 5. Option to view articles from past weeks by choosing the date.
#### 6. Option to choose which type of article you want to read (sport, culture, Karuizawa community, global issues…)



### Design statement
---
### Rationale for proposed solution
Considering the client's requests, I will develop an easy-to-use centralized application for managing UWC ISAK's journalism club articles. It will be designed and developed using Kivymd, Python, and SQlite. 
#### Why Python?
**Python** is a versatile language and can be used for a wide range of applications, including web development, scientific computing, data analysis, artificial intelligence, and more. This versatility makes it a good choice for building a wide range of applications, including custom software.1 Python has a large and active community of users and developers. This means that there is a wealth of resources available to help you learn the language and build your application, as well as a large pool of talented developers who can contribute to your project.2 Python has a simple, intuitive syntax that makes it easy for new users to learn and for experienced developers to quickly pick up. This makes it a good choice for building applications quickly and with fewer bugs, as well as for prototyping new ideas.3
#### Why KivyMD?
One of the main advantages of using **KivyMD** is that it allows developers to build applications that can run on multiple platforms, including Android, iOS, and Windows. This makes it an ideal choice for those who want to reach a wide audience with their apps. KivyMD is designed to be user-friendly and intuitive, making it easy for developers of all skill levels to get started with creating their own applications. This can help to save time and effort, allowing developers to focus on creating their app's functionality and features. KivyMD offers a wide range of customization options that allow developers to tailor their apps to meet the specific needs of their users. From changing the look and feel of the interface to adding custom animations, the library offers a variety of options to make an app truly unique.4
#### Why SQL?
**SQL** is designed to handle large amounts of data efficiently, making it an ideal choice for applications that need to store and manage a large amount of information. This makes it an ideal choice for applications that need to scale as they grow, as SQL databases can be easily expanded to meet the needs of the application. SQL databases allow for the storage of structured data, which can be easily queried and manipulated. This makes it easier to find the information you need, and to perform complex data analysis tasks. SQL databases are highly reliable, and offer features such as transaction management and data integrity to ensure that the data stored in the database remains accurate and up-to-date. This makes SQL an ideal choice for applications that need to store critical data that must be maintained even in the event of a power outage or other failure.5

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
"Python." Wikipedia, Wikimedia Foundation, 10 Feb. 2023, https://en.wikipedia.org/wiki/Python. ↩

"Why Choose Python." Python.org, Python Software Foundation, 10 Feb. 2023, https://www.python.org/about/gettingstarted/. ↩

"Python for Data Science Handbook." O'Reilly, O'Reilly Media, Inc., 10 Feb. 2023, https://www.oreilly.com/library/view/python-for-data/9781491912126/ ↩

"KivyMD: Material Design Components for Kivy." Github, 10 Feb. 2023, https://github.com/kivymd/KivyMD. ↩

"SQL." W3Schools, 10 Feb. 2023, https://www.w3schools.com/sql/ ↩
