Quick docker container for prototyping with Laravel. Includes laravel-mongodb, MySQL and Redis.

### Installation:

1. Pull this project.
2. copy .env.example to .env
3. copy ./docker-compose/.env.example to ./docker-compose/.env
4. Then cd into ./docker-compose and run the following commands:
```
$ sudo docker-compose build
$ sudo docker-compose up -d
$ sudo docker-compose ps // to check that all images are "UP"
```
5. Next run "**sudo docker-compose exec app bash**" to access bash on the php container and,
then run the following commands:
```
$ composer install
$ php artisan key:generate
``` 