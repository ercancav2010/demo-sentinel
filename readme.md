# Sentinel Demo

This is a basic demo showing some of the functionality of Sentinel on Laravel 4.2.

## Installation

##### 1. Clone this repo:

```
git clone git@github.com:cartalyst/demo-sentinel.git
```

##### 2. Setup your virtual host.

##### 3. Go into your app directory in your terminal and install the dependencies: (cartalyst requires a <a href="https://cartalyst.com/pricing">subscription</a>)

```
composer install
```

##### 4. Configure your database connection by opening `app/config/database.php` file.

##### 5. Update the `app/config/mail.php` file to use your email credentials.
>**Note:** make sure you set `pretend` to false after you configure your email credentials.

##### 6. Run the migrations

```
php artisan migrate --package="cartalyst/sentinel"
```

##### 7. Run the migration & database seeder

```
php artisan migrate --seed
```

##### 8. Publish the package to app folder(app/config/packages), so that you can manage throttling or other settings

```
php artisan config:publish cartalyst/sentinel
```
