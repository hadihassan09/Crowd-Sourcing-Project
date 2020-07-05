<p align="center"><img src="https://laravel.com/assets/img/components/logo-laravel.svg"></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/d/total.svg" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/v/stable.svg" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://poser.pugx.org/laravel/framework/license.svg" alt="License"></a>
</p>

Please Note The Long Delay in page loading is due to bad internet conection.

=============================================
Please Before Starting Make Sure you are connected to the internet for pusher service to Work.
--Before we start please go to https://pusher.com/ and create a new Account
Then Create your new application and dont select its type region should be "AP2"
After that you should be able to aquire your own App Keys
Open the project in an idm of your choice, and set the shown app_id and key and secret into the:
-.env file:

PUSHER_APP_ID=example id
PUSHER_APP_KEY=example key
PUSHER_APP_SECRET=example secret

-resources\assets\js\bootstrap.js:(line 52)
    key: 'example key',

=============================================
--Setup Your Own SQL SERVICE of your own with the specified DATABASE for this application in the .env file.
Please Note: the database should be created earlier and should be empty.
You should edit in the .env file the following:

DB_HOST=YOUR HOST
DB_PORT=YOUR PORT
DB_DATABASE=DATABASE NAME
DB_USERNAME=DATABASE USERNAME
DB_PASSWORD=DATABASE PASSWORD

=============================================
--In The Console type the following Command: php artisan migrate --seed
This will create your accounts and set the auto-accept option to 1.
-Users Accounts are as follows:
email: 0@gmail.com --> 10@gmail.com
all with password '123456'
-Admin Acount:
email: admin@gmail.com
passowrd: '123456'
=============================================
--After The Migrations are done, Please type in php artisan serve and procced to 'http://127.0.0.1:8000' to start the workshop.
=============================================



