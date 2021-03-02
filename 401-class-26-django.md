## Django Intro

- create a new django project with the command ` dhango-admin startproject mysite`

the command above will create a base file structure to start with

- **manage.py** is a command line utility that lets you interact with your django project

- **settings.py** configuration for the django project

- **urls.py**  table of contents of the django powered site

- **asgi.py** entry point for asgi compatable web servers
- **wsgi.py** entry point for wsgi compatable web servers

### development server

- entering **python manage.py runserver** will start up the development server use for development not production

- the port may be changed by specifying the port number after the command

- the ip can be changed as well passing it along with teh port seperated by a :

### Creating the polls app

- go inside the directory that manage .py is stored

- run command python3 manafe.py startapp polls

`from django.shortcuts import render
from django.http import HttpResponse


`def index(req):
    return HttpResponse('Hello,World. You\'re at the polls index')
    
`

- above is a simpe example on how to create a view

- after that you go to the urls.py inside of mysite dir and add the path to the file

### Django behind the scenes

 > our namesake is a python based web framework used by millions of devs
 - open source
 