# golang-final-simplier

This is the much simplier and easier to run version of the project. No docker file needed.

## To Run
Download this repo into your local directory, and run: 

go run main.go

App is is hard coded to run on port 3000, so all pathes should be accessible via localhost:3000

## What GET Paths?

- GET / *gets a homepage and is best opend from a browser*
- GET /customers *retrieves all current customers*
- GET /customers/{id} *retrieves a specific customer by primary key*
- GET /hello *As simple test reply comes back on this one*

## What are the POST, PATCH and DELETE paths pathes?

All paths for this project are 
- PATCH or DELETE /customers/{id} *use the id of the user to update or delete*
- POST /customers *use this path to post a new customer*

## What is the format of a POST or PATCH request body?

Ensure that you have the *Content-Type: application/json* header set.

The request body should look like this:

```json
{
    "Name": "A string value goes here",
    "Role": "A string value goes here",
    "Email": "A strong Value goes here",
    "Phone": 10 digit interger value,
    "Contacted": boolean value
}
```
