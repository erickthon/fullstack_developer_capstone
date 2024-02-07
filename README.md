# Django Application Setup

This repository contains a Django application. Follow the steps below to prepare the environment and run the application.

## Prerequisites

- Python 3.x installed on your system
- pip package manager

## Setup Instructions

1. Install `virtualenv` if you haven't already:
   pip install virtualenv

2. Create a virtual environment named djangoenv:
   virtualenv djangoenv
3. Activate the virtual environment. Use the appropriate command based on your operating system:
   source djangoenv/bin/activate
4. Install the required dependencies from the requirements.txt file:
   python3 -m pip install -U -r requirements.txt
5. Run database migrations to create necessary database schema:
   python3 manage.py makemigrations
   python3 manage.py migrate
6. Start the Django development server:
   python3 manage.py runserver
