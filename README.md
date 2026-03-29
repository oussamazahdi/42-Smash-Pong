# 42 Smash Pong

A full-stack web application built as part of the 42 curriculum — featuring real-time multiplayer Pong, live chat, and user management.

---

## Stack

| Layer | Technology |
|---|---|
| Frontend | Next.js |
| Backend | Node.js |
| Database | SQLite |
| Real-time | WebSocket |
| Reverse Proxy | Nginx |
| Containerization | Docker |
| Build | Makefile |

---

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/) and Docker Compose installed
- `make` available on your system

### Run the project

```bash
make
```

This will build and start all containers. The app will be available at:

```
https://localhost
```

### Stop the project

```bash
make down
```

### Clean up

```bash
make clean      # Stop containers and remove volumes
make fclean     # Full clean including images
make re         # Rebuild everything from scratch
```

---

## Project Structure

```
smash_pong/
├── frontend/        # Next.js app
├── backend/         # Node.js API & WebSocket server
├── nginx/           # Nginx configuration
├── docker-compose.yml
└── Makefile
```

---

## Features

- 🏓 Real-time multiplayer Pong (WebSocket)
- 💬 Live chat rooms
- 👤 User authentication & profiles
- 🏆 Match history & leaderboard
- 🔒 Secure — served over HTTPS via Nginx

---

## Environment Variables

Copy `.env.example` to `.env` and fill in the required values before running:

```bash
cp .env.example .env
```

---

## Authors

Made with ☕ at 42.
