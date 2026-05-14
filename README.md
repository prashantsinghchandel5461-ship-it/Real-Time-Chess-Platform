# Real-Time-Chess-Platform
# Chess Game Application

A full-stack real-time Chess game application built with React, TypeScript, WebSockets, and Node.js.

This project allows two players to play chess in real time with move validation powered by `chess.js` and live communication using WebSockets.

---

## Features

* Real-time multiplayer chess gameplay
* WebSocket-based communication
* Legal move validation using `chess.js`
* Interactive chessboard UI
* Responsive frontend interface
* TypeScript support for both frontend and backend
* Modern React + Vite frontend setup
* Lightweight backend server using WebSockets

---

## Tech Stack

### Frontend

* React 19
* TypeScript
* Vite
* Tailwind CSS
* React Router DOM
* chess.js

### Backend

* Node.js
* TypeScript
* WebSocket (`ws`)
* chess.js

---

## Project Structure

```bash
chess-main/
│
├── backend/
│   ├── dist/                # Compiled backend files
│   ├── src/                 # Backend source code
│   ├── package.json
│   └── tsconfig.json
│
├── frontend/
│   ├── src/                 # React frontend source
│   ├── public/              # Static assets
│   ├── package.json
│   ├── vite.config.ts
│   └── tsconfig.json
│
└── README.md
```

---

## How It Works

1. Two players connect to the backend server.
2. WebSocket communication establishes a live game session.
3. Moves are validated using `chess.js`.
4. The game state updates instantly on both clients.
5. Players continue until checkmate, draw, or resignation.

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/your-username/chess-game.git
cd chess-main
```

---

## Backend Setup

### Navigate to Backend

```bash
cd backend
```

### Install Dependencies

```bash
npm install
```

### Compile TypeScript

```bash
npx tsc
```

### Start Backend Server

```bash
node dist/index.js
```

The backend server will run on:

```text
http://localhost:8080
```

---

## Frontend Setup

### Navigate to Frontend

```bash
cd frontend
```

### Install Dependencies

```bash
npm install
```

### Start Development Server

```bash
npm run dev
```

The frontend will run on:

```text
http://localhost:5173
```

---

## Available Scripts

### Frontend

| Command           | Description                   |
| ----------------- | ----------------------------- |
| `npm run dev`     | Start Vite development server |
| `npm run build`   | Build frontend for production |
| `npm run preview` | Preview production build      |
| `npm run lint`    | Run ESLint                    |

### Backend

| Command              | Description                |
| -------------------- | -------------------------- |
| `npx tsc`            | Compile TypeScript backend |
| `node dist/index.js` | Start backend server       |

---

## WebSocket Communication

The backend uses WebSockets for real-time communication between players.

### Example Events

* Player connected
* Match created
* Move played
* Game updated
* Checkmate detected
* Player disconnected

---

## Chess Rules Engine

The application uses `chess.js` for:

* Move validation
* Turn management
* Check/checkmate detection
* Draw detection
* FEN generation
* PGN support

---

## Build for Production

### Frontend

```bash
npm run build
```

### Backend

```bash
npx tsc
```

---

## Future Improvements

* Matchmaking system
* User authentication
* Spectator mode
* Chess clock / timers
* Game history and replay
* AI opponent integration
* Online ranking system
* Mobile optimization
* Chat functionality

---

## Screenshots

Add screenshots here:

```text
frontend/public/screenshots/
```

Suggested screenshots:

* Home screen
* Chessboard UI
* Matchmaking screen
* Game result screen

---

## Deployment

### Frontend

Deploy easily using:

* Vercel
* Netlify
* GitHub Pages

### Backend

Deploy using:

* Render
* Railway
* VPS / Docker
* AWS / DigitalOcean

---

## Docker Support (Optional)

Example Docker build:

```bash
docker build -t chess-game .
```

Run container:

```bash
docker run -p 5173:5173 -p 8080:8080 chess-game
```

---

## Contributing

Contributions are welcome.

### Steps

1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Push changes
5. Open a pull request

---

## License

This project is licensed under the MIT License.

---

## Author

Developed with ❤️ using React, TypeScript, and WebSockets.
