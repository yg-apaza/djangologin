# Django Login

Login system made with Django

## Developing

- Install Python 3. Python 3 comes pre-installed as a default python interpreter for Ubuntu 18.04.
``sudo apt install python3-minimal``
- Install pip3
``sudo apt-get install python3-pip``
- Install development library for Python
``sudo apt-get install python3-dev``
- Install MySQL server
``sudo apt-get install mysql-server``
- Install MySQL libraries
``sudo apt-get install libmysqlclient-dev``
- Activate a virtual environment
- Install requirements
``python install -r requirements.txt``
- Create a MySQL database
- Edit the database configuration on settings.py

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

- ``./manage.py migrate``
- ``./manage.py runserver``
