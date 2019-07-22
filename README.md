MySQL Dumpper
===

# Prerequisites

* [mysqldump](https://dev.mysql.com/doc/refman/8.0/en/mysqldump.html) command

# Running

Copy and update Environment file :

>cp .env.sample .env

Create the **tables** file, this will contain the list of the table to export a selected database *db_name* :

>cp tables.sample tables

Get the list of table to export :

>select table_name from information_schema.tables where table_schema = 'db_name';

Copy the table's name inside the **tables** file.

Run the exporter :
>./index
