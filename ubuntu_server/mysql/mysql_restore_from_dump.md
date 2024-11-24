# Restoring a database from a single file dump

### Restoring

> sudo mysql -u root -p

> CREATE DATABASE db_name;

> mysql -u root -p nome_do_banco < DUMP-FILE_PATH

### Checking

> sudo mysql -u root -p

> USE db_name

> SHOW TABLES;
