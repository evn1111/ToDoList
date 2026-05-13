# To-Do App

Full-stack To-Do application with Go backend, React frontend, and PostgreSQL.

## Stack

- Go
- Gin
- React
- PostgreSQL
- Docker Compose

## Features

- Create tasks
- Edit tasks
- Delete tasks

## Project Structure

- `backend/` - Go API server
- `frontend/` - React client
- `docker-compose.yml` - local multi-container setup

## Run Locally

Prerequisites:

- Go 1.22+
- Node.js 18+
- npm

Backend:

```bash
cd backend
go run ./cmd/app
```

Frontend:

```bash
cd frontend
npm install
npm start
```

Frontend will be available at `http://localhost:3000`.

## Run With Docker

Prerequisites:

- Docker
- Docker Compose

```bash
docker compose up --build
```

## Environment

Main environment variables are stored in `.env` and used by `docker-compose.yml`.

Typical values include:

- backend and frontend container names
- database connection settings
- API base path for frontend proxy
