# AI Chat Assistant

A conversational AI workspace for developers and everyday tasks.

## Architecture
- **Frontend:** React + Vite
- **Backend:** Node.js + Express
- **Database:** MongoDB Atlas + Mongoose (optional but supported)
- **AI:** OpenAI-compatible server-side integration
- **Deployment:** Vercel

## Features
- Responsive premium AI workspace
- Server-side AI requests through `/api/ai`
- MongoDB persistence when `MONGODB_URI` is configured
- Environment-based secrets
- Production Vite build
- Vercel configuration

## Local setup
```bash
npm install
npm run dev
```

For the AI API in local development, deploy the `api` directory through Vercel or run it with a Node adapter. The frontend is intentionally separated from provider credentials.

## Environment variables
Copy `.env.example` and configure:
- `OPENAI_API_KEY`
- `OPENAI_MODEL` (optional)
- `MONGODB_URI` (optional)

**Never commit API keys.**

## Vercel
Import this repository into Vercel, keep the default Vite build settings or use the included `vercel.json`, and add environment variables in the Vercel dashboard.
