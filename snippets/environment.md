# Environment Variable Snippets

## Required and Optional Groups

```env
# Required
DATABASE_URL=
APPLICATION_SECRET=

# Optional integrations
REDIS_URL=
EXTERNAL_API_KEY=

# Runtime behavior
ENVIRONMENT=development
LOG_LEVEL=INFO
```

## Documentation Table

| Variable | Required | Scope | Description |
|---|---:|---|---|
| `DATABASE_URL` | Yes | Backend | Primary database connection |
| `APPLICATION_SECRET` | Yes | Backend | Token or session signing secret |
| `REDIS_URL` | No | Backend | Optional cache connection |
| `VITE_API_URL` | Yes | Frontend | Public API base URL |

Never place backend secrets in browser-exposed variables.
