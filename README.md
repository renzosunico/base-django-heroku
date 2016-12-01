# base-django-heroku
Deploying Django app to Heroku can be a bit tricky and confusing.
So I decided to create a base or empty django project that can be cloned and deployed as soon as possible.

## After Deployment
After deploying this project. You will need to run your migrations. To do this, you need to login to Heroku in your terminal. You need to install [Heroku CLI](https://devcenter.heroku.com/articles/heroku-command-line) in order to do this.

To login
```
heroku login
Email:
Password:
```

To migrate
```
heroku run "python manage.py migrate --settings='settings.production'" --app NAME_OF_HEROKU_APP
```

Get List of Heroku Apps
```
heroku apps
```
