# NestJS API

This exercise aims to demonstrate the ability to create a functioning REST API using NestJS and MongoDB.

## Subject
Build a REST API for the student list app using the NestJS framework and MongoDB database. 

The backend database shall contain at least 3 lists:
- user list (id, userName, passwordHash, and any other fields that may be required ),
- student list (id, firstName, lastName, and any other fields that may be required),
- exam list (id, name, and any other fields that may be required).

There should be 2 types of users: 
- teachers,
- administrators.

Teachers are allowed to create/read/update/delete students and assign exams to a student. 

Administrators are allowed to create/read/update/delete users and exams. 

Users need to be authenticated and authorized to access API.

Students can have zero or many exams assigned.  

Enrolled students count shall be returned together with exam data. 

### Routes

Please implement the following routes:

1. Login user with user name and password, should return JWT token

```
POST  /login
```

2. Student List:
- Create One (payload firstName (mandatory), lastName)
- Get One by Id
- Get All
- Update one (payload firstName, lastName. Only changing values shall be provided )
- Delete
- Assign exam (parameter userId, payload examId)

```
POST  /student
GET   /student/:studentId
GET   /student
PATCH /student/:studentId
DEL   /student/:studentId
POST  /student/assign-exam/:studentId
```

3 Exam List.
- Create exam (payload examName (mandatory))
- get One exam
- get All exams
```
POST  /exam
GET   /exam/:examId
GET   /exam
```

4 User List.
- Create user (payload userName, user password)
- Get One user
```
POST /user
GET  /user/:userId
```
*Do not forget about accss rights*
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

