# API Endpoint Tables

### Legend

- **Public** — no authentication
- **Auth** — authenticated user
- **Admin** — elevated role

| Method | Endpoint | Access | Description |
|---|---|---|---|
| `POST` | `/api/auth/login` | Public | Authenticate a user |
| `GET` | `/api/resources` | Auth | List owned resources |
| `POST` | `/api/resources` | Auth | Create a resource |
| `DELETE` | `/api/resources/:id` | Auth | Delete an owned resource |

Document unusual status codes, pagination, filters, and ownership rules below the table.
