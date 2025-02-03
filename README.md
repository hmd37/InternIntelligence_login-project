# Login Project

This is a Django-based project that provides user authentication features, including registration, login, logout, and token refresh using JWT (JSON Web Tokens).

## Features

- User Registration
- User Login
- User Logout
- JWT Token Refresh

## Requirements

- Python 3.x
- Django
- Django REST Framework
- djangorestframework-simplejwt
- PostgreSQL

## Setup

1. **Clone the repository:**

   ```bash
   git clone <repository-url>
   cd login_project
   ```

2. **Install pipenv if not already installed:**

   ```bash
   pip install pipenv
   ```

3. **Install the dependencies:**

   ```bash
   pipenv install
   ```

4. **Activate the virtual environment:**

   ```bash
   pipenv shell
   ```

5. **Apply migrations:**

   ```bash
   python manage.py migrate
   ```

6. **Run the server:**

   ```bash
   python manage.py runserver
   ```

## Usage

- **Register a new user:** Send a POST request to `/register/` with user details.
- **Login:** Send a POST request to `/login/` with username and password to obtain a JWT token.
- **Logout:** Send a POST request to `/logout/` to invalidate the token.
- **Refresh Token:** Send a POST request to `/token/refresh/` with the refresh token to obtain a new access token.
