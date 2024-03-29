# BLOGGER
A blog app for sharing your ideas with the world. Comes with a full featured blog app, custom user model, login/logout/signup, social authentication via django-allauth, and more.

## Features

- Django 3.1, Django REST Framework 3.12, and Python 3.8
- Custom user model
- Token-based auth
- Signup/login/logout
- [django-allauth](https://github.com/pennersr/django-allauth) for social auth
- [Pipenv](https://github.com/pypa/pipenv) for virtualenvs

## First-time setup

1.  Make sure Python 3.7x and Pipenv are already installed. [See here for help](https://djangoforbeginners.com/initial-setup/).
2.  Clone the repo and configure the virtual environment:

```
$ git clone https://github.com/AlbertHope7/blog_api_mastered.git
$ cd blog_api_mastered
$ pipenv install
$ pipenv shell
```

3.  Set up the initial migration for our custom user models in users and build the database.

```
(drfx) $ python manage.py makemigrations users
(drfx) $ python manage.py migrate
(drfx) $ python manage.py createsuperuser
(drfx) $ python manage.py runserver
```

4.  Endpoints

Login with your superuser account. Then navigate to all users. Logout. Sign up for a new account and repeat the login, users, logout flow.

- login - http://127.0.0.1:8000/api/v1/rest-auth/login/
- all users - http://127.0.0.1:8000/api/v1/users
- logout - http://127.0.0.1:8000/api/v1/rest-auth/logout/
- signup - http://127.0.0.1:8000/api/v1/rest-auth/registration/

---
