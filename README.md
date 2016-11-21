fleetcombat-backend
===================

The back-end is an REST API built with the Symfony framework.

#How to setup:
Make sure to have Composer installed globally on your computer. Then clone this repository.

After that run the `composer install` command to install all dependencies.

Make the database connection by editing `/app/config/parameters.yml`. You can copy the `parameters.yml.dist` file if 
there is no file created yet. On your local machine it may look something like this:
```yml
parameters:
    database_host: 127.0.0.1
    database_port: null
    database_name: fleetcombat-backend
    database_user: root
    database_password: root
```

#Database tables:
Migrations are used to create the database schema. Then run the migrations with the bin/console doctrine:migrations:migrate command. For more about migrations read the docs: http://symfony.com/doc/current/bundles/DoctrineMigrationsBundle/index.html
