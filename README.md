# Laravel Tutorial

## Install Laravel
https://laravel.com/docs/5.5/installation

```bash
# Install PHP Composer
sudo apt-get install composer
sudo apt-get install php-curl php-mcrypt php-mbstring php-gettext php-zip php-pgsql php-mysql

# Install Laravel
composer global require "laravel/installer"
```


## Tutorial
https://laravel.com/docs/5.1/quickstart


```bash
composer create-project laravel/laravel quickstart --prefer-dist
```

```bash
cp .env.example .env
php artisan key:generate
```


Edit .env
```
DB_CONNECTION=pgsql
DB_HOST=127.0.0.1
DB_PORT=5432
DB_DATABASE=coc
DB_USERNAME=coc
DB_PASSWORD=coc@123
```


```
php artisan make:migration create_tasks_table --create=tasks

php artisan migrate

php artisan make:model Task
```
