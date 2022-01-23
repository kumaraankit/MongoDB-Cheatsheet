# MongoDB-Cheatsheet

MongoDB is an open-source document database and leading NoSQL database. MongoDB is written in C++.

MongoDB is a cross-platform, document oriented database that provides, high performance, high availability, and easy scalability. MongoDB works on concept of collection and document.

**Database**
Database is a physical container for collections. Each database gets its own set of files on the file system. A single MongoDB server typically has multiple databases.

**Collection**
Collection is a group of MongoDB documents. It is the equivalent of an RDBMS table. Collections do not enforce a schema. Documents within a collection can have different fields.

**Document**
A document is a set of key-value pairs. Documents have dynamic schema. Dynamic schema means that documents in the same collection do not need to have the same set of fields or structure, and common fields in a collection's documents may hold different types of data.

**Advantages of MongoDB**


**Start the MongoDB**

Navigate to the application file and move to bin folder, from there just run the command mongod.exe in cmd. once thi starts then again execute mongod in the cmd, one > will come where we can start typing our code in mongodb.

db.help()   ------> to get the help with list of commands.

db.stats() -------> to check the status of the database.

![image](https://user-images.githubusercontent.com/64415303/150676582-b09770a6-7e8d-462a-ba65-1be370816a64.png)


Create database

use nameOfTheDatabase
![image](https://user-images.githubusercontent.com/64415303/150676438-e4f818fd-f07c-45e2-a983-da4c5b130a28.png)

show dbs ----------> it will show all the available databases.

**Note**: If nothing is inserted in the database then it wont show the name if we execute command "show dbs".

Insert the data using the below command
db.databasename.insert({"name":"Ankit"})

![image](https://user-images.githubusercontent.com/64415303/150676752-4d5a3100-e42b-4b53-8691-609cdd77581c.png)

