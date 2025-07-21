# RESR-API--Flask
# Flask REST API - User Management

This is a simple REST API built with Flask, Flask-RESTful, and Flask-SQLAlchemy.  
It manages user data with endpoints to create, read, update, and delete users.

## Features

- Store users in a SQLite database (`database.db`)
- RESTful endpoints for users
- Input validation with `reqparse`
- Response serialization with `marshal_with`

## Technologies

- Python 3.x
- Flask
- Flask-RESTful
- Flask-SQLAlchemy
- SQLite

## Installation & Running

1. Clone the repo or copy the code.
2. Create a virtual environment (optional but recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   
API ENDPOINTS
Method  	Endpoint	        Description
GET	     /api/users	      Get all users
POST	   /api/users	      Create new user
GET	     /api/users/<id>	Get user by ID
PATCH	   /api/users/<id>	Update user by ID
DELETE	 /api/users/<id>	Delete user by ID

Sample Requests
Get all users:

bash
Copy code
GET /api/users
Create user:

json

POST /api/users
{
  "name": "Alice",
  "email": "alice@example.com"
}
Update user:

json

PATCH /api/users/1
{
  "name": "Alice Updated",
  "email": "alice_updated@example.com"
}
##mini guide##
use flask to create endpoint 
store user in a dictonary or in memory list 
