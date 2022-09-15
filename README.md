# Laravel Docker

PHP/Laravel, PostgreSQL, Nginx, pgAdmin.

## Table of content:

- [General info](#general-info)
- [Setup](#setup)
- [Contacts](#contacts)

## General info

PHP/Laravel, PostgreSQL, Nginx, pgAdmin.

## Setup

```console
$ cp .env.example .env (and configurate)
$ git clone https://github.com/laravel/laravel.git app
$ cp ./app/.env.example. env (and configurate)
$ docker-compose up -d --build
$ docker-compose exec laravel composer install
$ docker-compose exec laravel php artisan key:generate --ansi
$ docker-compose exec laravel php artisan migrate
```

## Contacts

Created by [@stonedch](https://github.com/stonedch)
