# Postgres Basic Operations

Env: Docker on Lenovo (local img: postgres-0)

PostgreSQL version: PostgreSQL 12.6 (Debian 12.6-1.pgdg100+1)

## Operations on Docker (Enter into Psql console)

### Enter Psql console

After the postgres image started successfully, you may open the psql console by clicking the console button on the Docker's GUI toolbar. See picture as follows:

<<<<<<< HEAD
![Image 037](./1_BasicOperations.assets/Image_037.png)
=======
![Image 037](1_BasicOperations.assets/Image_037.png)
>>>>>>> 3b9669a18ab6f3ad61e74be2c672ec27b126ef20

Then, a terminal comes out and you may see a "**#**" at the top left corner in the terminal. The symbol "**#**" means you are now in Psql bash.

![Image 038](./1_BasicOperations.assets/Image_038.png)

Enter "**psql -U postgres**" in the terminal to switch to the user "postgres" like the picture shown below.

![Image 039](1_BasicOperations.assets/Image_039.png)

That's it. Now you are in the Psql console and you can do tasks of postgres.





sudo -u postgres psql
postgres=# create database mydb;
postgres=# create user myuser with encrypted password 'mypass';
postgres=# grant all privileges on database mydb to myuser;
