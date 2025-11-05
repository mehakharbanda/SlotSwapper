# SlotSwapper

SlotSwapper is a peer-to-peer time-slot scheduling application that allows users to mark busy calendar slots as **swappable** and exchange them with others.  
This project demonstrates full-stack development skills across authentication, database design, API logic, and frontend state management.

---

##  Tech Stack

**Frontend:** React (Vite)  
**Backend:** Node.js, Express, MongoDB, JWT Authentication  
**Containerization:** Docker + Docker Compose  
**Database:** MongoDB (via official Docker image)

---

## Core Features

- **User Authentication** — Secure signup/login using JWT  
- **Event Management** — Create and update calendar events (BUSY / SWAPPABLE / PENDING)  
- **Swap Requests** — Request, accept, or reject time-slot swaps  
- **Marketplace View** — Browse available swappable slots from other users  
- **State Updates** — Reflect accepted/rejected swaps dynamically  
- **Dockerized Setup** — One-command run for full stack

---

##  Setup Instructions

### Option 1: Run with Docker (Recommended)
```bash
git clone https://github.com/<your-username>/slotswapper.git
cd slotswapper
docker-compose up --build

---

### Option 2: Manual Setup

Backend

cd backend
cp .env.example .env
npm install
npm start


Frontend

cd frontend
npm install
npm run dev

---

### Folder Structure
slotswapper/
├── backend/
│   ├── src/
│   │   └── server.js
│   ├── Dockerfile
│   ├── .env.example
│   └── package.json
├── frontend/
│   ├── src/
│   │   └── main.jsx
│   ├── index.html
│   └── package.json
├── docker-compose.yml
└── README.md

---

### Future Enhancements

- **Real-time swap notifications (Socket.IO)

- **Unit tests for swap logic

- **Full calendar UI integration

- **Deployment to Render (backend) & Vercel (frontend)
