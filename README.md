# django-tutorial
## Virtual Env
#### to install virtualenv
`pip install virtualenv`

#### to create virtualenv
`virtualenv <venv_name>`

#### to activate virtualenv
`source <venv_name>/bin/activate`

#### to deactivate virtualenv
`deactivate`

## Git Tutorial
#### initialize git
`git init`

#### add your local repository as remote for your main repository
`git remote add origin https://github.com/user/repo.git`

#### Verify new remote
`git remote -v`

#### to add uncommited files
`git add .`
or
`git add -A`

#### to commit
`git commit -m ""`

#### to pull
`git pull`

#### to push as master
`git push -u origin master`

## Django
#### to start a project
`django-admin startproject <project_name>`

#### to create an app
`python manage.py startapp <app_name>`

#### to run server
`python manage.py runserver`

#### to make migrations to db
`python manage.py makemigrations`

#### to complete migration
`python manage.py migrate`

#### to create superuser
`python manage.py createsuperuser`


## PostgreSQL
#### to start postgres in command line
`psql -U <user_name> <db_name>`

#### to view relations
`\dt`

#### to view users and their roles
`\du`

#### to change password
`\password postgres`


## Steps to add an app to the database
1. Create the app model in models.py file of that app
2. Add the app in the settings.py file of the project
    * app.apps.app_nameConfig
3. Create Migrations (python manage.py makemigrations)
4. Migrate (python manage.py migrate)
5. Add app to the admin
    * from .models import app
    * admin.site.register(app)
