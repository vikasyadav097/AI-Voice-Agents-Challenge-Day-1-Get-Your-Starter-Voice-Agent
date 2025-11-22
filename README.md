🚀 AI Voice Agents Challenge – Day 1 Completed

Welcome to my journey of building 10 AI Voice Agents in 10 Days using Murf Falcon, LiveKit Agents, Gemini, and Deepgram.

This repository contains the complete codebase for Day 1, where I successfully set up and ran my first real-time AI Voice Agent.

✅ Day 1 – What I Completed

Installed and configured Python 3.11, Node.js, pnpm, uv

Set up the backend (LiveKit + Murf Falcon TTS + Gemini + Deepgram)

Set up the frontend (Next.js 15 + React 19 + Tailwind)

Downloaded and configured LiveKit Server

Connected all three layers: Backend → LiveKit → Frontend

Successfully ran my first live voice conversation

Pushed everything to GitHub

Project now runs fully end-to-end 🎉

📂 Repository Structure
ten-days-of-voice-agents-2025/
├── backend/       # Python backend with LiveKit + Murf Falcon TTS
├── frontend/      # Next.js UI for voice interaction
├── challenges/    # Daily challenge tasks
└── README.md

🧠 Backend (Python – LiveKit Agents)

The backend is based on LiveKit's template with Murf Falcon TTS integrated.

Features

LiveKit Agents + Turn Detection

Murf Falcon TTS (ultra-fast text-to-speech)

Gemini LLM for reasoning

Deepgram STT for speech recognition

Noise reduction, voice cancellation

Logging, metrics, evaluation suite

Production-ready Dockerfile

🎨 Frontend (Next.js 15 + React 19)

Built using LiveKit's starter React app.

Features

Real-time voice chat interface

Camera support

Screen share support

Audio visualization

Light/Dark mode

Fully customizable UI

🚀 Quick Start Guide
1️⃣ Prerequisites

Install:

Python 3.11 or 3.12

uv → pip install uv

Node.js 18+ + pnpm → npm install -g pnpm

LiveKit Server (download from GitHub releases)

🔑 Required API Keys

Add these inside backend and frontend .env.local:

MURF_API_KEY

GOOGLE_API_KEY

DEEPGRAM_API_KEY

LIVEKIT_API_KEY=devkey

LIVEKIT_API_SECRET=secret

LIVEKIT_URL=ws://127.0.0.1:7880

🛠️ Backend Setup
cd backend
uv sync --python 3.11

# Create .env.local
copy .env.example .env.local

# Download required model files
uv run python src/agent.py download-files

🎨 Frontend Setup
cd frontend
pnpm install

# Create .env.local
LIVEKIT_API_KEY=devkey
LIVEKIT_API_SECRET=secret
LIVEKIT_URL=ws://127.0.0.1:7880

🛰️ Run LiveKit Server

Windows:

.\livekit-server.exe --dev


Mac/Linux:

./livekit-server --dev

▶️ Running the Full Application

Open 3 terminals:

Terminal 1 – LiveKit
./livekit-server --dev

Terminal 2 – Backend Agent
cd backend
.venv\Scripts\Activate.ps1     # Windows
python src/agent.py dev

Terminal 3 – Frontend
cd frontend
pnpm dev


Open:
👉 http://localhost:3000

Your agent is now live! 🎤🤖

📅 Challenge Timeline

Day 1 – Starter Agent Setup ✔️

Day 2 – Coming soon

Day 3 – Coming soon

Day 4 – Coming soon

Day 5 – Coming soon

Day 6 – Coming soon

Day 7 – Coming soon

Day 8 – Coming soon

Day 9 – Coming soon

Day 10 – Coming soon

📚 Useful Resources

Murf Falcon TTS Docs

LiveKit Agents Docs

LiveKit Starter Templates

Gemini API Docs

Deepgram API Docs

🛠️ Tech Stack

Backend – Python, LiveKit Agents, Murf Falcon TTS, Deepgram STT, Gemini

Frontend – Next.js 15, React 19, Tailwind

Real-time – LiveKit Server

Package Managers – uv, pnpm

📄 License

This project uses MIT-licensed components from LiveKit, with additional integration of Murf Falcon TTS and custom features added for the challenge.

🎉 Final Note

This project marks the beginning of my 10 Days of AI Voice Agents challenge.
The goal is to learn, build fast, and create powerful voice-based AI systems.

Stay tuned for Day 2! 🚀