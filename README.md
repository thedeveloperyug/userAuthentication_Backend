Installation
To install the project, follow these steps:

Clone the repository
Install dependencies: 
# npm install

Connect MongoDB by pasting your URL:
# Mongo URL 

Usage
To run the project, use the following command:
# npm run dev

APIs Available
The following APIs are available:

../api/users
../api/contacts
You can access the APIs using the following format: http://localhost:5001/api/<endpoint>

<hr>
Register a New User
To register a new user, use the following API:
API: ../api/users/register
Method: POST
JSON Data:
{
  "username":"test",
  "email" : "test@gmail.com",
  "password":"test123"
}

<hr>

User Login
To log in as a user, use the following API:
API: ../api/users/login
Method: POST
JSON Data:
{
  "email" : "test@gmail.com",
  "password":"test123"
}

Output: You'll get an Access token copy that token.


<hr>

Getting Users Data
To get users' data, use the following API:
API: ../api/contacts/
Method: GET
Send request with token that you copied:
Thunder Client -> Auth -> Bearer -> (paste the token)

<hr>

Creating Users Data
To create a new user data, use the following API:
API: ../api/contacts/
Method: POST
Send request with JSON and token that you copied:
Thunder Client -> Auth -> Bearer -> (paste the token)
JSON Data:
{
  "username":"testdata",
  "email" : "testdata@gmail.com",
  "phone":"6734567890"
}

<hr>

Updating Users Data
To update a user data, use the following API:
API: ../api/contacts/_id
Replace _id with the unique_id of the user you want to update.
Method: PUT
Send request with JSON and token that you copied:
Thunder Client -> Auth -> Bearer -> (paste the token)
JSON Data:
{
  "username":"testdataupdated",
  "email" : "testdatav1@gmail.com",
  "phone":"9034567890"
}

<hr>

Deleting Users Data
To delete a user data, use the following API:
API: ../api/contacts/_id
Replace _id with the unique_id of the user you want to delete.
Method: DELETE
Send request with token that you copied:
Thunder Client -> Auth -> Bearer -> (paste the token)
