# Mini Task Manager Backend

This is a simple backend API for a Mini Task Manager application. It provides endpoints to manage tasks using an in-memory array (no database required).

## Features

- Create, read, update, and delete tasks
- Simple RESTful API design
- No authentication required
- CORS enabled for frontend integration

## Tech Stack

- Node.js
- Express.js

## Getting Started

### Prerequisites

- Node.js (v14+)

### Installation

```bash
git clone https://github.com/yourusername/mini-task-manager-backend.git
cd mini-task-manager-backend
npm install
```

### Running the Server

```bash
node index.js
```

The server will start on [http://localhost:8000](http://localhost:8000).

## API Endpoints

| Method | Endpoint      | Description              |
|--------|---------------|--------------------------|
| GET    | /tasks        | Get all tasks            |
| POST   | /tasks        | Create a new task        |
| PUT    | /tasks/:id    | Update a task by ID      |
| DELETE | /tasks/:id    | Delete a task by ID      |

## Notes

- Tasks are stored in memory and will be lost when the server restarts.
- Each task has `id`, `title`, `description`, and `completed` fields.

## Known Limitations

- No persistent storage: All data is lost when the server restarts.
- Not suitable for production use.
- No authentication or authorization implemented.
- Not scalable for large numbers of tasks or concurrent users.

## License

MIT
