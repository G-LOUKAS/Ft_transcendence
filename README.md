# 🎮 ft_transcendence: Multiplayer Game Platform

**ft_transcendence** is the final project of the 42 Common Core — a full-stack web application built using modern technologies. Our version focuses on **real-time multiplayer gaming**, including a classic **Ping Pong** game and a strategic **Tic Tac Toe** game, both playable online with matchmaking and real-time interactions.

## 🌍 Tech Stack

- 🧠 **Backend**: Django + Django Channels (WebSocket support)
- 💻 **Frontend**: HTML/CSS + Tailwind + JavaScript
- 🧩 **Games**: Ping Pong & Tic Tac Toe (Canvas & WebSocket-based)
- 🔐 **Authentication**: JWT + 2FA with Google Authenticator
- 🎮 **Live Play**: Matchmaking, spectators, real-time updates
- 🧠 **Database**: PostgreSQL + Redis for game states & queues
- 🐳 **Deployment**: Dockerized & NGINX reverse proxy

## 🕹️ Games Implemented

### 🏓 Ping Pong (Pong Classic)
- 1v1 real-time game with keyboard controls
- Matchmaking system for random opponents
- Spectator mode with live updates
- Tournaments and scoreboards

### ❌⭕ Tic Tac Toe
- Classic 3x3 grid game (PvP or vs Bot)
- Random matchmaking with timeouts
- Realtime interactions over WebSockets
- History and replay system

## 🧰 Features

- 🔒 Secure login with OAuth & optional 2FA
- 🧑‍🤝‍🧑 Friend system and chat (public/private)
- 🧾 Match history tracking
- 🏆 Leaderboard and rankings
- 🎮 Live matchmaking engine using Redis

## 📁 Project Structure

```
ft_transcendence/
├── backend/
│   ├── api/               # Django views, models, game logic
│   ├── websocket/         # Channels routing & consumers
│   └── games/             # Game logic: pingpong & tictactoe
├── frontend/
│   ├── templates/         # HTML templates
│   ├── static/            # TailwindCSS, JS, game canvas
│   └── js/                # WebSocket handlers
├── nginx/
├── docker-compose.yml
└── README.md
```

## 🧪 How to Run

1. **Clone and configure**:
   ```bash
   git clone https://github.com/yourusername/ft_transcendence.git
   cd ft_transcendence
   cp .env.example .env
   ```

2. **Run it with Docker**:
   ```bash
   docker-compose up --build
   ```

3. **Open in browser**:
   - App: `http://localhost`
   - Admin: `http://localhost/admin/`

## 🧠 What We Learned

- Handling **asynchronous events** with WebSockets
- Implementing **game state machines** and matchmaking queues
- Real-time communication with **Redis Pub/Sub**
- Building secure, scalable full-stack apps
- Designing a **clean UI/UX** with Tailwind CSS

## 🎯 Conclusion

This project combined our skills in software engineering, systems design, and front-end development to create a cohesive multiplayer gaming platform. With two fully implemented games and real-time capabilities, ft_transcendence is both a technical challenge and a showcase of collaborative development.

