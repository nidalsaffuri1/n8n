# Full-Stack To-Do App

A full-stack to-do application with user authentication and MongoDB persistence. Built with React (frontend), Express/Node.js (backend), and MongoDB (database), and containerized with Docker for deployment.

## Features
- User registration and login
- Add/edit/remove to-do items
- Mark tasks complete
- Filter tasks by status
- JWT authentication
- Responsive React UI
- RESTful API with Express
- Docker Compose for deployment

## Project Structure
- `frontend/` - React application
- `backend/` - Express server API
- `docker-compose.yml` - Defines services (frontend, backend, MongoDB)

## Getting Started

### Prerequisites
- Docker and Docker Compose installed

### Environment Variables
Create a `.env` file in `backend/`:

PORT=5000
MONGODB_URI=mongodb://mongo:27017/tododb
JWT_SECRET=your_jwt_secret
NODE_ENV=production


### Build and Run

docker-compose up --build


- Frontend: http://localhost:3000
- Backend API: http://localhost:5000

## Deployment
Deploy to AWS EC2 instance using Docker Compose and optionally manage infrastructure with Terraform.

## API Endpoints
- POST `/api/auth/register`
- POST `/api/auth/login`
- GET `/api/todos`
- POST `/api/todos`
- PUT `/api/todos/:id`
- DELETE `/api/todos/:id`

## License
MIT License