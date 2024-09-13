### Source Tutorial

> https://youtu.be/6c4jVLWmDYU?si=Tc7Meiwub-CbNdOb&t=4510

> GitHub : https://github.com/tonyxhepa/filamentphp-v3-tutorial

> This Git: https://github.com/samedan/2409_laravel-filament

> Countries : [laravel-country-states-city-seeds-migration](https://github.com/mshoaibdev/laravel-country-states-city-seeds-migration)

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

# Create Admin user

> php artisan make:filament-user

### Create resources for a model in Filament Directory

> php artisan make:filament-resource Country
> php artisan make:filament-resource State --generate
> ![Cities generated](https://github.com/samedan/2409_laravel-filament/blob/main/public/printscreens/cities.jpg)
> php artisan make:filament-resource City --generate --view
> ![Cities generated](https://github.com/samedan/2409_laravel-filament/blob/main/public/printscreens/users.jpg)

## Edit Icon & Menu & Slug & Name etc

> CountryResouces.php
> ![Menu left column](https://github.com/samedan/2409_laravel-filament/blob/main/public/printscreens/menu.jpg)

## Font, Colors, Logo & Favicon

> AdminPanelProvider.php

### Seed data

> \database\seeders\...
> php artisan migrate:fresh
> php artisan db:seed

### Create form - States/Create States

> StateResources.php ->add country relationship to 'Select' field
> Models\State.php -> belongsTo
> ![Create State](https://github.com/samedan/2409_laravel-filament/blob/main/public/printscreens/create-states.jpg)
