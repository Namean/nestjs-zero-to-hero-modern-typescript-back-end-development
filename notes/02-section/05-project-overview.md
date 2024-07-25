# NestJS Zero to Hero - Modern TypeScript Back-end Development
## Task Management Application (REST API)


## 5. Project Overview

Task Management Application


AppModule (root)

TasksModule
 - TaskController
 - TaskService
 - Status validationPipe
 - TaskEntity
 - TaskRepository
 - ... (a few more things)


We're going to have an isolated module for tasks then we'll have an auth module


AuthModule: Handling authentication and authorization
 - AuthController
 - AuthService
 - UserEntity: How we'll represent users in a database
 - UserRepository: Manages transactions and interactions with out database
 - JWTStrategy: Implementation of JSON Web Tokens, built into NestJS
 - ...: A few more things




API Endpoints - Tasks
<!-- [theasciicode.com](https://theasciicode.com.ar/extended-ascii-code/box-drawing-character-single-line-lower-left-corner-ascii-code-192.html) -->
┌--------------------------------------------------------┐
| Endpoint          | Method |         Description       |
|-------------------|--------|---------------------------|
| tasks/            | GET    | Get tasks (incl. filters) |
| tasks/:id         | GET    | Get a task                |
| tasks/            | POST   | Create a task             |
| tasks/:id/        | DELETE | Delete a task             |
| tasks/:id/status/ | PATCH  | Update task status        |
└--------------------------------------------------------┘

┌-------------------------------------┐
| Endpoint     | Method | Description |
|--------------|--------|-------------|
| auth/signup/ | POST   | Sign up     |
| auth/signin/ | POST   | Sign in     |
└-------------------------------------┘


Objectives: NestJS


- NestJS Modules
- NestJS Controllers
- NestJS Services and Providers
- Controller-to-Service communication
- Validation using NestJS Pipes


Objectives: Back-end & Architecture

- Develop production-ready REST APIs: Develop production-ready REST APIs
- CRUD operations (Create, Read, Update, Delete): Learn what CRUD operations are, and how to implement them.
- Error handling: How to handle our errors
- Data Transfer Objects (DTO): What are they and how to use them
- System modularity: Learn to develop modular systems
- Back-end development best practices: General backend best practices
- Configuration Management: How to manage configuration for different environments
- Logging: Learn how to log things properly so that we have a useful way to understand where things are going wrong.
- Security best practices: Apply security best practices in terms of storing passwords


Objectives: Persistence

- Connecting the application to a database
- Working with relational databases
- Using TypeORM
- Writing simple and complex queries using QueryBuilder
- Performance when working with a database


On the first part of the course we're going to use a Postgres database. On the GraphQL (i.e. second) part we're going
to be using MongoDB.

- Work with relation databases using TypeORM, which allows us to interact wit our database.
- Learn how to write simple and complex queries using the QueryBuilder of TypeORM
- How to tackle performance when working with a database



Objectives: Authorization/Authentication

- Signing up, singing in: The difference between authorization and authentication
- How to develop protected resources: Certain things should only be accessed by signed in users.
- How to apply ownership of tasks by certain users
- Using JWT: A common standard for authentication between front-end and back-end systems, especially useful in microservices
- Learn password hashing salts in a database how to properly store passwords in a database



Objectives: Deployment

- Polishing the application for production use
- Deploying NestJS apps to AWS (Amazon Web Services)
- Deploying front-end application to Amazon S3
- Wiring up the front-end and back-end


Bonus: Front-end Application

> Fully-featured front-end application that consumes the API we are developing throughout the course, for your own use.
