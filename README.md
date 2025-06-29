# Laravel Docker Environment

Ready-to-use Docker setup for PHP/Laravel applications with PostgreSQL, Nginx, and pgAdmin.

## Features

- PHP with Laravel support
- PostgreSQL database
- Nginx web server
- pgAdmin for database management
- Pre-configured Docker environment

## Table of Contents

1. [Requirements](#requirements)
2. [Quick Start](#quick-start)
3. [Detailed Setup](#detailed-setup)
4. [Services](#services)
5. [Contacts](#contacts)

## Requirements

- Docker
- Docker Compose
- Git (optional)

## Quick Start

1. Clone this repository:
```bash
git clone https://github.com/stonedch/laravel-docker-environment.git
cd laravel-docker-environment
```
2. Copy and configure environment files:
```bash
cp .env.example .env
```
3. Start the containers:
```bash
docker-compose up -d --build
```

## Detailed Setup

1. Prepare environment files:
```bash
cp .env.example .env
# Edit .env according to your needs
```
2. Clone Laravel application:
```bash
git clone https://github.com/laravel/laravel.git app
cp ./app/.env.example ./app/.env
# Configure Laravel .env file
```
3. Build and start containers:
```bash
docker-compose up -d --build
```
4. Install PHP dependencies:
```bash
docker-compose exec laravel composer install
```
4. Generate application key:
```bash
docker-compose exec laravel php artisan key:generate --ansi
```
5. Run database migrations:
```bash
docker-compose exec laravel php artisan migrate
```

## Services

- Web server: http://localhost:80
- PostgreSQL: port 5432
- pgAdmin: http://localhost:5050
  - Default credentials (change in .env):

## Contacts

Created by [@stonedch](https://github.com/Stonedch)
