# 🚀 AI Voice Agents Challenge – Day 1 (Completed)

This repository documents my journey of building **10 AI Voice Agents in 10 Days** using **Murf Falcon**, **LiveKit Agents**, **Google Gemini**, and **Deepgram**.

Day 1 is fully completed — including backend, frontend, and LiveKit server setup — with everything running end-to-end.

---

## ✅ **What I Achieved on Day 1**

* Installed & configured: **Python 3.11**, **Node.js**, **pnpm**, **uv**
* Fully set up the **Python backend** (LiveKit + Murf Falcon TTS + Gemini + Deepgram)
* Set up the **Next.js 15 frontend**
* Installed and configured the **LiveKit Server**
* Connected all layers: **Backend → LiveKit → Frontend**
* Successfully ran my first **real-time AI voice conversation**
* Pushed the complete project to GitHub

---

## 📂 **Repository Structure**

```
ten-days-of-voice-agents-2025/
├── backend/        # Python backend (LiveKit Agents + Murf Falcon TTS)
├── frontend/       # Next.js voice interface
├── challenges/     # Daily challenge tasks
└── README.md
```

---

## 🧠 **Backend (Python – LiveKit Agents)**

The backend is built using **LiveKit Agents** with full integration of:

* Murf Falcon (super-fast TTS)
* Google Gemini (LLM)
* Deepgram (speech recognition)
* Built-in turn detection
* Voice activity detection & noise reduction
* Complete logging & metrics
* Production-ready Dockerfile

---

## 🎨 **Frontend (Next.js 15 + React 19)**

The frontend is based on LiveKit’s starter UI.

### Features

* Real-time voice chat interface
* Camera & screen share support
* Audio waveform visualization
* Clean & customizable Tailwind UI
* Light/Dark mode

---

## 🚀 **Quick Start Guide**

### 1️⃣ **Prerequisites**

Install:

```sh
# Python
Python 3.11 or 3.12

# uv (Python package manager)
pip install uv

# Node + pnpm
npm install -g pnpm
```

Download **LiveKit Server** from GitHub Releases.

---

## 🔑 **Environment Variables**

Add these keys in **backend/.env.local** and **frontend/.env.local**:

```
MURF_API_KEY=your_key
GOOGLE_API_KEY=your_key
DEEPGRAM_API_KEY=your_key

LIVEKIT_API_KEY=devkey
LIVEKIT_API_SECRET=secret
LIVEKIT_URL=ws://127.0.0.1:7880
```

---

# 🛠️ **Backend Setup**

```sh
cd backend

# Install dependencies
uv sync --python 3.11

# Create local env file
copy .env.example .env.local

# Download model files
uv run python src/agent.py download-files
```

---

# 🎨 **Frontend Setup**

```sh
cd frontend

# Install packages
pnpm install

# Create environment file
copy .env.example .env.local
```

---

# 🛰️ **Run LiveKit Server**

### Windows

```sh
.\livekit-server.exe --dev
```

### Mac/Linux

```sh
./livekit-server --dev
```

---

# ▶️ **Running the Full System**

### **Terminal 1 – Start LiveKit**

```sh
./livekit-server --dev
```

### **Terminal 2 – Start Backend Agent**

```sh
cd backend
.venv\Scripts\Activate.ps1
python src/agent.py dev
```

### **Terminal 3 – Start Frontend**

```sh
cd frontend
pnpm dev
```

Open your browser:

👉 **[http://localhost:3000](http://localhost:3000)**
Your AI voice agent is now live! 🎤🤖

---

## 📅 **Challenge Progress**

| Day    | Status        |
| ------ | ------------- |
| Day 1  | ✔️ Completed  |

---

## 📚 **Useful Resources**

* Murf Falcon TTS Docs
* LiveKit Agents Documentation
* Gemini API Docs
* Deepgram API Docs
* Next.js 15 Docs

---

## 🛠️ **Tech Stack**

* **Backend**: Python, LiveKit Agents, Murf Falcon, Deepgram STT, Gemini
* **Frontend**: Next.js 15, React 19, Tailwind CSS
* **Real-time Layer**: LiveKit Server
* **Package Managers**: uv (Python), pnpm (Node)

---

## 🎉 **Final Note**

Day 1 is officially complete — the first AI voice agent is online and fully functional.
This challenge is focused on rapid experimentation, real-time AI, and building powerful voice-driven systems.

**Stay tuned for Day 2! 🚀**

---



