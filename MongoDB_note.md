# MongoDB Learning Notes

July 12, 2022

The note bases on MongoDB version 5.0

## MongoDB Cloud Platform - Atlas

MongoDB has a cloud platform named Atlas. Here is the [entrance](https://cloud.mongodb.com/).

![20220712015555](./MongoDB_note.assets/20220712015555.png)

### Database/Cluster structure on the cloud

- Organization(s)
  - Project(s)
    - Cluster(s)
      - Database(s) (will not be displayed on the page)

![20220712015938](./MongoDB_note.assets/20220712015938.png)

Atlas provides user **M0 shared cluster** for free.

## MongoDB Shell

Also known as **mongosh**. It is the tool for the connection to the cluster built on Atlas. [Download link](https://www.mongodb.com/products/shell).

### Connection string is used for connection from MongoSH

Log in Atlas, and go to the Database page, you may find a button "Connect" beside your cluster name. Here, mine is "Sandbox". Click on the button "Connect". And choose "Connect with MongoDB Shell" option.

![20220712021653](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712021653.png)

And then, choose "I have the MongoDB Shell installed", and the option "mongosh" from the dropdown list.

![20220712021842](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712021842.png)

When you finish the above selection, you may find the connection string generated at the lower part of the page.

![20220712022319](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712022319.png)

Copy the connection string from the page.

Open the command line terminal on your system.

![20220712022538](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712022538.png)

Enter the connection string after the command line prompt.

![20220712022904](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712022904.png)

Once connection completed, you may see the following information.

![20220712023816](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712023816.png)

## Commands

### Show current database (connected to)

**db**

![20220712024130](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712024130.png)

**\<tab\>** - Enter tab key to show all commands.

![20220712024333](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712024333.png)

**show dbs** - List all existed databases in the system.

![20220712024514](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712024514.png)

**use <database_name>** - Switch to the specified database.

![20220712024751](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712024751.png)

**show collections** - Show all collections that current database contains.

![20220712025051](D:\Workspace\knowledgebase\MongoDB_note.assets\20220712025051.png)
