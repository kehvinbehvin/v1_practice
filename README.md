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

Enabling cors

- pipenv install django-cors-headers

* Remember to add 'corsheaders' to settings.py at installed apps
* Remember to add 'corsheaders.middleware.CorsMiddleware' to settings.py at middleware...
* ...above 'commonMiddleWare'

Initiate git and commit

- git init

Install gunicorn

- pipenv install gunicorn

Create Procfile in root of project

- touch Procfile

* echo "web: gunicorn myproject.wsgi" >> Procfile

Install django_heroku

- pipenv install django_heroku

* Import in settings.py
* configurations inside settings.py django_heroku.settings(locals()) -> place at the bottom
