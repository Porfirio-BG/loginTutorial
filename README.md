# loginTutorial

Simple Django project to exercise basic concepts such as creating virtual environments and projects with Django, upload projects to Github
and use installed Django apps.

#USAGE
Assiming you have a virtualenv running with Django installed.
Create the database running the following command:
  $ python manage.py migrate
Create a superuser in the database running this command:
  $ python manage.py createsuperuser
Setup the app running:
  $ python manage.py runserver [port]
  (if you have smth running in localhost port 8000 specify other appropiate port <<such as 8050>> on [port])
go to localhost:[port]/ in your browser
  (where [port] is the port number where the project is running, defaults to 8000)
Sign in to the app using the superuser credentials defined 
That's it... this app doesn't do much
  
#NOTES
Taken from:
  https://wsvincent.com/django-user-authentication-tutorial-login-and-logout/

#ADDITIONAL NOTES
To upload an existing project to Github using Eclipse:
  1. Right-click on project -> Team -> Share project...
  2. Select "Use or create repository in parent project or folder"
  3. Click on "Create Repository"
  4. Log in to Github
  5. Select create new repository
  6. Copy the path from "Quick setup: use HTTPS" to the clipboard
  7. In Eclipse, from the git perspective expand your project's repository (i.e. loginTutorial)
  8. Under Remotes, select Create Remote
  9. When prompted for the URI select Change...
  10. Paste the URI from clipboard
  11. Enter Github credentials (same as used to log in directly into Github)
  12. Stage all files
  13. Commit all files.
  Done
