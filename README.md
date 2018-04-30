# Blog Project

**Author**: Alexander Stone, Justin Morris, Madeline Peters, Amanda Moen, Maxwell Rediker.

**Version**: 1.0.0 

## Overview
This project allows a user to build a basic website layout and get the HTML and CSS back that matches their creation.

## Getting Started
To get started, clone the files from GitHub and install all necessary dependencies. From your psql command:
CREATE TABLE users (user_id SERIAL PRIMARY KEY, username VARCHAR(255), email VARCHAR(255), password VARCHAR(255));

CREATE TABLE projects (project_id SERIAL PRIMARY KEY, project_name VARCHAR(255), user_id INTEGER REFERENCES users(user_id), html TEXT, css TEXT );

Then in your command line:
heroku pg:push fozzie postgresql-vertical-34898 --app fozzie-web-builder

Or, more easily, just open our deployed version and save yourself some work.
https://githubmaxwell.github.io/Fozzie-s-Website-Builder-Client/


## Architecture
HTML5, CSS3, JS, Jquery, Handlebars, Ajax.

## Change Log
04-30-2018 3:50pm - Application now has a readme.


## links to any 3rd party APIs that your back-end code will be using
https://developers.google.com/identity/sign-in/web/sign-in#before_you_begin
https://developers.google.com/drive/v3/web/about-sdk 

## Your database structure (table create statements) and any joins you plan to use
TABLE users 
user_id | username  | email | password 

TABLE projects 
project_id  | project_name | user_id INTEGER REFERENCE users(user_id) | html | css

We do not plan to use any joins.

## Credits and Collaborations