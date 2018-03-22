# Roskilde Building Project
___

## Intro and requirements
This project is for the purpose of introducing our new Campus Building at Zibat.

The project comprises 3 small project that connects together and run via Docker. To get the project up and running, please follow the instruction below.

| N | Requirements |
|---|-----------------------|
| 1 | Composer installed    |
| 2 | Docker installed      |
| 3 | Laravel installed     |
| 4 | Git

## Preparation
1. Pull the repo via Git
2. `docker exec -it roskildebuilding_api_1 /bin/bash` to go inside API container
3. Inside the container, run `cd var/www/html/app` to go to root folder of API
4. Run `php artisan key:generate` to add key to Laravel
5. Inside the container, run `composer install` to prepare al dependencies.
6. Run `php artisan migrate` to prepare db schema
7. Run `php artisan db:seed` to generate fake data from Faker
8. API address: http://localhost:8083/
9. Front-end address: http://localhost:8083/

Cheers man :)
Turbo