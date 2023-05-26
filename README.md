Project resulting from the [Laravel 8 from Scratch](https://laracasts.com/series/laravel-8-from-scratch) course in Laracasts. The original code for the project can be found in [this repository](https://github.com/JeffreyWay/Laravel-From-Scratch-Blog-Project).

The project must be ran with Laravel Sail, and you must create a database named `example_app`.

Here are some helpful commands:
- To install the dependencies run:
```
docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v "$(pwd):/var/www/html" \
    -w /var/www/html \
    laravelsail/php82-composer:latest \
    composer install --ignore-platform-reqs
```
- To do the migrations run `sail artisan migrate:fresh --seed`
- To start the project run `sail up`

Don't forget to create a `.env` file and generate an `APP_KEY` value.
