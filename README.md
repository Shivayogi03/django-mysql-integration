# Django MySQL Integration Project

This project demonstrates how to connect **MySQL** with a **Django** application and perform basic database operations using Django ORM.

It covers MySQL installation, Django configuration, and model creation.

---

## 🚀 Tech Stack

- **Backend:** Python, Django  
- **Database:** MySQL  
- **ORM:** Django ORM  
- **Tools:** MySQL Workbench, Git, GitHub  

---

## 📦 Features

- MySQL database connection with Django  
- Custom Django model (`Student`)  
- Database configuration using `settings.py`  
- Ready for migrations and CRUD operations  

---

## 🔧 MySQL Installation Steps

1. Download MySQL Installer  
   https://dev.mysql.com/downloads/installer/

2. Create an Oracle account (basic details)

3. Install with default settings, including:
   - MySQL Workbench  
   - MySQL Command Line Client  
   - MySQL Installer  

4. Open **MySQL Command Line Client**
   - Enter password when prompted

5. Create database:
   ```sql
   CREATE DATABASE developer;
Use database:

USE developer;
🐍 Python Packages Required
Install the following packages:

pip install pymysql
pip install mysql-connector-python
⚙️ Django MySQL Configuration
Add the following code at the top of settings.py:

import pymysql
pymysql.version_info = (1, 4, 13, "final", 0)
pymysql.install_as_MySQLdb()
Database Configuration
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'ur name',
        'USER': 'root',
        'PASSWORD': 'ur password',
        'HOST': 'localhost',
        'PORT': 3306,
    }
}
🧩 Sample Model
from django.db import models

class Student(models.Model):
    stname = models.CharField(max_length=100)
    stage = models.IntegerField()
▶️ Run the Project
python manage.py makemigrations
python manage.py migrate
python manage.py runserver

📌 Author
Shivayogi AM
Full Stack Developer (React | Django | MySQL)

📄 License
This project is for learning and demonstration purposes.
