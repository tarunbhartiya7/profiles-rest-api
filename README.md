# Demo project using Django framework

In this project we are going to create REST APIs.
This project is part of https://www.udemy.com/course/django-python/learn

# Mark down cheatsheet
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

# SSH keys
check for any existing SSH keys in your system -> ls ~/.ssh

create a new SSH key - refer https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

ssh-keygen -t rsa -b 4096 -C "tarunbhartiya7@gmail.com"

# create a vagrant file
vagrant init ubuntu/bionic64

# configure the vagrant file and run
vagrant up
vagrant ssh
to exit from the machine - exit

# Vagrant commands
vagrant status

To stop this VM, you can run `vagrant halt` to
shut it down forcefully, or you can run `vagrant suspend` to simply
suspend the virtual machine. In either case, to restart it again,
simply run `vagrant up`.


cd /vagrant - This includes all the files from our project directory
you can check by running ls command.
If you create any file in this folder via command line in the server(vagrant machine) it automatically gets created in  your
project directory(host).

# create a python virtual environment
python -m venv ~/env

activate python virtual env -> source ~/env/bin/activate

The reason we  do it in home directory of vagrant server so that we do not create 
the packages in our host machine

deactivate python venv -> deactivate

Refer python cheatsheet-> https://python-guide.readthedocs.io/en/latest/dev/virtualenvs/

install the python dependecies in venv
pip install -r requirements.txt

# create a django scafold project
django-admin.py startproject profiles_project .

# create a module for profiles api
python manage.py startapp profiles_api

# add installed apps to settings.py

# run django dev server
python manage.py runserver 0.0.0.0:8000
open browser and run localhost:8000