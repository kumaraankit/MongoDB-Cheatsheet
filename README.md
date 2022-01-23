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

**Insert** the data using the below command
db.databasename.insert({"name":"Ankit"})

![image](https://user-images.githubusercontent.com/64415303/150676752-4d5a3100-e42b-4b53-8691-609cdd77581c.png)

**Dropping the database**

db.dropDatabase()

**Create Collection**

![image](https://user-images.githubusercontent.com/64415303/150676925-c9143c51-877b-410b-9c47-39f06656805f.png)

**Drop Collection**

![image](https://user-images.githubusercontent.com/64415303/150677016-e7e0873c-f02f-45a2-8001-1a6dd738fff6.png)

**Insert the document in the collection**

![image](https://user-images.githubusercontent.com/64415303/150677272-bc6b86ee-a15c-4a1d-b21a-28175cc74f65.png)

**The insertOne() method**

If you need to insert only one document into a collection you can use this method.

db.COLLECTION_NAME.insertOne(document)

**The insertMany() method**

You can insert multiple documents using the insertMany() method. To this method you need to pass an array of documents.

**The find() Method**

**Get all the data from the document using find()**

![image](https://user-images.githubusercontent.com/64415303/150677415-f2d82896-67e5-424b-8748-8127ab8e88b7.png)

**The pretty() Method**

To display the results in a formatted way, use pretty() method.
**
**The findOne() method****
returns only one document.

![image](https://user-images.githubusercontent.com/64415303/150677593-c91768cb-a1a3-4afc-9998-a8857d5872bc.png)

**Update() Method**

The update() method updates the values in document.

![image](https://user-images.githubusercontent.com/64415303/150678748-ec0ff12f-6979-4ebe-9198-0b0deecd966d.png)

**Note**: By default, MongoDB will update only a single document. To update multiple documents, We need to set a parameter 'multi' to true.



