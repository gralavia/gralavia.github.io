---
title: Flask Social Media Platform
has_children: true
layout: default
nav_order: 5
---

This is a Flask web application that allows users to register, log in, like posts, comments, and delete posts. 

## Flask Application Setup (create_app function):
### Flask App Initialization:
1. Creates a Flask app.
2. Configures the app's secret key and sets the URI for the SQLite database.
### Database Initialization:
Initializes a SQLAlchemy database and associates it with the Flask app.
### Blueprint Registration:
1. Registers two blueprints (views and auth) that define different parts of the application's routes.
2. views is associated with general views (e.g., homepage, post details).
3. auth is associated with user authentication-related views (e.g., login, register).
### Database Creation and Login Manager Setup:
1. Calls the create_database function to create the SQLite database if it doesn't exist.
2. Initializes a Flask-Login LoginManager and sets up user loading.
## Database Creation (create_database function):
1. Checks if the SQLite database file (database.db) exists in the "website" directory.
2. If not, creates the database using SQLAlchemy within the Flask app context.

## Note:
The SECRET_KEY is a cryptographic key used to keep data safe. It should be kept secret and unique for each Flask application.
The SQLALCHEMY_DATABASE_URI specifies the URI for the SQLite database.