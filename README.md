<h3>My Flask-CORS drafts from the FullStack Web Developer Nanodegree</h3>

Creating the plantsdb database locally

1. Create the database - Create the database and a user. Run the following:

```shell
# Connect to the PostgreSQL
psql
# Create the database,  *plantsdb*, and create a user `student`. Grant all privileges to the student
\i <db_folder>/plantsdb_setup.sql
# Exit the PostgreSQL prompt
\q
```

2. Create tables - Once your database is created, you can create a table (plants) and apply constraints. Actual steps may vary depending on your OS.

```shell
# Mac users
psql -f plants.psql -U student -d plantsdb
# Linux users
su - postgres bash -c "psql plantsdb < /path/to/plants.psql"
```
