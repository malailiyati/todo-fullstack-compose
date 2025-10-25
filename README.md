# 🐳 Todo App – Fullstack (Docker Compose)

This repository contains the **Docker Compose setup** for running both the frontend and backend of the Industrix Todo Application.

## 📁 Repository Structure

```
todo-fullstack/
├── todo-frontend/          # React + Ant Design frontend
├── todo-backend/           # Go + Gin + PostgreSQL backend
├── docker-compose.yml      # Compose configuration
└── README.md
```

## 🛠️ Tech Stack

### Frontend

- React
- Ant Design
- Vite

### Backend

- Go
- Gin Framework
- PostgreSQL

## 📋 Prerequisites

Before running this application, make sure you have installed:

- [Docker](https://docs.docker.com/get-docker/) (version 20.10 or higher)
- [Docker Compose](https://docs.docker.com/compose/install/) (version 2.0 or higher)
- Git

## 🚀 How to Run

### 1️⃣ Clone all repositories

```bash
git clone https://github.com/malailiyati/todo-fullstack
cd todo-fullstack
git clone https://github.com/malailiyati/todo-frontend
git clone https://github.com/malailiyati/todo-backend
```

### 2️⃣ Run with Docker Compose

```bash
docker compose up -d --build
```

Or run in foreground mode (to see logs directly):

```bash
docker compose up --build
```

### 3️⃣ Access the application

- **Frontend**: [http://localhost:5173](http://localhost:5173)
- **Backend API**: [http://localhost:8080](http://localhost:8080)

## 🛑 Stopping the Application

To stop all running containers:

```bash
docker compose down
```

To stop and remove all data (including database volumes):

```bash
docker compose down -v
```

## 🔧 Development

### View Logs

```bash
# All services
docker compose logs -f

# Specific service
docker compose logs -f frontend
docker compose logs -f backend
```

### Rebuild Services

```bash
docker compose up --build --force-recreate
```

## 📝 API Documentation

The backend API endpoints are available at `http://localhost:8080`. Common endpoints include:

- `GET /api/todos` - Get all todos
- `POST /api/todos` - Create a new todo
- `PUT /api/todos/:id` - Update a todo
- `DELETE /api/todos/:id` - Delete a todo

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature`)
3. Commit your changes (`git commit -m 'Add some Feature'`)
4. Push to the branch (`git push origin feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

## 👤 Author

**Malailiyati**

- 🔗 [LinkedIn](https://www.linkedin.com/in/ma-la-iliyati)
