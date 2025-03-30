# TutorSama

A full-stack application with AdonisJS backend, React frontend, and PostgreSQL database.

## Architecture

This application uses Docker to containerize the following components:

- **Backend**: AdonisJS application
- **Frontend**: Vite + React application
- **Database**: PostgreSQL
- **Nginx**: Reverse proxy that routes `/api` requests to the backend and all other requests to the frontend

## Getting Started

### Prerequisites

- Docker and Docker Compose

### Setup

1. Clone this repository
2. Set up the backend (AdonisJS)
   ```bash
   cd backend
   # Initialize AdonisJS project
   npm init adonis-ts-app@latest .
   ```

3. Set up the frontend (Vite + React)
   ```bash
   cd ../frontend
   # Create a new Vite + React project
   npm create vite@latest . -- --template react
   ```

4. Start the application
   ```bash
   docker-compose up -d
   ```

5. Access the application at http://localhost

## Development

- Backend API is available at http://localhost/api
- Frontend is available at http://localhost
- Database is accessible within the Docker network

## Environment Variables

See the `.env` file for configurable environment variables.
