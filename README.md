Symfony2 Starter Kit
======

A Symfony project to start new systems with user control, bootstrap.


Includes:
1. Symfony 2.7
2. Bootstrap 3.x
3. FosUserBundle
4. jQuery 11.x


NEEDS
1. PHP 5.5+ 
2. MySQL 2.+
3. composer.phar
4. Github account
5. PHP extensions



<h1>INSTALL</h1>

1. Clone the project
```
$ git clone git@github.com:cmontedonico/symfony-starter-kit.git
```
2. Install the Vendor with Symfony 2.7
```
$ composer install  
``
3. Configure the Database
````
    $ cd symfony2
    $ cp app/config/parameters.yml.dist parameters.yml
    $ vi app/config/parameters.yml // change the Database information
    $ php app/check.php
```

 This must be something like this.
  *****************************************
  [OK]
  Your system is ready to run Symfony2 projects
    ***************************************
```
 $ php app/console doctrine:schema:update --force
    Check the database for the FOS_USER table.
 $ php app/console doctrine:schema:update --force
    Create first user
```
    


3. WebServer
        3.1 if you have apache/nginx install your virtual directory.
        3.2 If you don't have webserver
            $ php app/console server:run

4. Website
        Open your browser and go to 127.0.0.1/app_dev.php


<h1>Possible Errors</h1>
      PARSER ERROR WITH CLASS.PHP
      ```
        $rm -rf app/cache/*
        $rm -rf app/logs/*
      ```

      Library errors
        install php extensions: ctype and tokenizer


************************************
Included and configured
    "require": {
            "php": ">=5.3.9",
            "symfony/symfony": "2.7.*",
            "doctrine/orm": "~2.2,>=2.2.3,<2.5",
            "doctrine/dbal": "<2.5",
            "doctrine/doctrine-bundle": "~1.4",
            "symfony/assetic-bundle": "~2.3",
            "symfony/swiftmailer-bundle": "~2.3",
            "symfony/monolog-bundle": "~2.4",
            "sensio/distribution-bundle": "~4.0",
            "sensio/framework-extra-bundle": "~3.0,>=3.0.2",
            "incenteev/composer-parameter-handler": "~2.0",
            "friendsofsymfony/user-bundle" : "~2.0@dev",
            "braincrafted/bootstrap-bundle": "~2.0",
            "twbs/bootstrap": "3.0.*",
            "jquery/jquery":  "1.11.*"