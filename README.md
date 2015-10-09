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



INSTALL

1. Clone the project

 $ git clone git@taquitosoft.com:cmontedonico/symfony2.git

2. Install

 $ cd symfony2
 $ vi app/config/parameters.yml // change the Database information
 $ php app/check.php

 This must be something like this.
  *****************************************
  [OK]
  Your system is ready to run Symfony2 projects
    ***************************************

 $ php app/console doctrine:schema:update --force
    Check the database for the FOS_USER table.


3. WebServer
    3.1 if you have apache/nginx install your virtual directory.
    3.2 If you don't have webserver
        $ php app/console server:run

4. Website
    Open your browser and go to 127.0.0.1/app_dev.php


