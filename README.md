# InterviewMirror AI

AI-powered mock interview platform — realistic AI interviewers, adaptive questions, live performance analysis (confidence, clarity, structure, specificity), and presence tracking (eye contact, posture, tone) via voice and camera.

## Stack

- **Client** — React + Vite (`client/`)
- **Server** — Node.js + Express + MongoDB (`server/`)
- AI question generation and evaluation via Gemini

## Project structure

```
IM AI/
├── client/     # React/Vite frontend
└── server/     # Express backend + MongoDB models/routes
```

## Setup

```bash
cd "IM AI/server" && npm install && cp .env.example .env   # fill in MONGO_URI, JWT_SECRET, GEMINI_API_KEY
cd "IM AI/client" && npm install
```

Run both dev servers (client on Vite's port, server on `PORT` from `.env`, default 5000).

## Features

- Guest and registered-user auth (JWT), role-based mock interviews across 10+ domains
- Adaptive AI interviewer personas with configurable difficulty and pressure mode
- Live voice answer capture (STT/TTS) with real-time analysis feed
- Resume/job-description-aware question generation
- Session history, PDF export, and performance dashboards
