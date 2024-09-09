### Source Tutorial

> https://www.youtube.com/watch?v=6c4jVLWmDYU

> GitHub : https://github.com/tonyxhepa/filamentphp-v3-tutorial

### Install laravel

> composer create-project laravel/laravel:^10.0 example-app

### Install Filament

# Source

> https://filamentphp.com/docs/3.x/panels/installation

> composer require filament/filament:"^3.2" -W

> php artisan filament:install --panels

> php artisan migrate

> php artisan make:filament-user

# Open filament

> http://127.0.0.1:8000/admin

### Create resources for a model in Filament Directory

> php artisan make:filament-resource Country
> php artisan make:filament-resource State --generate
> php artisan make:filament-resource City --generate --view
