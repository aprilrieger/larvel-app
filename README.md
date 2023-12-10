# The Processs

## Tested on:
- Mac M2
- macOs: Ventura 13.5.2
- Docker: 4.22.1

## Install:
- Docker
- Php
- Composer
- Node.js

## How to directions on a Mac

** helpful documentation if on Windows or Linux:
https://kinsta.com/knowledgebase/install-laravel/#how-to-install-laravel-on-macos:

``````
brew install docker
brew install composer
brew install php
composer global require laravel/installer
composer create-project --prefer-dist laravel/laravel app-name
cd app-name
php artisan serve
```

Go to your browser: http://localhost:8000/

Now that we were able to see the dependancies necessary to get this application up locally, we can apply that knowledge to the dockerization of the application! 

How to dockerize the application now:
Helpful video: https://www.youtube.com/watch?v=uYhowDSkwyk

# Working the stack

Note: All common environment variables located in the .env

## Build the docker image on your machine:
`docker compose build`

## Bring the stack up locally with:
`docker compose up -d`

## Got to your perferred browser
Navigate to http://localhost:8000/