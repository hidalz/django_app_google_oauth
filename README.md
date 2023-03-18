# Django Allauth Google OAuth Boilerplate

This is a boilerplate Django application that uses Django Allauth for user authentication with Google OAuth. It provides a simple login through Google OAuth that can be used as a starting point for building more complex applications.

## Installation

To use this boilerplate, follow these steps:

### 1. Clone the repository:

```shell
git clone https://github.com/hidalz/django_app_google_oauth
```

### 2. Install dependencies:

```shell
cd django_app_google_oauth
pip install -r requirements.txt
```

### 3. Run database migrations:

```
python3 manage.py migrate
```

### 4. Create a Google OAuth application at the Google Developer Console.

### 5. Create a superuser to log in as admin

```shell
python3 manage.py createsuperuser
```

### 6. Run the development server:

```shell
python3 manage.py runserver
```

### 7. Log in as admin

### 8. Head to Social Applications and input:

- Provider: Google
- Name: Any, i.e: OAuth app
- Client id: The Google client id
- Secret key: Google client secret
- Sites: 127.0.0.1:8000


## Usage

Once the server is running, you can access the login page at /accounts/google/login/. Clicking the "Sign in with Google" button will redirect you to the Google OAuth consent screen. After granting access, you will be redirected back to the application and logged in.

To view the registered users, navigate to the Django admin portal at /admin/. You can log in with the superuser account created during installation.

There is /logout/ URL to unlog when registered as any other user.

## Info

Reference: https://www.section.io/engineering-education/django-google-oauth/
Done for a University Project in Master's in Cybersecurity in UC3M

