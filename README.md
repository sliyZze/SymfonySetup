# Simple Symfony Setup

## Installation
Already installed
- Docker Desktop
- IDE (PHPStorm)

Copy the repository

in the .env change it to your project name
```env
COMPOSE_PROJECT_NAME= x /automatic soon
```
then run in the project to create the images and the container
```cmd
docker-compose up -d --build
```
and then to install all dependencies
```cmd
docker-compose exec php composer install
```


## PHP configuration
Go to Settings PHP and select CLI Interpreter from the current php project img

## xDebug configuration
Go to Settings-> PHP-> debug under xDebug the chosen port from the conf 

Go to Settings-> PHP-> Servers and add a new one with "+" give it a name like xDebug
and set port to 80. Click "use path mappings" and add "/var/www/html" under
the project files in the column "Absolute path on the server".

Go Run / Debug Configurations beside the bug icon and select "edit
configurations". Press "+" and add the "PHP Remote Debug". Name it 
example xDebug and check "Filter debug connection by IDE Key". Select
the server you created and type in the IDE Key "PHPSTORM".

## Database in PHPSTORM
Select mariadb and look at the data in the env or compose for the login.

## Symfony packages
Already installed
- maker-Bundle
- doctrine orm

## Note
don't forget to change the ports if you run multiple projects at the same
time, have fun! -> localhost:8080