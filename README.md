# Pug-or-Ugh-API
Create a backend API for a fully coded front end web site. 
Build out the database and REST API backend using the Django REST Framework. 
You'll create database models, program routes, and use token-based authentication to control access to the API.

Paw left or right in this app to help potential pet owners find the dog of their dreams! 
You will be provided with a fully coded front end site that is setup to access a backend that you will build. 
Your task is to build out the database and REST API backend using Django REST Framework that makes the whole thing work.

INSTRUCTIONS:

The application needs the following models with the associated field names included.

Dog Model
name
image_filename
breed
age - integer for months
gender - “m” for male, “f” for female, “u” for unknown
size, "s" for small, "m" for medium, "l" for large, "xl" for extra large, "u" for unknown

UserDog Model
user
dog
status - “l” for liked, “d” for disliked

UserPref Model
user
age - “b” for baby, “y” for young, “a” for adult, “s” for senior
gender - “m” for male, “f” for female
size - “s” for small, “m” for medium, “l” for large, “xl” for extra large

Serializers are needed for the Dog and UserPref Models. 
All fields need to be revealed except user from the UserPref Model.

The front end JavaScript application is expecting the following routes to be in place:

To get the next liked/disliked/undecided dog
/api/dog/<pk>/liked/next/
/api/dog/<pk>/disliked/next/
/api/dog/<pk>/undecided/next/

To change the dog's status
/api/dog/<pk>/liked/
/api/dog/<pk>/disliked/
/api/dog/<pk>/undecided/

To change or set user preferences
/api/user/preferences/

The supplied project includes Token-Based Authentication, that functionality should be maintained.

Unit test the app.
Write unit tests to test that each view is displaying the correct information. 
Write unit tests to test that the models, classes, and other functions behave as expected.
