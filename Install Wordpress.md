# Install Wordpress

## An example: building a wordpress for linuxharbour.com

```
$ mkdir /var/www/linuxharbour.com
$ cd /var/www/linuxharbour.com
$ wget https://wordpress.org/latest.zip
$ unzip latest.zip
$ mv wordpress/* .
```

## Setup the MySQL database for the wordpress  

```
CREATE DATABASE linuxharbour;
CREATE USER 'linuxharbour'@'localhost' IDENTIFIED BY 'SECRETPASSWORD';
GRANT ALL ON linuxharbour.* to 'linuxharbour'@'localhost';
FLUSH PRIVILEGES;
```
