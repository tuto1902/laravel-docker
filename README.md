# laravel-docker
A Laravel + MySQL + Apache dev environment with Docker

# Installation
Make sure you have docker installed. Then run

````
$ git clone git@github.com:tuto1902/laravel-docker.git
$ cd laravel-docker
$ docker-compose up -d
````

## Composer install & artisan commands [TailwindCSS]
```
$ docker exec -it laravel-app bash -c "sudo -u devuser /bin/bash"

$ composer install
$ composer require laravel/ui
$ composer require laravel-frontend-presets/tailwindcss --dev
...
$ php artisan key:generate
...
$ php artisan migrate
...
$ php artisan ui --auth
```

## Compile assets with npm
```
$ docker-compose run --rm npm install
$ docker-compose run --rm npm run dev
```

## Visit http://localhost:8080
