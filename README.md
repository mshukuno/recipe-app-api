# recipe-app-api

## Creating Docker image
1. In terminal, change directory to the project folder.
2. ```docker build .```
3. ```docker-compose build```
4. ```docker-compose run app sh -c "django-admin.py startproject app ."```

## Creating models
```docker-compose run app sh -c "python manage.py startapp <name your folder>"```

## Creating new migrations
```docker-compose run app sh -c "python manage.py makemigrations core"```
 
## Unit Test
```docker-compose run app sh -c "python manage.py test"```
with flake8
```docker-compose run app sh -c "python manage.py test && flake8"```

