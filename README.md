# NestJS API

This exercise aims to demonstrate the ability to create a functioning REST API using NestJS and MongoDB.

## Subject
Build a REST API for the student list app using the NestJS framework and MongoDB database. 

The backend database shall contain at least 3 lists:
- user list,
- student list,
- exam list.

There should be 2 types of users: 
- teachers,
- administrators.

Teachers are allowed to create/read/update/delete students and assign exams to a student. 

Administrators are allowed to create/read/update/delete users and exams. 

Users need to be authenticated and authorized to access API.

Students can have zero or many exams assigned.  

Enrolled students count shall be returned together with exam data. 

## Requirements
* Use JWT for Authentication (preferred).
* Use DTO and ValidationPipes for mandatory fields validation in Incomming Requests.
* Use modules, services, controllers, and NestJS dependency injection while structuring your application.
* Use Swagger to document routes.
* Mongoose is our prefered way to work with MongoDB.
* Make sure your code is well typed with Typescript.


## Tech Stack

- NestJS
- Typescript
- Mongoose
- Mongo DB
- Swagger
- Jest

