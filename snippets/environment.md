# Environment Variables Snippet

## Full-Stack Web App

````md
## ⚙️ Environment Variables

### Backend (`backend/.env`)

```env
NODE_ENV=development
PORT=3000

DB_NAME={{DATABASE_NAME}}
DB_USER={{DATABASE_USER}}
DB_PASSWORD={{DATABASE_PASSWORD}}
DB_HOST=127.0.0.1
DB_DIALECT=postgres

JWT_SECRET={{JWT_SECRET}}

BASE_URL=http://localhost:3000
API_URL=http://localhost:3000/api
```

### Frontend (`frontend/.env`)

```env
BASE_URL=http://localhost:3000
VITE_API_URL=http://localhost:3000/api
VITE_DEBUG_MODE=true
```

For production, do not use `localhost`. Use the deployed backend URL instead.
````

## AI Full-Stack App

````md
## ⚙️ Environment Variables

### Backend

```env
DATABASE_URL=
ALLOWED_ORIGINS=
CLOUDFLARE_TURNSTILE_SITE_KEY=
CLOUDFLARE_TURNSTILE_SECRET_KEY=
AZURE_CONNECTION_STRING=
REPLICATE_API_TOKEN=
ENVIRONMENT=development
```

### Frontend

```env
VITE_API_BASE_URL=http://127.0.0.1:8000/api
VITE_TURNSTILE_SITE_KEY=
```
````

## Discord Bot

````md
## ⚙️ Environment Variables

```env
DISCORD_TOKEN=
DATABASE_URL=
AZURE_CONNECTION_STRING=
```
````
