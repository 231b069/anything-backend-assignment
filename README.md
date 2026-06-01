# Backend Developer Intern Assignment - Task Management API

This is a backend REST API built for the Backend Developer Intern Round-0 assignment.

The project provides user authentication and task management features using Node.js, Express.js, MongoDB, JWT, and Mongoose.

## Features

- User registration
- User login
- JWT based authentication
- Create task
- Get all tasks of logged-in user
- Get single task
- Update task
- Delete task
- Search tasks by title
- Filter tasks by status
- Error handling and validations

## Tech Stack

- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- JWT
- bcryptjs
- dotenv
- cors

## API Endpoints

### Auth Routes

| Method | Endpoint | Description |
|---|---|---|
| POST | /api/auth/register | Register a new user |
| POST | /api/auth/login | Login user |

### Task Routes

| Method | Endpoint | Description |
|---|---|---|
| POST | /api/tasks | Create a new task |
| GET | /api/tasks | Get all tasks |
| GET | /api/tasks/:id | Get a single task |
| PUT | /api/tasks/:id | Update a task |
| DELETE | /api/tasks/:id | Delete a task |

## Environment Variables

Create a .env file in the root directory:

PORT=5003
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret

## Installation and Setup

npm install
npm run dev

Server will run on:

http://localhost:5003

## Test User Flow

1. Register a user using /api/auth/register
2. Login using /api/auth/login
3. Copy the JWT token
4. Pass token in headers:

Authorization: Bearer YOUR_TOKEN

5. Access protected task routes

## Author

Aryan Swain
