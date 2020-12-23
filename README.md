# Welcome to django-rest-auth
  ===========================


Django-rest-auth provides a set of REST API endpoints for Authentication and Registration

# Documentation
  -------------
  http://django-rest-auth.readthedocs.org/en/latest/


# Technology Stack We have used

1. Python 3.6
2. Django REST Framework
3. sqlite3 Database
4. Google Chrome v.83.0.4103.61    
5. Google Chrome driver v.83.0.4103.61


# Project Structure:
 
	
	.
	├── mysite
	│   ├── db.sqlite3
	│   ├── manage.py
	│   └── mysite
	│       ├── asgi.py
	│       ├── __init__.py
	│       ├── __pycache__
	│       ├── settings.py
	│       ├── urls.py
	│       └── wsgi.py
	└── README.md
	

# Features:
  ---------
  * User registration

  * User email verification

  * Change password - with password reset email.

 
  

## APIs Details

See documentation [here.](./API.md)
  
  
## Run the project Locally ##

i. Clone the repository.

ii. Go to directory of manage.py and install the requirements.

	pip install -r requirements.txt
	
**Note:**
You may configure the virtual environment if required.

For instructions, click here : https://virtualenv.pypa.io/en/latest/installation/
    
iii. Create local_settings.py inside mysite directory.

	EMAIL_HOST_USER = '<to_be_filled>'

	EMAIL_HOST_PASSWORD = '<to_be_filled>'

	DEFAULT_FROM_EMAIL = '<to_be_filled>'

**Note:**
By default, dbSqlite3 database is used. You may also use different database in local_settings file if required.

iv. Run migrations

	python manage.py migrate

v. Ready to run the server.

	python manage.py runserver



# Linting:

	make lint


# Testing:

	python manage.py test







	
