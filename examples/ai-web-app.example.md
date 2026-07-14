<div align="center">

# ✨ ForgeStudio

### A hybrid image platform combining asynchronous AI processing with instant browser tools

</div>

## 🚀 Why ForgeStudio

ForgeStudio began as an image upscaler and grew into a broader image workspace. Expensive AI operations run through a controlled backend pipeline, while lightweight transformations stay in the browser for immediate feedback.

## 🎯 Features

### AI tools

- Image upscaling
- Background removal
- Color restoration
- Object removal

### Browser tools

- Resize, crop, rotate, and flip
- Compression and format conversion
- Metadata removal
- Color-palette extraction
- Watermarking

### Platform capabilities

- Turnstile verification
- Per-feature usage limits
- Queue capacity control
- Direct storage uploads
- Status polling
- Session restoration
- Signed result URLs
- Automatic retention cleanup

## 🧠 Architecture Highlights

- React owns previews, local transforms, and session restoration
- FastAPI owns secure job orchestration and validation
- AI providers are hidden behind a provider interface
- PostgreSQL stores usage and job state
- Object storage holds temporary inputs and results
- Cleanup removes expired artifacts

## 🔄 AI Processing Flow

1. Browser validates the input
2. Backend verifies anti-bot and usage rules
3. Browser uploads directly with signed metadata
4. Backend creates and queues the job
5. Provider executes the model
6. Client polls status
7. Result becomes available through a controlled URL
8. Retention cleanup removes expired data

## 🏗️ Project Structure

```text
forgestudio/
├── backend/
│   ├── app/
│   ├── providers/
│   ├── services/
│   └── tests/
├── frontend/
│   └── src/
│       ├── components/
│       ├── hooks/
│       ├── pages/
│       └── services/
└── docs/
```

## ⚙️ Environment Variables

```env
DATABASE_URL=
STORAGE_CONNECTION_STRING=
AI_PROVIDER_TOKEN=
TURNSTILE_SECRET=
ALLOWED_ORIGINS=http://localhost:5173
```

## 🧪 Quality

```bash
ruff check backend
pytest backend
npm --prefix frontend run lint
npm --prefix frontend run build
```

## 🛡️ Reliability and Security

Inputs are validated before expensive processing, provider calls have explicit timeouts, queue capacity prevents overload, and cleanup is safe to rerun.
