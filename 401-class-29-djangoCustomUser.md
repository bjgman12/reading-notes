# Read 29

## best practices with django: custom user model

> custom user models provide more flexibility than the one built into django  so as a general rule always crete a custom user model

## Setup

- create and navigate to a dedicated dir called 'accounts'

- install django

- make a new project called 'config'

- make an app called 'accounts'

- start local web server

[reference site](https://learndjango.com/tutorials/django-custom-user-model)

## AbstractUser vs AbstractBaseUser

> use abstractUser to extend for now the base user is complicated

## Custom User Model

- update config/settings.py

- create CustomUser model
- create usercreation and userchange form
- update admin
