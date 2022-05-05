# Docker and Postgres Notes

## **Experiment Environment**: 

1. Win10 pro; 
2. Docker Desktop 4.1.1 (69879)
3. PostgreSQL 12.6 (Debian 12.6-1.pgdg100+1)

## Operations on Docker (Enter into Psql console)

### Enter Psql console

After the postgres image started successfully, you may open the psql console by clicking the console button on the Docker's GUI toolbar. See picture as follows:

![Image 037](1_BasicOperations.assets/Image_037.png)

Then, a terminal comes out and you may see a "**#**" at the top left corner in the terminal. The symbol "**#**" means you are now in Psql bash.

![Image 038](./1_BasicOperations.assets/Image_038.png)

Enter `psql -U postgres` in the terminal to switch to the user "postgres" like the picture shown below.

![Image 039](1_BasicOperations.assets/Image_039.png)

That's it. Now you are in the Psql console and you can do tasks of postgres. Enter `exit` at the "#" you can simply quit from the console.

## List all users(roles)

In Postgres console, we can use meta-command`\du` at the "#" prompt symbol to show available users(roles) in the server. Or, we can use the following SQL script to do the same.

```SQL
SELECT rolname FROM pg_roles;
```

The results we can see here as follows.

![Image_001](1_BasicOperations.assets/Image_001.png)



### Create a user(role)





sudo -u postgres psql
postgres=# create database mydb;
postgres=# create user myuser with encrypted password 'mypass';
postgres=# grant all privileges on database mydb to myuser;
