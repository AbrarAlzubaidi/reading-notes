# Django Best Practices: Custom User Model
 **notes**

 - Django ships with a built-in User model for authentication.

 - the official Django documentation highly recommends using a custom user model instead. This provides far more flexibility down the line.

 - create and navigate into a dedicated directory start the local web server run: 


        (accounts) $ django-admin.py startproject config .
        (accounts) $ python manage.py startapp accounts
        (accounts) $ python manage.py runserver


## AbstractUser vs AbstractBaseUser

- AbstractBaseUser requires much, much more work.
- AbstractUser which actually subclasses AbstractBaseUser but provides more default configuration.

## Superuser

to create a super user in django: 
`python manage.py createsuperuser`


-----------


#  DjangoX
an open-source Django starter framework that includes a custom user model, email/password by default instead of username/email/password, social authentication, and more.


## Features
1. Django 3.1 & Python 3.8
2. Install via Pip, Pipenv, or Docker
3. User log in/out, sign up, password reset via 4. django-allauth
4. Static files configured with Whitenoise
5. Styling with Bootstrap v4
6. Debugging with django-debug-toolbar
7. DRY forms with django-crispy-forms
