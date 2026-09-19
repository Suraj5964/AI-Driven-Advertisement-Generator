# AI-Driven Advertisement Generator

A full-stack web application that generates professional advertisement copy using AI.

## Stack
- Frontend: React + Vite
- Backend: Node.js + Express
- AI: OpenAI-compatible API (optional)
- Styling: Plain CSS

## Features
- Product/service input form
- Target audience, tone, platform and offer selection
- AI-generated headline, primary ad copy, CTA, hashtags and campaign idea
- Demo/fallback mode works without an API key
- Copy-to-clipboard buttons
- Responsive modern dashboard

## Run

### 1. Backend
```bash
cd backend
npm install
```

Create `.env` from `.env.example` and add your API key if you want live AI generation.

```bash
npm run dev
```

Backend runs on http://localhost:5000

### 2. Frontend
Open a second terminal:
```bash
cd frontend
npm install
npm run dev
```

Open the URL shown by Vite, normally http://localhost:5173.

## AI configuration
The backend accepts an OpenAI-compatible endpoint.

`.env`:
```env
PORT=5000
AI_API_KEY=your_api_key
AI_BASE_URL=https://api.openai.com/v1
AI_MODEL=gpt-4o-mini
```

If `AI_API_KEY` is empty, the app automatically uses a local demo generator, so the project still runs for presentations.

## Project structure
```
AI-Driven-Advertisement-Generator/
├── backend/
│   ├── package.json
│   ├── .env.example
│   └── server.js
├── frontend/
│   ├── package.json
│   ├── index.html
│   └── src/
│       ├── main.jsx
│       ├── App.jsx
│       └── styles.css
└── README.md
```
