# mySqlOneReporting
mySqlOneReporting is a contribution for the 101companies project (http://101companies.org).
It´s purpose is to extend the database schema as defined in [Contribution:mySqlOne](http://101companies.org/wiki/Contribution:mySqlOne).
For more information please refer to [Contribution:mySqlOneReporting](http://101companies.org/wiki/Contribution:mySqlOneReporting).

## Requirements
* MySQL Client >= 5.0
* MySQL Server >= 5.0

## Preparation
Create the database(s):

    mysql> CREATE DATABASE onereporting;

NOTE: Grant privileges in case you don´t want to use the root user.
You can use "n" source databases.

Load database schema:

    $ mysql -u <USERNAME> -p -h <HOSTNAME> onereporting < sql/schema.sql

OPTIONAL: Populate the databases using sample data:

    $ mysql -u <USERNAME> -p -h <HOSTNAME> onereporting < sql/sample.sql
