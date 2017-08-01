## Ranktrail template for WordPress.

This imge works with external MySQL database.
Before you start the instaltion you need to setup the WorpdPress database, user and password with the following commands;
```
$ mysql -u root -p
```
```
CREATE USER wp_user IDENTIFIED BY 'mypass';
CREATE DATABASE wordpress;
GRANT ALL PRIVILEGES ON wordpress.* TO wp_user;
```
Alsow you need to create two Rancher sotrage pools:
* rt-wordpress-code
* rt-wordpress-html

On those storages will be mounted the /code and /var/www/html WordPress folders
