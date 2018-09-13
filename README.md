# Django Login

Login system made with Django

## Developing

- Install Python 3. Python 3 comes pre-installed as a default python interpreter for Ubuntu 18.04.

```shell
sudo apt install python3-minimal
```

- Install pip3

```shell
sudo apt-get install python3-pip
```

- Install the standard development library for Python

```shell
sudo apt-get install python3-dev
```

- Install MySQL server

```shell
sudo apt-get install mysql-server
```

- Install MySQL libraries

```shell
sudo apt-get install libmysqlclient-dev
```

- Activate a virtual environment

```shell
python3 -m venv env
source env/bin/activate
```

- Install requirements

```shell
pip3 install -r requirements.txt
```

- Create a MySQL database

- Edit the database configuration on djangologin/settings.py

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

```shell
python3 manage.py migrate
```

- Create a new user

```shell
python3 manage.py createsuperuser
```

- Start Django built-in web-server

```shell
python3 manage.py runserver
```

- Avoid to commit your database credentials

```shell
git update-index --assume-unchanged djangologin/settings.py
```
