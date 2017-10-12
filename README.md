# sql-tutorial
A simple tutorial to learn MySQL for GWC TV. This is intended to be done in C9.

## Start MySQL
```
$ mysql-ctl start
```

## Create the tables and load the database
```
$ mysql -u [C9 USERNAMe] -p < pets.sql
```
Note that the default password is blank, so you can just press ENTER when prompted for a password.

## Connect to the database
There's two ways to do this in C9.  The easy way is to use the mysql-ctl command
```
$ mysql-ctl cli
```

The standard way is to use the mysql command
```
$ mysql -u [C9 USERNAME] -p pets
```

## Sample queries
Run these queries and see what they do.

```
DESC pets;
SELECT * from pets;
SELECT * FROM pets JOIN visits WHERE pets.account_num=visits.account_num ORDER BY 3;
```

## Exercises
1. Insert a row into each table.
2. Update existing data in a row.
3. Delete a row.
4. Create a new table.
5. Drop a table.
6. Drop a database.