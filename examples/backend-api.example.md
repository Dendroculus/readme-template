# Task Ownership API

A small authenticated JSON API where users can create tasks and may only read, update, or delete their own records.

## Capabilities

- Register and login
- JWT bearer authentication
- Password hashing
- User-owned task CRUD
- Structured success and error responses
- Automatic development schema setup

## Endpoints

| Method | Endpoint | Access | Description |
|---|---|---|---|
| `POST` | `/api/auth/register` | Public | Create an account |
| `POST` | `/api/auth/login` | Public | Return a JWT |
| `GET` | `/api/tasks` | Auth | List the caller's tasks |
| `POST` | `/api/tasks` | Auth | Create a task |
| `PUT` | `/api/tasks/:id` | Auth | Update an owned task |
| `DELETE` | `/api/tasks/:id` | Auth | Delete an owned task |

## Request Flow

```text
Bearer token
→ authentication middleware
→ validated controller input
→ ownership-aware service
→ Sequelize model
→ JSON response
```

## Environment

```env
PORT=3000
DB_HOST=127.0.0.1
DB_NAME=task_api
DB_USER=root
DB_PASSWORD=
JWT_SECRET=replace_me
```

## Run

```bash
npm install
npm run setup
npm run dev
```
