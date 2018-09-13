# Django Login

Login system made with Django

## Developing

1. Install Python 3. Python 3 comes pre-installed as a default python interpreter for Ubuntu 18.04.
``sudo apt install python3-minimal``
- Install pip3
``sudo apt-get install python3-pip``
- Install the standard development library for Python
``sudo apt-get install python3-dev``
- Install MySQL server
``sudo apt-get install mysql-server``
- Install MySQL libraries
``sudo apt-get install libmysqlclient-dev``
- Activate a virtual environment
``python3 -m venv env``
``source env/bin/activate``
- Install requirements
``pip3 install -r requirements.txt``
- Create a MySQL database
- Edit the database configuration on djangologin/djangologin/settings.py

```
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'database-name',
        'USER': 'database-user',
        'PASSWORD': 'password',
        'HOST': 'localhost',
        'PORT': '3306'
    }
}
```

- Apply migrations
``python3 djangologin/manage.py migrate``
- Create a new user
``python3 djangologin/manage.py createsuperuser``
- Start Django built-in web-server
- ``python3 djangologin/manage.py runserver``
