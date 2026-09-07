# Django Introduction

## 1. Create a virtual environment

A Python virtual environment is an isolated folder containing a specific Python interpreter and its own dedicated set of libraries/packages

### Prerequisite

- Python 3+
- Visual Studio Code

### Steps

- Go to your computer terminal
- Navigate to where you want your virtual environment folder to be
- Run the following line of command to create a virtual environment:

```bash
python3 -m venv blog_venv # 'blog_venv' is the name of my virtual environment. Any meaningful name can be used.
```

- Activate your virtual environment. Type out the following command:

_*Windows*_

```powershell
.\blog_venv\Scripts\activate

# if you get error such as:
# File C:\path\to\your\project\Scripts\activate.ps1 cannot be loaded because running scripts is disabled on this system. For more information, see about_Execution_Policies at https:/://microsoft.com. Run the following command:
Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser

# Run .\blog\Scripts\activate again
```

_*Mac*_

```bash
source blog_venv/bin/activate
```

- Confirm if the virtual environment is activated by checking whether **(blog_venv)** begins the immediate line or not. On Window, (blog_venv) will turn green. You are now set!

## 2. Install Django

Django is a python package which gives us the ability to write Django web application. This package is online therefore, we have to connect our computer to the internet to download it.

- Run the following command in your terminal to install

```bash
pip3 install django
```

### 3. Create a project

- After you have successfully installed Django package, you can now proceed to create a Django project. Run the following command to create the project

```bash
django-admin startproject django_blog # 'django_blog' is the name of my project. It can be anything apart from django_blog.
```

- The command above will create a new folder/directory named **'django_blog'**. To check if you have successfully set Django up, navigate to the project folder **'django_blog'**, try to run the server with the following command:

```bash
python3 manage.py runserver
```

- The command you ran above will start the application server. Read the output until you find "<http://127.0.0.1:8000>". Copy the address and paste it in your browser's search bar and press 'Enter'. You should see a webpage the contains a rocket picture with the message "The install worked successfully! Congratulations!"
