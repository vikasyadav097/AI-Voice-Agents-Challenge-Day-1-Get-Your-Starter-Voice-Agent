🚀 AI Voice Agents Challenge – Day 1 Complete

Welcome to Day 1 of my journey to build 10 AI Voice Agents in 10 Days using Murf Falcon, LiveKit Agents, Gemini, and Deepgram.

Today marks a major milestone — my first real-time AI Voice Agent is live and fully functional. 🔥

✅ Day 1 Achievements

I successfully completed the full foundational setup for the project:

🖥️ System Setup

Installed and configured: Python 3.11, Node.js, pnpm, uv

Downloaded and configured the LiveKit Server

🔗 End-to-End Integration

Built the backend with LiveKit Agents, Murf Falcon TTS, Gemini, Deepgram

Set up the Next.js frontend (React 19 + Tailwind)

Connected all layers: Backend → LiveKit → Frontend

Ran my first live, real-time voice conversation

Pushed everything to GitHub — the entire system now runs E2E 🎉

 ''' 📂 Project Structure
ten-days-of-voice-agents-2025/
├── backend/       # Python backend with LiveKit Agents + Murf Falcon TTS
├── frontend/      # Next.js 15 UI for real-time voice interaction
├── challenges/    # Daily challenge tasks and documentation
└── README.md
'''

🧠 Backend (Python – LiveKit Agents)

Powered by LiveKit’s agent framework with Murf Falcon integrated for ultra-fast TTS.

🚀 Features

LiveKit Agents with turn detection

Murf Falcon TTS – lightning fast voice output

Gemini for reasoning + conversational logic

Deepgram STT for accurate speech recognition

Noise reduction + echo cancellation

Detailed logs, metrics, and evaluation suite

Production-ready Dockerfile

🎨 Frontend (Next.js 15 + React 19)

Built from LiveKit’s starter template, optimized for real-time voice interaction.

✨ Features

Real-time, low-latency voice chat UI

Camera + screen share support

Live audio waveform visualizer

Light/Dark theming

Modular, customizable UI components

🚀 Quick Start Guide
1️⃣ Prerequisites

Install:

Python 3.11/3.12

uv → pip install uv

Node.js 18+ + pnpm → npm install -g pnpm

Download LiveKit Server from releases

🔑 Environment Variables

Add to .env.local in both backend and frontend:

MURF_API_KEY=
GOOGLE_API_KEY=
DEEPGRAM_API_KEY=

LIVEKIT_API_KEY=devkey
LIVEKIT_API_SECRET=secret
LIVEKIT_URL=ws://127.0.0.1:7880

🛠️ Backend Setup
cd backend
uv sync --python 3.11

# Copy environment
cp .env.example .env.local

# Download model files
uv run python src/agent.py download-files

🎨 Frontend Setup
cd frontend
pnpm install

# Add environment vars
echo LIVEKIT_API_KEY=devkey > .env.local
echo LIVEKIT_API_SECRET=secret >> .env.local
echo LIVEKIT_URL=ws://127.0.0.1:7880 >> .env.local

🛰️ Run LiveKit Server
Windows
.\livekit-server.exe --dev

Mac/Linux
./livekit-server --dev

▶️ Run the Full Application

Open 3 terminals:

Terminal 1 – LiveKit
./livekit-server --dev

Terminal 2 – Backend Agent
cd backend
.venv\Scripts\Activate.ps1   # Windows
python src/agent.py dev

Terminal 3 – Frontend
cd frontend
pnpm dev


Then open:
👉 http://localhost:3000

Your voice agent is now live and listening. 🎤🤖

📅 10-Day Challenge Timeline

Day 1 – Core Setup & First Agent ✔️

Day 2 – Coming soon…

Day 3 – Coming soon…

Day 4 – Coming soon…

Day 5 – Coming soon…

Day 6 – Coming soon…

Day 7 – Coming soon…

Day 8 – Coming soon…

Day 9 – Coming soon…

Day 10 – Coming soon…

📚 Resources

Murf Falcon TTS Docs

LiveKit Agents Documentation

LiveKit React Starter

Gemini API Docs

Deepgram API Docs

🛠️ Tech Stack Overview

Backend: Python, LiveKit Agents, Murf Falcon, Gemini, Deepgram
Frontend: Next.js 15, React 19, Tailwind
Real-Time Layer: LiveKit Server
Package Managers: uv, pnpm

🎉 Final Note

Day 1 sets the foundation for everything that comes next.
My goal with this challenge is simple:
👉 Learn fast, build fast, and ship powerful AI voice systems.

Buckle up — Day 2 drops soon. 🚀🔥
