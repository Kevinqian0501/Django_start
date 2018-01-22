# install python

```
$:virtualenv -p python3.5 py35

$:source py35/bin/activate

$:python --version

Python 3.5.2
```

# install Django

```
$:git clone https://github.com/django/django.git

$:pip install -e django/

$:python -m django --version

2.1.dev20180121070910

```

# Build a project

```
$:django-admin startproject mysite

$:python manage.py runserver 0:8008

“Set host ”

```

# new a app in the project

```
$:python manage.py startapp polls

$:nano polls/views.py 

$:nano polls/urls.py # link views.py

$:nano urls.py  # link polls/urls.py

$:python manage.py runserver 0:8008
```
# wsgi

```
$:gunicorn mysite.wsgi -b0.0.0.0:8008
```
