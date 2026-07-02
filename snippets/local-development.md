# Local Development Snippet

## Full-Stack Web App

````md
## 🚀 Local Development

### 1. Clone

```bash
git clone {{REPOSITORY_URL}}
cd {{REPOSITORY_FOLDER}}
```

### 2. Run Backend

```bash
cd backend
npm install
npm run setup
npm run dev
```

### 3. Run Frontend

```bash
cd frontend
npm install
npm run dev
```
````

## AI Full-Stack App

````md
## 🚀 Local Development

### 1. Run Backend

```bash
cd backend
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
```

### 2. Run Frontend

```bash
cd frontend
npm install
npm run dev
```
````

## Discord Bot

````md
## 🚀 Local Development

```bash
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
python bot.py
```

If the project uses a worker, run it in a second terminal:

```bash
python worker.py
```
````
