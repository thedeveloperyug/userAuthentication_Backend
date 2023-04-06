## Steps to run the project
To run the project, follow these steps:

Clone the repository
Install dependencies: 
# npm install

Connect MongoDB by pasting your URL:
# Mongo URL 
(Don't forget to add your current IP Address in MongoDB)</br>
Usage:</br>
To run the project, use the following command:
# npm run dev

APIs Available
The following APIs are available:

../api/users
../api/contacts
</br>
You can access the APIs using the following format: http://localhost:5001/api/<endpoint>

<hr>
Register a New User </br>
To register a new user, use the following API:</br>
API: ../api/users/register</br>
Method: POST</br>
JSON Data:</br>
{
  "username":"test",
  "email" : "test@gmail.com",
  "password":"test123"
}

<hr>

User Login </br>
To log in as a user, use the following API: </br>
API: ../api/users/login </br>
Method: POST </br>
JSON Data: </br>
{
  "email" : "test@gmail.com",
  "password":"test123"
}
</br>
Output: You'll get an Access token copy that token.
</br>

<hr>

Getting Users Data  </br> 
To get users' data, use the following API:  </br>
API: ../api/contacts/  </br>
Method: GET   </br>
Send request with token that you copied:   </br>
Thunder Client -> Auth -> Bearer -> (paste the token)   </br>

<hr>

Creating Users Data </br>
To create a new user data, use the following API: </br>
API: ../api/contacts/ </br>
Method: POST </br>
Send request with JSON and token that you copied: </br>
Thunder Client -> Auth -> Bearer -> (paste the token) </br>
JSON Data: </br>
{
  "name":"testdata",
  "email" : "testdata@gmail.com",
  "phone":"6734567890"
}

<hr>

Updating Users Data </br>
To update a user data, use the following API: </br>
API: ../api/contacts/_id </br>
Replace _id with the unique_id of the user you want to update. </br>
Method: PUT </br>
Send request with JSON and token that you copied: </br>
Thunder Client -> Auth -> Bearer -> (paste the token) </br>
JSON Data: </br>
{
  "username":"testdataupdated",
  "email" : "testdatav1@gmail.com",
  "phone":"9034567890"
}

<hr>

Deleting Users Data </br>
To delete a user data, use the following API: </br>
API: ../api/contacts/_id </br>
Replace _id with the unique_id of the user you want to delete. </br>
Method: DELETE </br>
Send request with token that you copied: </br>
Thunder Client -> Auth -> Bearer -> (paste the token) </br>
