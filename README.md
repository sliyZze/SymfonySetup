# Simple Symfony Setup

## Installation
Already installed
- Docker Desktop
- IDE (PHPStorm)

Copy the repository and run 
```cmd
docker-compose up -d --build
```
In the project to create the images and the container

## PHP configuration
Go to Settings PHP and select CLI Interpreter from the current php project img

## xDebug configuration
Go to Settings-> PHP-> debug under xDebug the chosen port from the conf 

Go to Settings-> PHP-> Servers and add a new one with "+" give it a name like xDebug
and set port to 80. Click "use path mappings" and add "/var/www/html" under
the Projec files in the row "Absolute path on the server".

Go Run / Debug Configurations beside the bug icon and select "edit
configurations". Press "+" and add the "PHP Remote Debug". Name it 
example xDebug and check "Filter debug connection by IDE Key". Select
the server you created and type in the IDE Key "PHPSTORM".

## Symfony packages
Already installed
- maker-Bundle
- doctrine orm

