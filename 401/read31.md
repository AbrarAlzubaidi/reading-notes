# Docker
With Docker it doesn’t matter if you are using a Mac, Windows, or Linux computer anymore. The entire development environment is isolated: programming language, software packages, databases, and more.
## containers
 Linux containers, also known as “containerization,” has become increasingly popular. For most applications, a virtual machine provides far more resources than are needed and a container is more than sufficient.

## Containers vs Virtual Environments
Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great.

But…virtual environments can only isolate Python packages. They still rely on a global, system-level installation of Python albeit they can refer to the proper version. So when we use Python 2.7 in a project, we’re pointing to an installation of Python 2.7 on the computer itself, not actually within the virtual environment.


------


# Django for APIs

A traditional Django website consists of a single project and one (or more) apps representing discrete functionality.

Django REST Framework is added just like any other third-party app
`pipenv install djangorestframework~=3.11.0` then add it to the INSTALLED_APPS config in your settings.py