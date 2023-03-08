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
**Python** Python versatility allows a great cross platform development[^1] which is a neccesity for the application I will be developing. Python has a large and active community of users and developers. [^2] Python has a simple, intuitive syntax that makes it easy for new developers to adapt to code and efficiently continue develpment[^3]. 
#### Why KivyMD?
One of the main advantages of using **KivyMD** is that it allows developers to build applications that can run on multiple platforms, including Android, iOS, and Windows. This makes it an ideal choice when targeting wide & international audiance like ISAK's journalism club application would.It is also very suitable for co-developing due to small number of variables used allowing easy interpretation and allowing easy extensibility of the application. This can help to save time and effort, allowing developers to focus on creating their app's functionality and features[^4].
When compared to another UI creating software such as Flutter, KivyMD has more advantage on some components like more supportive online community, user-friendliness but most importantly KivyMD is better as it can work with python coding language while Flutter cannot which therefore is more suitable in this project.[^5]
#### Why SQL?
**SQL** is designed to handle large amounts of data efficiently. This makes it an ideal choice for applications that needs to scale as they grow such as this one, as SQL databases can be easily expanded to meet the needs of the application. SQL databases allow for the storage of structured data, which can be easily queried and manipulated. This makes it easier to find the information you need, and to perform complex data analysis tasks. SQL databases are highly reliable ensuring the data stored in the database remains accurate and up-to-date.[^6]

# Criterion B: Solution Overview 
### Diagrams
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

![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/Blank%20diagram.png)
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
|33| Create First Flow diagram| Create a flow diagram for the try_register method which validates inputed data, and creates an account if all the criteria is met| 30 minutes| 7.3.2023| B|
|34| Create Second Flow diagram| Create a flow diagram for the read method which allows users to read desired articles by selecting them in the artilce table and choosing read article function| 30 minutes| 7.3.2023| B|
|35| Create Third Flow diagram | Create a flow diagram for the update method which updates article table, not displaying any deleted articles| 25 minutes | 7.3.2023| B|
|36|Add the code parts that show the development proccess that answers success criteria | Add adequate code snippets to criteria C develpment under all success criteria | 30 minutes| 8.3.2023|C |
|37|Add criteria C development proccess with the reasoning for methods and tools used in addition to connecting it to computational thinking. |Have this task done for criteria 1,2,3, and 4 |1 hour |8.3.2023 |C|
|38|Add criteria C development proccess with the reasoning for methods and tools used in addition to connecting it to computational thinking. |Have this task done for criteria 5,6,7 | 30 minutes |9.3.2023 |C|
Table 2:
> Record of Task-:shows the planning and working process throughout the project. This includes: programming, documentation, client's meetings, and other  process from the start of the project to the due date. Table contains order, description, Planned Outcome, Design Cycle, Time Estimate, Target Completion, Criteria


# Criterion C: Development
### Criteria number 1: The application contains account registration and login feature using username email and adequate password.
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/login_screen_proof.gif)
Fig. 8 Shows proof of the criteria 1, by showcasing functional login feature. It consists of two text fields (1) username/email and (2) password. If either the username or email match with the password enetered, user will be signed in to an adequate account containing these credentials.
#### LoginScreen Python code
```.py
class LoginScreen(MDScreen):
    current_user = None
    editor = False

    def try_login(self):
        print("User tries to login")
        uname = self.ids.uname.text
        passwd = self.ids.passwd.text
        query = f"SELECT * from users WHERE username= '{uname}' or email='{uname}' "
        db = database_worker("accounts.db")
        result = db.search(query = query)
        db.close()
        if len(result) == 1:
            print(result)
            id, email, hashed, uname = result[0]
            editor_validation = False
            editor_check = "@isakinsider.jp"
            if editor_check in email:
                editor_validation = True
            if check_password(user_password = passwd, hashed_password = hashed) and editor_validation == True:
                print("Login as an editor was successful")
                self.ids.passwd.text = ""
                EditorHomeScreen.user_name = uname
                self.parent.current = "EditorHomeScreen"
                LoginScreen.current_user = result[0]
                LoginScreen.editor = True
            else:
                if check_password(user_password = passwd, hashed_password = hashed):
                    print("Login as a reader was successful")
                    self.ids.passwd.text = ""
                    HomeScreen.user_name = uname
                    self.parent.current = "HomeScreen"

        else:
            print("login incorrect")

    def go_register(self):
        print("screen to register screen")
        self.parent.current = "SignupScreen"

```
Fig. 9 Shows the python code used for the Login part of the code. Here I created an algorithm that uses If statements as a method of checking if credentials are correct and link to any existing accounts. Following one of my client's requests regarding safe access to the application. Without a username and password that match one of the account in the user database, one can not acces and use the application. With this said the first request of criteria 1 stated by my client was fulfiled, and a functional login screen was created.
#### LoginScreen KivyMD code
```.kv
<LoginScreen>:
    size:500,500
    FitImage:
        source:"newspapers.png"
    MDCard:
        size_hint:0.6,.9
        elevation:2
        orientation:"vertical"
        pos_hint:{"center_x":.5,"center_y":0.5}
        padding:dp(50)
        MDBoxLayout:
            MDLabel:
                size_hint:0.15,1
            FitImage:
                source:"Untitled design.png"
                size_hint:.53,1
            MDLabel:
                size_hint:0.15,1
        MDTextField:
            id:uname
            hint_text:"Enter your username or email"
            icon_left:"email"

        MDTextField:
            id:passwd
            hint_text:"Enter your password"
            icon_left:"key"
            password:True

        MDBoxLayout:
            size_hint:1,.1
            MDRaisedButton:
                id:login
                text:"Login"
                on_press: root.try_login()
                size_hint:.3,1
                md_bg_color:"#161223"
            MDLabel:
                size_hint:.3,1
            MDRaisedButton:
                id:signup
                text:"Register"
                on_press: root.go_register()
                size_hint:.3,1
                md_bg_color:"#11dd99"
   ```
Fig. 10 Shows the KivyMD code used for the LoginScreen and all the functions in it. Using stylish background, appropriate to a digital newspapers article, comnbined with more stylistic features such as fitting button colors, I made sure that users will feel comfortable using this application and will enjoy the expirience to the fullest.
 
 
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/registerScreen_proof.gif)
 Fig.11 Shows proof of the criteria 1, by showcasing functional register feature. The screen consists of four text fields (1) username (2) email (3) password and (4) repeated password. If email does not follow the email validation policy, by missing "@" sign, an error in email textbox will appear. Similarly, if passwords do not match or the length of password does not follow the password policy, error will appear in these textboxes. If all the credentials are entered adequatly, an account will be created and user will be resurected to login screen to sign in to newly created account.
#### SignupScreen Python code
```.py
class SignupScreen(MDScreen):

    def try_register(self):
        uname = self.ids.uname.text
        email = self.ids.email.text
        passwd1 = self.ids.passwd.text
        passwd2 = self.ids.passwd_confirm.text
        if "@" not in email:
            self.ids.email.error = True

        if passwd1 != passwd2 or len(passwd1) < 6:
            self.ids.passwd.error = True
            self.ids.passwd_confirm.error = True

        if "@" in email and passwd1 == passwd2 and len(passwd1) >= 6:
            hash = encrypt_password(passwd1)
            db = database_worker("accounts.db")
            query = f"INSERT into users(email,password,username) values('{email}','{hash}','{uname}')"
            db.run_save(query)
            db.close()
            print("Registration completed")
            self.parent.current = "LoginScreen"

    def cancel(self):
        self.parent.current = "LoginScreen"
        self.ids.passwd.text = ""
        self.ids.passwd_confirm.text = ""
```
Fig. 12 Shows the python code used for the signup/registration feature of the application. I created an algorithm that uses If statements as a method of checking if data inserted into these text fields follow apropriate validation requirements. Even though I recognized a pattern and at first thought that last if is not needed and an else could be a better solution, I relaized that in order to meet my clients request of assuring that all the data must meet policies set for its type. The reason for the last if statement is to prevent someone incorrectly puting an email, but the correct passwords, but then since the else is tied to the if statement regarding password policy, account with an invalid email would be created, which would go against my clients request. But by using my algorithm this was not the case as the third if statement validates if both email and password policiy requirements were met. with this said by using computational thinking the second request of the success criteria 1 regarding signup feature was successfully met. 
#### SignupScreen KivyMD code
```.kv                
<SignupScreen>:
    size:500,500
    FitImage:
        source:"newspapers.png"
    MDCard:
        size_hint:0.8,.9
        elevation:2
        orientation:"vertical"
        pos_hint:{"center_x":.5,"center_y":0.5}
        padding:dp(50)

        FitImage:
            source:"Re.png"

        MDTextField:
            id:uname
            hint_text:"Enter your username"
            icon_left:"account"

        MDTextField:
            id:email
            hint_text:"Enter your email"
            icon_left:"email"
            helper_text_mode:"on_error"
            helper_text:"Email is not valid"

        MDTextField:
            id:passwd
            hint_text:"Enter your password"
            icon_left:"key"
            password:True

        MDTextField:
            id:passwd_confirm
            hint_text:"Enter your password (min. 6 characters, containing number and a letter)"
            icon_left:"key"
            password:True
            helper_text_mode:"on_error"
            helper_text:"Password does not match or fails password policy"
        MDLabel:
            size_hint:1,.05
        MDBoxLayout:
            size_hint:1,.2

            MDRaisedButton:
                id:signup
                text:"Submit"
                on_press: root.try_register()
                size_hint:.3,1
                md_bg_color:"#161223"

            MDLabel:
                size_hint:.3,1

            MDRaisedButton:
                id:cancel
                text:"cancel"
                on_press: root.cancel()
                size_hint:.3,1
                md_bg_color:"#11dd99"
```
Fig.13 shows KivyMD code used for the user interface of the SignupScreen. It consists of 4 textboxes mentioned in Fig 11, aswell as sumbition button that creates an account if all the data is correctly entered, showcased and explained in Fig.11 and cancel button that returns user to the login screen.
### Criteria number 2: Differentiates normal readers and editor accounts which would have an option to add articles if their account is authorized as a journalism club member.Viewers can only read. Editors have a feature of adding articles.
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/editor_reader_proof.gif)
Fig. 14 showcases the difference between account that is registered as an editor (following the specific email structure that editors have) and an account registered as a normal user.
#### Python code used to differenciate editors and normal readers.
```.py
 editor_validation = False
            editor_check = "@isakinsider.jp"
            if editor_check in email:
                editor_validation = True
            if check_password(user_password = passwd, hashed_password = hashed) and editor_validation == True:
                print("Login as an editor was successful")
                self.ids.passwd.text = ""
                EditorHomeScreen.user_name = uname
                self.parent.current = "EditorHomeScreen"
                LoginScreen.current_user = result[0]
                LoginScreen.editor = True
            else:
                if check_password(user_password = passwd, hashed_password = hashed):
                    print("Login as a reader was successful")
                    self.ids.passwd.text = ""
                    HomeScreen.user_name = uname
                    self.parent.current = "HomeScreen"
```
Fig. 15 Shows the code part that checks credentials and if the account created will be an editor account or not. It checks if the "@isakinsider.jp" is in the user's email. If it is, the user will be given author credentials and will have access do editor home screen. If not, account will be a reader, gaining access to reader home screen. In order to solve this problem of differenciating users based on their credentials. I used decomposition and got rid of the unnecesary validations of passwords, until I find the solution to check if user is editor based on their email. I got this idea by recognizing a pattern of validating data based on the content of the string inputed. All this is showcased in Fig. 14. With this said, criteria 2 was successfully answered.

### Criteria number 3: Application will have a feature to add an article and safely store it.

![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/add_article_proof.gif)
Fig. 16 Shows the proccess of adding an article, and showcases how it was stored and displayed in article table.
#### Python code for the method that adds an article and stores it
```.py
    def add_article(self):
        author = self.ids.author.text
        title = self.ids.title.text
        content = self.ids.content.text
        image = self.ids.image.text
        if title and content:
            db = database_worker("accounts.db")
            query = f"INSERT into articles(author,title,content,image) values('{author}','{title}','{content}','{image}')"
            db.run_save(query)
            db.close()
            self.ids.title.text = ''
            self.ids.content.text = ''
            self.parent.current = "EditorHomeScreen"
```
Fig.17 Shows method used to add articles by gathering data inputed in the author,title, content, image link  in the text fields. It then uses a query that inserts these values into the database containing articles, which will later be accesed to show data in it in the form of an article table.
### Criteria number 4: Option to see image of the article, allowing full expirience of digital newspapers.
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/Image_view_proof.gif)
Fig. 18 shows proof of succesful image showcasing, using the image link provided when article was being created.
```.py
 def photo(self):
        ArticleImageScreen.url = f"{self.image_link}"
        print(self.image_link)
        print(ArticleImageScreen.url)
        self.parent.current = "ArticleImageScreen"


class ArticleImageScreen(MDScreen):
    url = None

    def on_pre_enter(self, *args):
        print(self.url)
        if self.url:
            self.ids.article_image.source = self.url
```
Fig. 19 Shows the python method photo that takes the image url of the article which was stored in the article database, and then using that url acceses the image which has the matching url and is inside of the same file as the projects main code. I recognized the problem of the picture not being visible enough when presented in the popup format, so I created a method that serves as a bridge between article screen and a screen that will fully show desired picture. This way I answered my client's additional request for the picture to be in the largest format possible, making it very visible, just like it would be in the physical newspapers. Criteria 4 was answered successfully this way, assuring much needed full digital newspapers expirience. 
### Criteria number 5: Option to view past articles containing the author, title, and its content.
```.py
 self.dialog = MDDialog(
                text = f"Author: [size=22sp][color=333333]{author}[/color][/size]  \n \n \n "
                       f"[size=40sp][color=555555]{title}[/color][/size]\n \n \n"
                       f"[size=15sp][color=666666]{content}[/color][/size]",
                content_cls = MDBoxLayout(padding = dp(20)),
                size_hint = (0.8, None),
                height = dp(500)
            )
            self.dialog.open()
```
Fig. 20 Shows a code that creates popup contianing the articles that were selected for reading previously. I had a request to make selected articles both visible and estetic, but also easy to close and move to the next article. So by using computational thinking, more specificly decomposition, I tackled first problem by choosing specific font style and the spacing, similar to ones used in online newspapers. Second problem was solved by using MDDialog as a tool to create popup screens, which allowed quick transition to the article user wants to read next. Finally I combined to decomped smaller solved problems into one final solution, and with that I have succesfully fulfilled client's criteria 5.
By implementing 
### Criteria number 6: Option to select multiple articles and read them one after another, just like in digital newspapers.
```.py
 for r in rows_checked:
            id = int(r[0])
            query1 = f"Select author,title,content,image from articles where id={id}"
            result = db.search(query1)
            author, title, content, image_link = result[0]
            self.image_link = image_link


            # Create the dialog content
            self.dialog = MDDialog(
                text = f"Author: [size=22sp][color=333333]{author}[/color][/size]  \n \n \n "
                       f"[size=40sp][color=555555]{title}[/color][/size]\n \n \n"
                       f"[size=15sp][color=666666]{content}[/color][/size]",
                content_cls = MDBoxLayout(padding = dp(20)),
                size_hint = (0.8, None),
                height = dp(500)
            )
            self.dialog.open()
```
Fig.21 Shows the algorithm I created in order to answer the request of my client regarding creation of the way that allows users to read all checked articles one after another, without the need to check in between readings, but by simply clicking outside of the popup to move to the next article. I used pattern recognition to realize that this could be done through a for loop. Implementing computational thinking to this problem not only solved the issue but gave a rather practical method of moving to the next article. With this, by adapting the once normal read function of a single article, I transformed it into practical multi article feature. That feature was what my client asked for and what fulfilled criteria number 6.
### Criteria number 7: Option to delete articles created by the user logged in.
![](https://github.com/AleksandarDzudzevic/Project_Unit_3/blob/main/delete_article_proof.gif)
```.py
 def delete(self):
        rows_checked = self.data_table.get_row_checks()
        print("riw;", rows_checked)
        db = database_worker("accounts.db")
        for r in rows_checked:
            id = r[0]
            author = r[1]
            # Check if the article was created by the current user
            if author == LoginScreen.current_user[3]:
                query = f"DELETE FROM articles WHERE id={id}"
                db.run_save(query)
                self.data = None
                confirm_dialog = MDDialog(
                    title = "Article deleted!",
                    text = "The selected articles have been deleted.",
                    buttons = [
                        MDFlatButton(
                            text = "OK",
                            on_release = lambda *args: confirm_dialog.dismiss()
                        )
                    ]
                )
                confirm_dialog.open()

                self.parent.current = "EditorHomeScreen"
        db.close()
        self.update()
```
Fig.22 shows the method used when choosing to delete articles that were written by the user. The method uses an algorithm. which goes through for iteration until it went through all selected rows. Using an if statement in checks if those articles were writtenn by the editor currently signed in. This was done because in order to avoid any potential conflict between isak insider edtiors, no editor can delete articles written by other editors. This way option to delete any irrelevant or outdated articles is available, which was my client's final success criteria.
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
