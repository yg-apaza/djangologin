# Django Login

Login system made with Django

## Developing

- Install Python 3. Python 3 comes pre-installed as a default python interpreter for Ubuntu 18.04.
``sudo apt install python3-minimal``
- Install pip3
``sudo apt-get install python3-pip``
- Install the standard development library for Python
``sudo apt-get install python3-dev``
- Install MySQL server
``sudo apt-get install mysql-server``
- Install MySQL libraries
``sudo apt-get install libmysqlclient-dev``
- Clone this repo and activate a virtual environment in the same directory
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
        'NAME': 'login',
        'USER': 'root',
        'PASSWORD': '123456',
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
