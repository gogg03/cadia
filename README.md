# Cadia - Circadian Rhythm Sleep Optimization App

Cadia is a self-hosted web application designed to optimize sleep patterns using natural circadian rhythms, solar/lunar cycles, and environmental factors.

## Project Structure

```
cadia/
├── frontend/          # React + Vite + TypeScript frontend
├── backend/           # Node.js + Express + TypeScript API
├── docker/            # Docker configuration files
├── docs/              # Documentation and deployment guides
├── memory-bank/       # Project documentation and design docs
└── .cursor/           # Cursor IDE rules and configuration
```

## Tech Stack

- **Frontend**: React, Vite, TypeScript, Tailwind CSS, PWA
- **Backend**: Node.js, Express, TypeScript, MongoDB
- **DevOps**: Docker, Docker Compose, Nginx, PM2
- **Hosting**: Ubuntu Server, Let's Encrypt, UFW, Fail2Ban
- **Monitoring**: Uptime Kuma, Netdata

## Prerequisites

- Node.js (v18 or later)
- Docker and Docker Compose
- MongoDB (local or Docker)
- Git

## Development Setup

### 1. Clone the Repository

```bash
git clone <repository-url>
cd cadia
```

### 2. Install Frontend Dependencies

```bash
cd frontend
npm install
```

### 3. Install Backend Dependencies

```bash
cd ../backend
npm install
```

### 4. Environment Configuration

Create `.env` files in both frontend and backend directories:

**Backend `.env**:**
```env
NODE_ENV=development
PORT=3001
MONGODB_URI=mongodb://localhost:27017/cadia
```

**Frontend `.env**:**
```env
VITE_API_URL=http://localhost:3001/api
```

### 5. Development Commands

**Frontend Development:**
```bash
cd frontend
npm run dev          # Start development server
npm run build        # Build for production
npm run lint         # Run ESLint
npm run format       # Format code with Prettier
```

**Backend Development:**
```bash
cd backend
npm run dev          # Start development server with hot reload
npm run build        # Build TypeScript to JavaScript
npm run start        # Start production server
npm run lint         # Run ESLint
npm run format       # Format code with Prettier
```

## Docker Development

Use Docker Compose for local development with all services:

```bash
docker-compose up -d
```

This will start:
- Frontend (React app)
- Backend (Express API)
- MongoDB database
- Nginx reverse proxy

## Production Deployment

See the [Implementation Plan](memory-bank/Implementation-plan.md) for detailed deployment instructions.

## Documentation

- [App Design Document](memory-bank/app-design-document.md) - Application design and user experience
- [Tech Stack](memory-bank/Tech-stack.md) - Technology choices and architecture
- [Implementation Plan](memory-bank/Implementation-plan.md) - Detailed development roadmap
- [Progress Tracking](progress.md) - Development progress and milestones

## Contributing

1. Read the development guidelines in `.cursor/rules/`
2. Follow the implementation plan phases
3. Update documentation when adding features
4. Run linting and formatting before committing

## License

This project is private and not licensed for public use.
