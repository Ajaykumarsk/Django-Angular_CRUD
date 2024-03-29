﻿# Django-Angular_CRUD
Project Setup

#To check Python Version
->py --version

#To create Virtual Environment 
->py -m venv venv

#To use Virtual Environment 
->venv/Scripts/activate

#To Install Djangos 
->py -m pip install Django 

->py -m pip install djangorestframework

->py -m pip install django-cors-headers

->py -m pip install psycopg2


#Create New Database 
In postgresql create a database 


#To Start Project
->django-admin startproject main .

->django-admin startapp users

#open settings.py

Add below 

ALLOWED_HOSTS = ['*'] # To allow all hosts


#Application definition
INSTALLED_APPS = [
    'django.contrib.admin',
    'django.contrib.auth',
    'django.contrib.contenttypes',
    'django.contrib.sessions',
    'django.contrib.messages',
    'django.contrib.staticfiles',
    'rest_framework',
    'corsheaders',
    'users'
]


#Rest framework Configuration
REST_FRAMEWORK={
    'DEFAULT_PERMISSION_CLASSES':[
        'rest_framework.permissions.AllowAny'
    ]
}



#Postgresql configration 
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'djangodb',
        'USER':'postgres',
        'HOST':'localhost',
        'PORT':'5432',
        'PASSWORD':'admin'
    }
}



#CORS HEADERS TO ALLOW
CORS_ORIGIN_ALLOW_ALL = True
CORS_ALLOW_CREDENTIALS = True



#Install Node.js

->npm install -g @angular/cli

->ng version 

->ng new frontend

#Add Angular Extensions (lang and snippets)

->npm start

->npm install bootstrap

 #add Bootstrap in angular.json

 "styles": [
              "src/styles.css",
              "./node_modules/bootstrap/dist/css/bootstrap.min.css"
            ],


 "scripts": [
              "./node_modules/bootstrap/dist/js/boootstrap.min.js"
            ],

# OUTPUT

![Screenshot 2024-02-24 181908](https://github.com/Ajaykumarsk/Django-Angular_CRUD/assets/115660974/8421cdcb-2a73-448c-8980-994cc8dec67e)
![Screenshot 2024-02-24 181103](https://github.com/Ajaykumarsk/Django-Angular_CRUD/assets/115660974/56d0a24d-a934-4ae0-bb1a-95cc91ab884d)
![Screenshot 2024-02-24 181046](https://github.com/Ajaykumarsk/Django-Angular_CRUD/assets/115660974/21dc6de2-4525-4dd5-b4be-41b45976c30e)
![Screenshot 2024-02-24 181013](https://github.com/Ajaykumarsk/Django-Angular_CRUD/assets/115660974/63187aad-94e7-444a-8682-05768ac80009)
