 Build a rest api with flask
 * Project Overview :
 
This project demonstrates the development of a simple RESTful API using Python and Flask. The API performs basic CRUD (Create, Read, Update, Delete) operations to manage user data stored in memory.
The goal of this task is to understand API development fundamentals, HTTP methods, routing, and JSON request/response handling.
* Objective :
  
To create a REST API that:
Manages user data
Supports GET, POST, PUT, DELETE operations
Uses in-memory storage (dictionary)
Can be tested using Curl or Postman
*  Technologies Used :
  
Python
Flask
Curl / Postman (for testing)

* Project Structure :
flask_api to  app.py create files
app.py → Contains all API routes and logic.

* Features Implemented :
  ** GET /users
      --Returns all users stored in memory.
  ** GET /users/
      --Returns a specific user by ID.
  ** POST /users
      --Creates a new user.
      --Requires JSON input

**  PUT /users/
      --Updates an existing user.
**  DELETE /users/
      --Deletes a user by ID.
      
* How to Run the Application
**Install Flask:
-pip install flask

* Run the application:
-python app.py
-Server will start at:
-Copy code
-http://127.0.0.1:5000

* How to Test the API
  - Using Curl 
Example – Create User:
curl -X POST http://127.0.0.1:5000/users -H "Content-Type: application/json" -d "{\"name\":\"Veena\",\"email\":\"veena@gmail.com\"}"

* Using Postman
Select method (GET/POST/PUT/DELETE)
Enter URL
Choose Body → Raw → JSON (for POST/PUT)
Click Send

* Learning Outcomes
Through this project, the following concepts were understood:
REST API architecture
HTTP methods (GET, POST, PUT, DELETE)
JSON data handling
Flask routing
Request and response handling
Basic error handling
In-memory data storage
API testing tools

* Limitations :
Data is stored in memory (not persistent).
Data will reset when the server restarts.
Not suitable for production use.


* Future Improvements :
- Connect to a database (SQLite/MySQL)
- Add input validation
- Implement authentication
- Use Flask-RESTful
- Deploy to cloud platform

* Conclusion :
This project successfully demonstrates the fundamentals of building a REST API using Flask. It provides hands-on experience in handling HTTP requests, managing user data, and testing APIs.
