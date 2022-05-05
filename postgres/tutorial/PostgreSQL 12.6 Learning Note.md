# PostgreSQL 12.6 Learning Note

## Psql and applications running in it

**Psql** is the PostgreSQL interactive terminal. You can take the **Psql** as the front-end of the PostgreSQL, so that it enables you to carry out any SQL queries, check the result of queries, and invoke a set of **meta-commands** and shell-like functions to help you 

## User, Group and Role

In Postgres, User, Group and Role are the same thing. They are all roles. For example, **CREATE USER** equals **CREATE ROLE** with LOGIN permission.

```sql
CREATE USER myuser WITH PASSWORD 'mypassword';
```

```SQL
CREATE ROLE myuser WITH LOGIN PASSWORD 'mypassword';
```

The above two SQL scripts do the same thing that to create a user named "myuser" . You don't need to specify the LOGIN permission 

