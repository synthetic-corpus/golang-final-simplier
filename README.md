# golang-final-simplier

This Golang project is the capstone project for Udacity's Go Language course. It simulates a simple API that does CRUD requests against an API, and delivers a homepage when run.

Program is written as if it is in three layers, (API router, businesses logic layer, and database layer). The 'database' is struct with associated methods. However, it doesn't actually write to a database in this version. Future versions could expand on this struct to make an actual database connection.

This is the much simplier and easier to run version of the project. No docker file needed.

## To Run
Download this repo into your local directory, and run: 

go run main.go

App is is hard coded to run on port 3000, so all pathes should be accessible via localhost:3000

## What are the GET Paths?

- `GET /` *gets a homepage and is best opened from a browser*
- `GET /customers` *retrieves all current customers*
- `GET /customers/{id}` *retrieves a specific customer by primary key*
- `GET /hello` *As simple test reply comes back on this one*

## What are the POST, PATCH and DELETE paths pathes?

All paths for this project are 
- `PATCH or DELETE /customers/{id}` *use the id of the user to update or delete*
- `POST /customers` *use this path to post a new customer*

## What is the format of a POST or PATCH request body?

Ensure that you have the *Content-Type: application/json* header set.

The request body should look like this:

```json
{
    "Name": "A string value goes here",
    "Role": "A string value goes here",
    "Email": "A strong Value goes here",
    "Phone": "10 digit interger value goes here",
    "Contacted": "a boolean value goes here"
}
```
