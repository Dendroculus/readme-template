<div align="center">

  EN | [YOUR_LANGUAGE](./docs/translation/README_YOUR_LANGUAGE.md) | [YOUR_LANGUAGE](./docs/translation/README_YOUR_LANGUAGE.md)
</div>

<p align="center">
  <img src="https://img.shields.io/badge/Node.js-{{NODE_VERSION}}-43853D?logo=node.js&logoColor=white" alt="Node.js">
  <img src="https://img.shields.io/badge/Express-{{EXPRESS_VERSION}}-000000?logo=express&logoColor=white" alt="Express">
  <img src="https://img.shields.io/badge/React-{{REACT_VERSION}}-61DAFB?logo=react&logoColor=white" alt="React">
  <img src="https://img.shields.io/badge/Vite-{{VITE_VERSION}}-646CFF?logo=vite&logoColor=white" alt="Vite">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white" alt="PostgreSQL">
</p>

<p align="center" style="margin-top: -12px;">
  <img src="https://img.shields.io/badge/{{CSS_FRAMEWORK}}-06B6D4?logo=tailwind-css&logoColor=white" alt="{{CSS_FRAMEWORK}}">
  <img src="https://img.shields.io/badge/License-{{LICENSE_NAME}}-22C55E?logo=opensourceinitiative&logoColor=white" alt="{{LICENSE_NAME}}">
</p>

<div align="center">

# ✨ {{PROJECT_NAME}}
### {{PROJECT_SUBTITLE}}
</div>

## 🚀 Why {{PROJECT_NAME}}

<div style="max-width: 720px;">

{{PROJECT_DESCRIPTION}}

</div>

<br>

- ⚡ {{HIGHLIGHT_1}}  
- 🔐 {{HIGHLIGHT_2}}  
- 📊 {{HIGHLIGHT_3}}  
- 🎨 {{HIGHLIGHT_4}}  
- 🛠️ {{HIGHLIGHT_5}}  

## 🎯 Features

### A) Core Features

1. {{CORE_FEATURE_1}}  
2. {{CORE_FEATURE_2}}  
3. {{CORE_FEATURE_3}}  
4. {{CORE_FEATURE_4}}  
5. {{CORE_FEATURE_5}}  

### B) Platform & System Capabilities

6. {{SYSTEM_FEATURE_1}}  
7. {{SYSTEM_FEATURE_2}}  
8. {{SYSTEM_FEATURE_3}}  
9. {{SYSTEM_FEATURE_4}}  
10. {{SYSTEM_FEATURE_5}}  

## 🔴 Real-Time Implementation

{{REALTIME_DESCRIPTION}}

### Live Use Cases

1. **{{REALTIME_CASE_1_TITLE}}**  
   {{REALTIME_CASE_1_DESCRIPTION}}

2. **{{REALTIME_CASE_2_TITLE}}**  
   {{REALTIME_CASE_2_DESCRIPTION}}

3. **{{REALTIME_CASE_3_TITLE}}**  
   {{REALTIME_CASE_3_DESCRIPTION}}

### Realtime Architecture

```txt
Backend service action
→ event publisher
→ realtime transport
→ WebSocket server
→ authenticated client rooms
→ frontend provider
→ event-specific listeners
→ UI state updates
```

## 🧠 Architecture Highlights

- Split frontend and backend responsibilities  
- REST API follows controller → service → model separation  
- Database stores transactional and relational business data  
- Authentication protects user and admin-only routes  
- Reusable hooks, services, and UI components keep pages clean  
- {{ARCHITECTURE_POINT_1}}  
- {{ARCHITECTURE_POINT_2}}  

## 💡 Design Considerations

- {{DESIGN_CONSIDERATION_1}}  
- {{DESIGN_CONSIDERATION_2}}  
- {{DESIGN_CONSIDERATION_3}}  
- {{DESIGN_CONSIDERATION_4}}  

## 🔧 Processing Models

### 🔄 Server-Side Flow

1. {{SERVER_FLOW_1}}  
2. {{SERVER_FLOW_2}}  
3. {{SERVER_FLOW_3}}  
4. {{SERVER_FLOW_4}}  

### ⚡ Client-Side Flow

1. {{CLIENT_FLOW_1}}  
2. {{CLIENT_FLOW_2}}  
3. {{CLIENT_FLOW_3}}  
4. {{CLIENT_FLOW_4}}  

## 🏗️ Architecture & Stack

<div style="max-width: 760px; line-height: 1.65;">

- **Frontend ({{FRONTEND_STACK}})** — {{FRONTEND_DESCRIPTION}}

- **Backend ({{BACKEND_STACK}})** — {{BACKEND_DESCRIPTION}}

- **Database ({{DATABASE_STACK}})** — {{DATABASE_DESCRIPTION}}

</div>

## 📦 Main Dependencies

### Frontend

- {{FRONTEND_DEPENDENCY_1}}
- {{FRONTEND_DEPENDENCY_2}}
- {{FRONTEND_DEPENDENCY_3}}

### Backend

- {{BACKEND_DEPENDENCY_1}}
- {{BACKEND_DEPENDENCY_2}}
- {{BACKEND_DEPENDENCY_3}}

## 📁 Project Structure

```txt
{{PROJECT_STRUCTURE}}
```
## ⚙️ Environment Variables

### Backend (`backend/.env`)

Use either individual database variables or a single database URL, depending on how your backend config is written.

#### Option A: Individual database variables

```env
DB_NAME=your_database_name
DB_USER=your_database_user
DB_PASSWORD=your_database_password
DB_HOST=127.0.0.1
DB_DIALECT=postgres
```

#### Option B: Single database URL

```env
DATABASE_URL=postgres://user:password@localhost:5432/database_name
```

> Only use `DATABASE_URL` if your backend actually reads it from the environment.

### Frontend (`frontend/.env`)

```env
BASE_URL=http://localhost:3000
VITE_API_URL=http://localhost:3000/api
VITE_DEBUG_MODE=true
```

For production, do not use `localhost`. Use the deployed backend URL instead.

## 🚀 Local Development

### 1. Clone

```bash
git clone {{REPOSITORY_URL}}
cd {{REPOSITORY_FOLDER}}
```

### 2. Prepare Database

```sql
CREATE DATABASE {{DATABASE_NAME}};
```

### 3. Run Backend

```bash
cd backend
npm install
{{BACKEND_SETUP_COMMAND}}
npm run dev
```

### 4. Run Frontend

```bash
cd frontend
npm install
npm run dev
```

## 🧰 Useful Scripts

### Backend

```bash
npm run dev
npm run lint
npm run lint:fix
```

### Frontend

```bash
npm run dev
npm run build
npm run preview
npm run test
npm run lint
npm run lint:fix
```

## 🔒 Security Notes

- JWT authentication is used for protected routes  
- Admin-only routes use authentication and role authorization middleware  
- Passwords are hashed before storage  
- Environment variables are used for secrets and database credentials  
- Never commit real `.env` files or production secrets  

## 🗄️ Database Schema

### 📊 Entity Relationship Diagram

<div align="center">
  <img src="{{ERD_IMAGE_PATH}}" alt="ERD Diagram" width="700" style="max-width: 100%; height: auto;">
</div>

## 📚 API Endpoints

### Legend

- **Public** — no login required  
- **Auth** — login required  
- **Admin** — admin role required  

{{API_ENDPOINT_TABLES}}

## 🧪 Testing & Quality

```bash
{{TEST_COMMANDS}}
```

## 🤝 Contributing

PRs and improvements are welcome.

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Open a Pull Request

## 📜 License

Licensed under the {{LICENSE_NAME}} License. See [LICENSE](./LICENSE) for details.

## 🙏 Acknowledgements

- {{ACKNOWLEDGEMENT_1}}
- {{ACKNOWLEDGEMENT_2}}
- Open-source contributors and libraries used

## 👤 Contributors

{{CONTRIBUTORS_TABLE}}
