# Django Login

Login system made with Django

## Developing

- Install Python 3
- Install pip3
- sudo apt-get install python-dev
- Install mysql-server
- sudo apt-get install libmysqlclient-dev
- Activate a virtual environment
- python install -r requirements.txt
- Create a MySQL database
- Execute the MySQL script
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

- ./manage.py migrate
- ./manage.py runserver
