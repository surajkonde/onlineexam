# Mcq-Web-App
A Python Django web application for taking MCQ (Multiple choice questions) tests.

### About
This application is developed in Python Django (a web framework for rapid development).
A user can sign in with any of the one roles "Moderator" or "Contestant". for more info see roles below.
This Web Application presents a set of random questions from database to user and calculates user score accordingly.

### Types of User-Roles (Roles)
 **Moderator:** A user who wants to take tests.
 **Contestant:** A user who gives tests.

### Features
1. **Contestant Exam State Tracking.**
2. **Contestant Login and SignUp.**
3. **Admin Panel.**
4. **Score Calculation Rules.**
5. **Moderator can take multiple tests.**
6. **Moderator can assign any number of test that he has designed to any number of some students.**

### Setup in production environment:
This application is currently in development phase and hence its not suitable to use it in production environment till then you can try this application on your local machine see intructions "**Run on local machine**"
Once its release of first version it can be used in production.

### Run on local machine - instructions
1. git clone https://github.com/sharadbhagwat/mcqWebApp.git
2. cd mcqWebApp
3. pip install -r requirements.txt 
If mysqlclient installatioon you can refer https://www.youtube.com/watch?v=6SnE0r7g2lE&t=133s 
4. Open mysql client, create database 'create database mcqDb'
5. Set correct mysql credentials in mcqWebApp/settings.py
6. python manage.py makemigrations questions
7. python manage.py migrate
8. Create admin user 'python manage.py createsuperuser'
9. python manage.py runserver 8080
10. Open this link -> 127.0.0.1:8080 and try this application.

### Todo
1. Import questions from excel sheet.
2. Ability to select questions for each test.
3. Ability to select students for each test
4. Ability to set marking scheme for each test.

### Contributing
1. You can setup this project locally by following intructions given above.
2. Then after fixing any issue yo can do a pull request.
3. In case of any issues please contact me => ankitwrk at gmail