# Django Application Setup

This repository contains a Django application. Follow the steps below to prepare the environment and run the application.

## Prerequisites

- Python 3.x installed on your system
- pip package manager

## Setup Instructions

1. Install `virtualenv` if you haven't already:
    ```bash
    pip install virtualenv
    ```

2. Create a virtual environment named `djangoenv`:
    ```bash
    virtualenv djangoenv
    ```

3. Activate the virtual environment. Use the appropriate command based on your operating system:
    - Linux/MacOS:
        ```bash
        source djangoenv/bin/activate
        ```
    - Windows:
        ```bash
        djangoenv\Scripts\activate
        ```

4. Install the required dependencies from the `requirements.txt` file:
    ```bash
    python3 -m pip install -U -r requirements.txt
    ```

5. Run database migrations to create necessary database schema:
    ```bash
    python3 manage.py makemigrations
    python3 manage.py migrate
    ```

6. Start the Django development server:
    ```bash
    python3 manage.py runserver
    ```

7. Access the application in your web browser at `http://127.0.0.1:8000/`

## Notes

- Make sure to replace `python3` with the appropriate command if your Python executable has a different name.
- Adjust the virtual environment activation command according to your operating system.
- Ensure that the necessary database configurations are set up in the Django settings file (`settings.py`).
