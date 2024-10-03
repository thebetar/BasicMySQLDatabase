# Instructions

In this project we create a mysql database and run queries on it to better understand SQL.

To initialise the project use
`docker compose -f ./mysql-docker-compose.yml up --build`

# Commands

-   To spin up the projects follow the following steps
    -   `docker exec -it edaba_mysql bash` to open bash in the container
    -   `mysql -u root -p` in the container to login to the database
    -   Fill out password 'test_pass'
    -   You're in!
-   To go to a database use `USE <database_name>;`
-   To create a table use `CREATE TABLE <table_name> (<column_name> <type> <functions>, ..., PRIMARY KEY(<column_name>), FOREIGN KEY(<column_name>) REFERENCES <table_name>(<column_name>));`
-   To query a row use `SELECT * FROM <table_name> WHERE <condition>;`
-   To insert a row use `INSERT INTO <table_name> (<column_name>) VALUES (<values>);`
-   To query a row using a join `SELECT * FROM <table_name> LEFT JOIN <table_name2> ON <table_name>.<column_name>=<table_name2>.<column_name2>;`
-   To delete a row use `DELETE FROM <table_name> WHERE <condition>;`
-   To update a row use `UPDATE <table_name> SET <column_name>=<value> WHERE <condition>;`
