# TeamUp

Real-time collaboration platform where users can discover, join, and contribute to team-based tech projects by roles/stacks.

## ✨ Highlights
- Real-time presence, teams, and roles
- Drag-and-drop flows for onboarding & tasks (React Flow)
- REST API for teams, roles, invites, and activity feed
- Designed for 100+ concurrent users (MVP target)

## 🧱 Tech Stack (MVP)
**Frontend:** React, React Flow, Vite, TypeScript  
**Backend:** FastAPI (Python), Uvicorn  
**Realtime & Cache:** Redis (pub/sub)  
**DB (start simple):** PostgreSQL  
**Auth (MVP):** Email magic links (placeholder)  
**Infra (later):** Docker, Docker Compose

## 🗺️ Architecture (planned)
```mermaid
flowchart LR
  A[React + React Flow] -- REST/WebSocket --> B(FastAPI)
  B -- pub/sub --> C[Redis]
  B -- SQL --> D[(PostgreSQL)]
  B <-- logs --> E[Logging/Monitoring (to add)]

## 📂 Planned Structure

/frontend   # React + React Flow
/backend    # FastAPI app
/docs       # screenshots, diagrams
