# HungerVerse AI — Intelligent Zero Hunger Platform

> **An AI-powered food redistribution operating system** that connects surplus food to hungry communities in real-time using Digital Twin city modeling, Hidden Hunger Detection, and Food Genome Intelligence.

![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-active-brightgreen)
![SDG](https://img.shields.io/badge/UN%20SDG-%232%20Zero%20Hunger-orange)

---

## 🌍 Mission

**ಹಸಿವು ಇಲ್ಲದ ನಾಳೆ** — *A hunger-free tomorrow.*

Every day, tonnes of edible food are wasted while millions go hungry. HungerVerse AI solves this by using a multi-agent AI pipeline to intelligently detect, match, and route surplus food to the communities that need it most — in real time.

---

## ✨ Features

| Feature | Description |
|---|---|
| 🌆 **Digital Twin Hunger City** | Interactive Leaflet.js map showing live food sources, hunger hotspots, and volunteer routes |
| 🧬 **Food Genome Intelligence** | AI analyzes food nutrition, shelf-life, and urgency upon upload |
| 🤖 **Multi-Agent AI Pipeline** | 5 specialized agents for intake, spatial mapping, hunger detection, matching, and dispatch |
| 🔍 **Hidden Hunger Detection** | Identifies at-risk communities using alternative signals (school absenteeism, labour camps, health data) |
| 📊 **Real-Time Impact Dashboard** | Live metrics, activity feed, and weekly trend charts |
| 🏆 **Volunteer Leaderboard** | Gamified impact tracking with AI-verified delivery scores |
| 🔮 **Predictive AI Insights** | 7-day demand forecasting to pre-position food resources |
| 🚨 **Emergency SOS** | One-click broadcast to all nearby volunteers |
| 🤝 **NGO Partner Portal** | NGO registration, active partner table, and quick food request form |

---

## 🗂️ Project Structure

```
hungerverse-ai/
├── frontend/
│   ├── index.html      # Main SPA entry point
│   ├── styles.css      # Glassmorphism design system
│   └── script.js       # Core logic, Leaflet map, AI simulations, Geolocation
├── backend/
│   ├── app.py          # Flask API Gateway (7 endpoints)
│   ├── agents.py       # Multi-Agent AI logic
│   └── requirements.txt
├── serve.ps1           # PowerShell static file server (Windows)
└── README.md
```

---

## 🚀 Quick Start

### Option 1: Frontend Only (No install needed)

Open `frontend/index.html` directly in your browser. All CDN dependencies load automatically.

> **Note:** The live location feature works best when served over HTTP (not `file://`). Use Option 2 for the full experience.

### Option 2: Serve Locally (Windows — Recommended)

```powershell
# In the project root directory:
powershell -ExecutionPolicy Bypass -File serve.ps1
```

Then visit **`http://localhost:3000/`** in your browser.

### Option 3: Run with Backend API

```bash
# Install dependencies
pip install -r backend/requirements.txt

# Start Flask API
python backend/app.py
# API runs at http://localhost:5000
```

---

## 🤖 AI Agent Architecture

```
User Input
    │
    ▼
[Agent 1: Food Scanner]   ── NLP extraction, Food Genome Profile
    │
    ▼
[Agent 2: City Twin]      ── Spatial mapping onto Digital Twin
    │
    ▼
[Agent 3: Hunger Detector]── Hidden hotspot scoring & ranking
    │
    ▼
[Agent 4: Nutrition Allocator]── Scientific food-to-need matching
    │
    ▼
[Agent 5: Dispatch Coordinator]── Volunteer routing & logistics
    │
    ▼
Outcome → [Feedback Loop] → Updates Agent 3 model
```

---

## 🌐 Backend API Reference

| Method | Endpoint | Description |
|---|---|---|
| `POST` | `/api/upload` | Upload food, triggers Genome Analysis |
| `GET` | `/api/nodes` | Get hunger zone hotspots |
| `POST` | `/api/match_food` | AI match food to best zone |
| `POST` | `/api/dispatch` | Dispatch volunteer with route |
| `GET` | `/api/impact` | Live impact statistics |
| `GET` | `/api/run_scenario/<A/B/C>` | Trigger demo scenario |

---

## 🛠️ Tech Stack

**Frontend:** HTML5, CSS3 (Glassmorphism), Vanilla ES6+ JavaScript, Leaflet.js, Font Awesome

**Backend:** Python 3, Flask, Flask-CORS

**AI/Logic:** Multi-agent pipeline with rule-based NLP, Haversine routing, urgency scoring

**Design:** Dark mode, glassmorphism cards, particle physics background, micro-animations

---

## 🌱 Roadmap

- [ ] Connect to live PostgreSQL / Firebase database
- [ ] Google Maps / Mapbox integration for real routing
- [ ] User authentication (NGO / Volunteer / Admin roles)
- [ ] WhatsApp community tip integration
- [ ] ML model for predictive demand forecasting
- [ ] Deploy on Vercel / Railway / AWS

---

## 📄 License

This project is licensed under the **MIT License** — see [LICENSE](LICENSE) for details.

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first.

---

*Built with ❤️ for Zero Hunger — Aligned with [UN SDG #2](https://sdgs.un.org/goals/goal2)*
