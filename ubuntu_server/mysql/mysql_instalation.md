# MySQL Instalation in Ubuntu Server

### Steps

### Install
> sudo apt update && sudo apt upgrade -y

> sudo apt install mysql-server -y

> mysql --version

> sudo mysql_secure_installation

### Enable root remote access trought another host

> sudo nano /etc/mysql/mysql.conf.d/mysqld.cnf

> bind-address = 127.0.0.1 to 0.0.0.0 ( Accessible from all IP's )

> sudo systemctl restart mysql

### Create User with Privileges

> CREATE USER 'user'@'%' IDENTIFIED BY 'password';

> GRANT ALL PRIVILEGES ON *.* TO 'user'@'%';

> FLUSH PRIVILEGES;

### Basic comands: start, stop, status

> sudo systemctl start mysql

> sudo systemctl stop mysql

> sudo systemctl status mysql
