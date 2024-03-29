# MongoDB Learning Notes

July 12, 2022

*The document has not been completed yet. It will be gradually improved along with my learning going deeply.*
The note bases on MongoDB version 5.0

## Content
- [MongoDB Cloud Platform - Atlas](#mongodb-cloud-platform---atlas)
- [MongoDB Shell](#mongodb-shell)
- [Commands in the Shell](#commands-in-the-shell)

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

![20220712021653](./MongoDB_note.assets/20220712021653.png)

And then, choose "I have the MongoDB Shell installed", and the option "mongosh" from the dropdown list.

![20220712021842](./MongoDB_note.assets/20220712021842.png)

When you finish the above selection, you may find the connection string generated at the lower part of the page.

![20220712022319](./MongoDB_note.assets/20220712022319.png)

Copy the connection string from the page.

Open the command line terminal on your system.

![20220712022538](./MongoDB_note.assets/20220712022538.png)

Enter the connection string after the command line prompt.

![20220712022904](./MongoDB_note.assets/20220712022904.png)

Once connection completed, you may see the following information.

![20220712023816](./MongoDB_note.assets/20220712023816.png)

## Commands in the Shell

- **db** - is to show current connected database.

![20220712024130](./MongoDB_note.assets/20220712024130.png)

- **\<tab\>** - enter the Tab key to show all commands available in the Shell.

![20220712024333](./MongoDB_note.assets/20220712024333.png)

- **show dbs** - list all databases existed in the system.

![20220712024514](./MongoDB_note.assets/20220712024514.png)

- **use **<database_name> - switch to the database specified by \<database_name\>, and make it as the current database.

![20220712024751](./MongoDB_note.assets/20220712024751.png)

- **show collections** - show all collections that current database holds.

![20220712025051](./MongoDB_note.assets/20220712025051.png)

- **db.**\<collection_name\>**.find({**\<criteria\>**})** - find document(s) within the specified collection by criteria in the current database. For example, to find all qualified documents stored in the collection **zips**.

![20220712232325](MongoDB_note.assets/20220712232325.png)

- **db.**\<collection_name\>**.findOne()** - show one document randomly stored in the collection.
- **db.**\<collection_name\>**.find({**\<criteria\>**}).pretty()** - show query result in a JSON style.
- **db.**\<collection_name\>**.find({**\<criteria\>**}).count()** - count all qualified documents queried by the criteria.

![20220712233227](MongoDB_note.assets/20220712233227.png)

- 

## Features and Matters need attention

- `_id` property with a collection-unique value. Every MongoDB document must have a `_id` property, and its value must be unique within the whole collection.
- You can omit the `_id` property when you insert a new document into the collection. MongoDB will generate one for you automatically.
- 