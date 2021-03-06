
## About the web-App:

CrowdFunding Web App that allow user to:

- Signup and login
- Create and modify his profile data or delete his account
- Create or Delete funding projects
- show all projects details
- Donate, Rate, Report, and Comment other projects


## Built With:

- [Django Framwork](https://docs.djangoproject.com/en/)
- [MySqlClient Database](https://pypi.org/project/mysqlclient/)
- [Soft UI Design System](https://github.com/app-generator/django-soft-ui-design)
- [HTML, CSS, JS, Bootstrap....](https://www.w3.org/)

## Installation and Run project:

1- Download or Clone the project

2- Install python on your machine

- [Download from here](https://www.python.org/downloads/windows/)
- [check your version]

  ```bash
  python --version
  ```

  \*\* must be v.3 or up

- [install and upgrade pip]

  ````bash
  python3 -m pip install --upgrade pip

3- run your mysql server and create new Schema in your DBMS with name "crowdfunding" or change the name at (setting.py) and set your DB Server information [ host name and password ]

4- Open the project in vs Code

5- In a Terminal window run the following >>

- [install VirtualEnvironment]
  ```bash
  pip3 install virtualenv
  ```
- [Create and Activate VirtualEnvironment]

  ```bash
  virtualenv .venv
  ```

  for win

  ```bash
  .venv\Scripts\activate
  ```

  for linux

  ```bash 
  source .venv/bin/activate
  ```

- [Install requirments]
  ```bash
  pip3 install -r requirements.txt
  ```
- [Install mysqlClient]
  ```bash
  pip3 install mysqlclient
  ```

6- Set These Values in "setting.by" file to test Verification using email

EMAIL_USE_TLS = True  
EMAIL_HOST = 'smtp.gmail.com'  
EMAIL_HOST_USER = 'ahmedfares4518@gmail.com'  
EMAIL_HOST_PASSWORD = 'djsfzhgksgktljtf'
EMAIL_PORT = 587

\*\* or you can add your [gmail] but insure that the account security not activated :D

7- put the 'index.py' file to this path '.venv/Lib/site-packages/django/templatetags/'

8- go to this path '.venv/Lib/site-packages/django/conf/global_settings.py'

- search for [PASSWORD_HASHERS] list
- add this 'django.contrib.auth.hashers.UnsaltedMD5PasswordHasher' in the first of this list

9- Run the following to load Data base

```bash
python manage.py makemigrations
```

```bash
python manage.py migrate
```

10- create your superuser [admin] to access [Admin Dashboard]

```bash
python manage.py createsuperuser
    > enter user name
    > enter user email
    > enter password
```

11- After All is Finished run server

```bash
	python manage.py runserver
```

\*\* take the link (http://127.0.0.1:8000/) and put it on your browser

## Notes

1- you can access the [Admin Dashboard] by :

- in your broswer use (http://127.0.0.1:8000/admin)
- enter user-nameand password created
- add some categories and tags
- you can featured projects from here

2- if you create any account in site you need to activate it from this [gmail account] >>

- Email : ahmedfares4518@gmail.com
- Password : djsfzhgksgktljtf
## Demo

https://user-images.githubusercontent.com/72516521/167317970-c0bfbb76-4342-462c-931c-b21f9f625d39.mp4

# Authors

- [@Ahmed Ebrahim]
- [@Mohamed Fathi]
- [@Eman Mahmoud]