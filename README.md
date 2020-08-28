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

