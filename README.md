# Py Task List
#### Video Demo:  <https://youtu.be/12rKUQwUXfg>
## Description:

### What will your software do?
My software is a Task List Application developed using Django and Python, designed to help users manage their daily tasks efficiently. The application allows users to sign up and log in with a username and password. Once logged in, users can add, view, edit, and delete tasks, ensuring they stay organized and on top of their to-do lists.

### What features will it have?
User Registration and Authentication:<br>
Users can create an account by registering with a unique username and password.<br>
Users can log in and log out securely.

### Task Management:
Add new tasks: Users can input their tasks in a text field and submit them.<br>
View tasks: A list of tasks is displayed on the main page after login.<br>
Edit tasks: Users can click on a task to be redirected to an edit page where they can modify the task details.<br>
Delete tasks: Users can remove tasks from the list.

### User Interface:
Display the username in the header after login.<br>
A welcoming prompt "Something to be done?" with an input field labeled "What are today's tasks?" for adding tasks.<br>
Dynamic updates to the task list upon adding, editing, or deleting tasks.<br>

### How will it be executed?
The application is deployed on Railway, leveraging PostgreSQL as the database backend. Users can access the application through a web browser, where they can interact with the user-friendly interface to manage their tasks.

### What new skills will you need to acquire? What topics will you need to research?
To enhance and possibly expand this project, I will need to acquire and research the following skills and topics:

Advanced Django Features: To implement more complex functionalities, such as task prioritization or deadline reminders.<br>
Frontend Development: Improve the user interface and user experience using HTML, CSS, and JavaScript frameworks like React or Vue.js.<br>
Deployment and Scaling: Learn more about deploying Django applications at scale, managing server resources, and ensuring the application can handle a growing number of users.<br>
Security Best Practices: Implementing advanced security features to protect user data and prevent vulnerabilities.<br>
API Integration: Exploring how to create and consume APIs to integrate with other services or mobile applications.<br>

### If working with one or two classmates, who will do what?
While this project is currently a solo endeavor, if I were to collaborate with classmates, the responsibilities could be divided as follows:

Backend Development: One person focuses on the core Django backend, handling the database models, views, and authentication logic.<br>
Frontend Development: Another person could work on the user interface, ensuring the application is visually appealing and user-friendly.<br>
Deployment and DevOps: A third team member could manage the deployment process, set up continuous integration/continuous deployment (CI/CD) pipelines, and ensure the application runs smoothly on the Railway platform.

### Good, Better, and Best Outcomes
Good Outcome:
Successfully deploy the application with all the core features working as intended (user registration, login, adding, editing, and deleting tasks).
Ensure basic security measures are in place.

Better Outcome:
Enhance the user interface with improved styling and responsive design.
Implement additional features such as task categorization, due dates, and notifications.
Optimize the application for better performance and user experience.

### Best Outcome:

Integrate advanced features like real-time updates using WebSockets or similar technology.<br>
Develop a mobile version of the application or a companion mobile app.<br>
Implement comprehensive security measures, including two-factor authentication and data encryption.<br>
Achieve seamless scalability to support a large number of concurrent users without performance degradation.<br>
By achieving these outcomes, the Task List Application will not only serve its primary function effectively but also provide a robust and enjoyable user experience.<br>

## Project Structure and File Descriptions

### Root Directory
• staticfiles: This directory is typically used to collect static files from different apps in the Django project during deployment. It helps in serving these files efficiently.<br>
• todo: This is the main application folder containing all the app-specific files and subdirectories.<br>
• .gitattributes: This file is used to manage how Git treats certain files, ensuring consistent behavior across different environments, particularly with line endings.<br>
• Procfile: A file used by Heroku and similar platforms to specify the commands that are run by the app’s dynos. Typically, it will contain instructions to run the Django web server.<br>
• db.sqlite3: The SQLite database file that stores all the data for the application. This is used during development; in production, you use PostgreSQL.<br>
• manage.py: A command-line utility that allows you to interact with your Django project. It includes commands for running the development server, applying migrations, creating users, etc.<br>
• requirements.txt: This file lists all the Python packages required to run your project. It is used to install dependencies in a consistent environment.<br>
• runtime.txt: Specifies the Python version to be used, ensuring compatibility and consistency across different deployment environments.<br>

### todo Directory
• static: Contains static files specific to the todo app.<br>
• migrations: Stores migration files, which are used by Django to apply changes to the database schema.<br>
• pycache: A directory containing compiled Python bytecode files to speed up execution.<br>
• templates: Contains HTML template files for the todo app.<br>

### todo Static Directory
• css/index.css: This file contains styles specific to the task list, such as the appearance of text boxes and submit buttons, their positions, and sizes.<br>
• css/style.css: Defines the general design of the page, including background colors, text box colors, and other overarching styling elements.<br>
• js/todo.js: Contains JavaScript code for the todo app. It includes a function to change the background color of an HTML element to green when called.<br>

### todo Templates Directory
• edit_todo.html: The template for the page where users can edit existing tasks.<br>
• login.html: The template for the login page where users enter their credentials to log in.<br>
• signup.html: The template for the signup page where new users can create an account.<br>
• todo.html: The main page template where users can add new tasks and view their task list.<br>


### todo Python Files
• .env: Contains environment variables, such as secret keys and database configurations, that are loaded into the Django settings.<br>
• init.py: An initialization file for the todo app, making it a Python package.<br>
• admin.py: Registers the models with the Django admin site, allowing for administrative operations on the models.<br>
• asgi.py: Configures the ASGI application for asynchronous support.<br>
• models.py: Contains the database models for the todo app, defining the structure of the data.<br>
• settings.py: The main settings file for the Django project, including configuration options for installed apps, middleware, templates, databases, and more.<br>
• urls.py: Defines the URL patterns for the todo app, mapping URLs to their corresponding views.<br>
• views.py: Contains the view functions or classes that handle HTTP requests and return responses.<br>
• wsgi.py: Configures the WSGI application for serving the project in a production environment.<br>

## Design Justifications
Color Scheme: The primary color of the application is purple. This choice was made because purple is often associated with creativity, calmness, and productivity, making it an ideal color for a task management application. It helps create a visually appealing and engaging user experience.<br>
File Structure: The organization of files and directories follows the Django best practices, separating static files, templates, and Python modules for better maintainability and clarity.<br>
Use of SQLite: SQLite is used during development for simplicity and ease of setup. PostgreSQL is used in production for robustness and scalability.<br>
Static Files Management: By separating CSS and JavaScript into distinct files, the project ensures a clean and modular approach to frontend design, allowing for easier updates and maintenance.

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/django/django-plain.svg" height="40" alt="django logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="40" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" height="40" alt="postgresql logo"  />
</div>

<div style="display: inline_block" align="left">
    <img align="center" alt="DJANGO"src="https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white"/>
    <img align="center" alt="Spring"src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
    <img align="center" alt="Spring"src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white"/>
</div><br>

<div style="display: flex"><br/>
<img align="center"  alt="todo"src="https://github.com/muriloalvesx/ListaDeTarefas/assets/153781890/e5003910-6149-428c-acbc-f20fa8854faf" width="550px"/>
<img align="center"  alt="db"src="https://github.com/muriloalvesx/ListaDeTarefas/assets/153781890/2face8b3-0ca6-474c-867c-e9a2eb80284d" width="350px"/>
