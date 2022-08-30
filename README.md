<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

# Getting started


Clone the repository

    git clone git@github.com:akitomen/microservices-laravel-docker-vue-nuxt-redis-rabbitmq.git

Switch to the repo folder

    cd microservices-laravel-docker-vue-nuxt-redis-rabbitmq

Run containers for following services : Users, Influencer, Emails, Checkout, Admin, Admin-frontend

    docker-compose build
    
    docker-compose up -d
        
    
Install all the dependencies using composer for following services :  Users, Influencer, Emails, Checkout, Admin, Admin-frontend

    docker-compose exec app composer install 

    
Run the database migrations (Set the database connection in .env before migrating)

    docker-compose exec app php artisan migrate

Copy the example env file and make the required configuration changes in the .env file

    cp .env.example .env
    
    DB_DATABASE=db
    DB_USERNAME=root
    DB_PASSWORD=root

For Influencer-frontend and Admin-frontend services use the following commands :
```
npm install
```
```
npm run serve
```

```
npm run build
```
```
npm run lint
```
    
For Checkout-frontend services use the following commands :

```
$ npm install
```
```
$ npm run dev
```
```
$ npm run build
```
```
$ npm run start
```
```
$ npm run generate
```

