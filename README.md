Install Django

- pipenv install django

Enter virtual environment

- pipenv shell

Create a README for project description

- touch README.md

Create a new project at the folder root

- django-admin startproject main .

Test the server

- python manage.py runserver

Create App

- django-admin startapp first_app

* Remember to add app to settings.py file in main project

Install Django REST Framework

- pipenv install djangorestframework

* Remember to add rest_framework to settings.py file in main project

Install Prostgres adapter for python -> psycopg2

- pipenv install psycopg2

* Remember to configure Database engine and name in settings.py file in main project
* Configure a local db for your project so that you have a local database to play with
  - 'ENGINE': 'django.db.backends.postgresql_psycopg2'
  - 'NAME': 'your_db_name'

Initial Migrate -> Migrate to your local db

- python manage.py migrate

Create admin user

- python manage.py createsuperuser

* I usually use name: admin, password: pw

Initiate git

- git init
