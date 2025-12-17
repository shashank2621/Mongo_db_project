# Mongo_db_project
# backend_mongodb
Mongodb is a backend which stores the data in the cloud server
For mongodb it goes from mongoatlas, compass which gets connected to the vscode

1. *Import MongoDB Client*  
   The script begins by importing the MongoClient class from the mongodb package, which is used to interact with MongoDB.

2. *Define Connection URI*  
   It sets up a connection string (uri) to connect to a MongoDB Atlas cluster using the provided username and password.

3. **Define an Async Function main()**  
   The core logic is wrapped inside an asynchronous function called main() to handle asynchronous database operations.

4. *Create a MongoDB Client Instance*  
   A new MongoClient object is created using the connection URI.

5. *Connect to MongoDB Atlas*  
   The script attempts to connect to the MongoDB Atlas cluster. If successful, it logs "Connected to Atlas".

6. *Access Database and Collection*  
   It accesses the school database and the students collection within that database.

7. *CREATE Operation*  
   A new document { name: "Alex", age: 22, marks: 12 } is inserted into the students collection. A message "Inserted one document." is logged.

8. *READ Operation*  
   All documents in the students collection are retrieved using find().toArray() and printed to the console.

9. *UPDATE Operation*  
   The document with name: "Alex" is updated to change the marks field from 12 to 10. A message "Updated one document." is logged.

10. *DELETE Operation (Commented Out)*  
   The code includes a commented-out line that would delete a document with name: "Dev" if uncommented.

11. *Error Handling*  
   If any error occurs during the operations, it is caught and logged with the message "Error:" followed by the error details.

12. *Close Connection*  
   Whether successful or not, the script ensures the MongoDB client connection is closed at the end and logs "Connection closed."

13. *Execute the Function*  
   Finally, the main() function is called to run the entire sequence.
