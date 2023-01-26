# install-mysql-server-on-ubuntu
This repository is intended to facilitate the configuration os mysql server on ubuntu

## Installing mysql-server on Ubuntu

$ ``` sudo apt install mysql-server ```

## Consulting mysql-server IP adress

$ ``` SELECT host FROM information_schema.processlist WHERE ID = connection_id() LIMIT 0,10; ```

## Listening mysql-server port

$ ``` SHOW GLOBAL VARIABLES LIKE 'port'; ```

## Conectar ao servidor mysql
$ ``` mysql -u root ```

##  Uma vez conectado

mysql> ``` ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password'; ```

##  Nas próximas vezes

$ ``` sudo mysql -u root -p ```
