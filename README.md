# Docker For Laravel Development
This repository provides you a starter to dockerize your laravel development process

## Usage
1. Install [docker](https://docs.docker.com/engine/installation/) and [docker-compose](https://docs.docker.com/compose/install/)
2. Move all files and folders from this repository to your laravel project.
3. From your laravel project directory, start your docker service by running command:
  ```
    docker-compose up -d --build
  ```
4. Four additional container i created to ease the development which are artisan, npm, composer and phpmyadmin
    - `docker-compose run --rm composer update`
    - `docker-compose run --rm npm run dev`
    - `docker-compose run --rm artisan migrate`
5. For phpmyadmin you can open it at : `<your-docker-ip>:8088`

## Exposed Ports
1. **nginx**: `80`
1. **mysql**: `3306`
1. **php**: `9000`
