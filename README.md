#### Install Project

1. Run `sudo git clone https://github.com/jeremykenedy/laravel-tasks.git laravel-tasks`
2. Create a MySQL database for the project
    * ```mysql -u root -p```, if using Vagrant: ```mysql -u homestead -psecret```
    * ```create database laravelTasks;```
    * ```\q```
3. From the projects root run `cp .env.example .env`
4. Configure your `.env`
5. Run `sudo composer update` from the projects root folder
6. From the projects root folder run `sudo chmod -R 755 ../laravel-tasks`
7. From the projects root folder run `php artisan key:generate`
8. From the projects root folder run `php artisan migrate`
9. From the projects root folder run `composer dump-autoload`


#### View the Project in Browser
1. From the projects root folder run `php artisan serve`
2. Open your web browser and go to `http://localhost`


### Laravel-Tasks Authentication URL's (routes)
* ```/```
* ```/auth/login```
* ```/auth/logout```
* ```/auth/register```
* ```/password/reset```

### Laravel-Tasks URL's (routes)
* ```/home```
* ```/tasks```
* ```/tasks/create```
* ```/tasks/{id}/edit```
* ```/tasks-all```
* ```/tasks-complete```
* ```/tasks-incomplete```

#### Laravel Developement Packages Used References
* https://laravelcollective.com/docs/5.2/html
* http://laravel.com/docs/5.2/authentication
* http://laravel.com/docs/5.2/authorization
* http://laravel.com/docs/5.2/routing
* http://laravel.com/docs/5.0/schema
