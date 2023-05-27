# Django Google Calendar Api connect

Google calendar OAuth2 integration using Django REST API.

# Steps

Here are the steps you can follow to create a Google Calendar API in the Google Cloud Console:

1. Go to the [Google Cloud Console](https://console.cloud.google.com/) and sign in with your Google account.

2. In the dashboard, click on the "Select a Project" button in the top bar. If you haven't created any projects yet, you'll be prompted to create one.

3. In the sidebar on the left, click on the "APIs & Services" button and then select "Credentials" from the menu.

4. Click on the "Create credentials" button, then select "OAuth client ID".

5. Select "Web application" as the application type, and enter a name for application.

6. In the "Authorized JavaScript Origins" and "Authorized Redirect URIs" fields, enter the URLs of your application that will be handling the OAuth flow.
   In this project, "http://localhost:8000" is set as the "Authorized JavaScript Origins" and "http://localhost:8000/rest/v1/calendar/redirect" is set as the "Authorized Redirect URIs" field.

7. Click on the "Create" button.

8. Once the OAuth client ID has been created, you'll be able to see the client ID and client secret in the "Credentials" tab.

9. In the sidebar on the left, click on the "Library" button, then search for "Google Calendar API" and select it.

10. Click on the "Enable" button to enable the Google Calendar API for roject.

11. Publish application by clicking on OAuth consent screen --> Publish status -->Publish App

12. You can now use the client ID and client secret to authenticate with the Google Calendar API in application.

13. Add client_secret.json file in this application


# Development Setup

1. Install Python and Django on your machine
2. Clone or download the project from the repository
3. Navigate to the project directory in the command line
4. Run  command `pip install virtualenv` to install virtual environment
5. Run command `source//venv//Scripts//activate` to start virtual environment
6. Run  command `pip install -r requirements.txt` to install the project dependencies
7. Run  command `python manage.py migrate` to apply the migrations to the database
8. Run  command `python manage.py runserver` to start the development server
9. Visit "http://127.0.0.1:8000/" in your web browser to see the project running
