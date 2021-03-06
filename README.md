# BeSnitch

BeSnitch is a social network service for those who want to stay anonymous, yet want to tell the world what it needs to know.

BeSnitch allows you to post articles or comments without having to reveal who you are, and posts get deleted when it reaches a certain number of views defined by the owner of the post.

## Installation
Make sure you have [Python 3](http://python.org) installed before you begin this step!

1. Install Python3 Package Installation Manageer

`sudo apt-get install python3-pip`

2. Install *virtualenv* so that this project gets separated from other projects

`sudo pip3 install virtualenv `

3. In your desired directory, create a virtual environment (or raw environment)

`virtualenv [DIRECTORY_NAME_OF_YOUR_CHOICE]`

4. Activate your virtual environment

* Linux: `source [DIRECTORY_NAME_OF_YOUR_CHOICE]/bin/activate`
* Windows: `[DIRECTORY_NAME_OF_YOUR_CHOICE]/Scripts/activate`

5. Clone this repository in your desired repository

`git clone git@github.com:papapalapa/BeSnitch.git`

6. Install the libraries:

`pip install -r requirements.txt`

7. Execute database migration

`python manage.py makemigrations`

`python manage.py migrate`

8. Run the server

`python manage.py runserver localhost:8888`

9. Open a browser of your choice and type **localhost:8888**

10. KaBOOM!

You are ready to move on!

## Configuration
#### Creating an admin account in the project

After you run this command:

`python manage.py createsuperuser --email [YOUR_EMAIL] --username [USERNAME]`

it will prompt you to create a password for this account