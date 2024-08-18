# Project Title : CUSTOMER RELATIONSHIP MANAGEMENT 

## Description

This project is a web application built using Django, designed to manage user **registration, login, and logout functionalities**. It includes user authentication and authorization, allowing authorized users to to perform various data operations, including [inserting, viewing, deleting, and updating records in the database]. This project is built using Django, Python, HTML, and Bootstrap It includes user authentication and authorization, allowing authorized users to perform CRUD (Create, Read, Update, Delete) operations on the [mention the core data or functionality]. 

## Features

- User Registration and Login/Logout
- User Authentication and Authorization
- CRUD Operations 
- Responsive Design using Bootstrap
- Notifiaction System
- SQL Database Integration

## Installation

### Prerequisites

- Python 3.12 
- Django 3.x or later
- pip (Python package installer)

# Project Setup Instructions

## 1. Clone the Repository

```bash
git clone https://github.com/yourusername/your-repository.git
```

## 2. Navigate to the Project Directory
```
cd your-repository
```
## 3. Create and Activate a Virtual Environment
```
python -m venv virt
source virt/Scripts/activate   
```

## 4. Install the Required Dependencies
```
pip install django
pip install mysql
pip install mysql-connector-python
pip install -r requirements.txt
```
## 5. Apply Migrations to Set Up the Database
```
django-admin startproject dcrm
python manage.py startapp website
```

## 6. Database setup
Add the following configuration to your `settings.py` file for the MySQL database:

```
DATABASES = {
    "default": {
        "ENGINE": "django.db.backends.mysql",
        "NAME": "elderco",
        "USER": "name_of_your_root_user",
        "PASSWORD": "your_mymysql_password",
        "HOST": "localhost",
        "PORT": "3306",
    }
}
```

```
touch mydb.py
```

## 7. Create a Superuser Account
```
python manage.py migrate
winpty python manage.py createsuperuser  
```
## 8. Run the Development Server
```
python manage.py runserver
```

## 9. Access the Application in Your Web Browser

http://127.0.0.1:8000



## Project Structure

```
Django-CRM
│
├── dcrm
│   ├── __pycache__
│   ├── __init__.py
│   ├── controllers/
│   ├── setting.py
│   └── urls.py
│   └── wsgi.py
│
├── website
│   ├── migrations
|       ├── __pycache__
|       ├── 0001_initail.py
|       ├── __init__.py
|   ├── template
|       ├── add_record.html
|       ├── base.html
|       ├── footer.html
|       ├── home.html
|       ├── navbar.html
|       ├── record.html
|       ├── register.html
|       ├── update_record.html
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── models.py
│   ├── tests.py
│   └── urls.py
│   └── views.py

│
├── manage.py
|
└── mydb.py

```
