# Google Cloud SQL Sakila Database

This is a specially adapted version of the Sakila sample database for Google Cloud SQL. The Sakila database is a sample database that represents a DVD rental store, containing tables for films, actors, customers and rental information.

## Files in this Directory

- `mysql-sakila-schema.sql` - Contains the database schema (tables, views, stored procedures)
- `mysql-sakila-insert-data.sql` - Contains all the insert statements to populate the database
- `mysql-sakila-delete-data.sql` - Script to delete all data while preserving the schema
- `mysql-sakila-drop-objects.sql` - Script to drop all database objects

## Deployment Instructions

To deploy this database to Google Cloud SQL, follow these steps:

1. First, deploy the schema:
```bash
mysql -h 34.159.94.208 -u root -p < mysql-sakila-schema.sql
```

2. Then, populate the database with data:
```bash
mysql -h 34.159.94.208 -u root -p < mysql-sakila-insert-data.sql
```
