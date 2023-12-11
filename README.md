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

## How-to directions on a Mac

** helpful documentation if on Windows or Linux:
https://kinsta.com/knowledgebase/install-laravel/#how-to-install-laravel-on-macos:

```
brew install docker
brew install composer
brew install php@8.2
composer global require laravel/installer
composer create-project --prefer-dist laravel/laravel laravel-app
cd laravel-app
php artisan serve
```

Go to your browser: http://localhost:8000/

Now that we were able to see the dependancies necessary to get this application up locally, we can apply that knowledge to the dockerization of the application! 

How to dockerize the application now:
Helpful video: https://www.youtube.com/watch?v=uYhowDSkwyk

# Working twith the stack in Docker
```
git clone git@github.com:aprilrieger/larvel-app.git
cd laravel-app
cp .env.example .env
```

After copying the .env.example file set these:
DB_HOST=db
DB_PASSWORD=CHANGEME

```
composer install
docker compose build
docker compose up -d
```

Navigate to browser: http://localhost:8000/