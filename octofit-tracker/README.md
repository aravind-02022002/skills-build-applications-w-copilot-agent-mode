# 🐙 OctoFit Tracker

A modern multi-tier fitness tracking application built with GitHub Copilot Agent Mode.

## Project Structure

```
octofit-tracker/
├── frontend/          # React 19 + Vite application
│   ├── src/
│   ├── package.json
│   ├── vite.config.ts
│   └── tsconfig.json
└── backend/           # Node.js + Express + TypeScript API
    ├── src/
    ├── package.json
    └── tsconfig.json
```

## Technology Stack

### Frontend
- **React 19**: Latest React with modern features
- **Vite**: Lightning-fast build tool
- **TypeScript**: Type-safe development
- **Port**: 5173

### Backend
- **Node.js**: JavaScript runtime
- **Express**: Web framework
- **TypeScript**: Type-safe development
- **Mongoose**: MongoDB object modeling
- **Port**: 8000

### Database
- **MongoDB**: NoSQL database
- **Port**: 27017

## Getting Started

### Prerequisites
- Node.js (v18 or higher)
- MongoDB running locally or accessible via connection string
- npm or yarn package manager

### Installation

#### Backend Setup
```bash
cd octofit-tracker/backend
npm install
cp .env.example .env
npm run build
npm run dev
```

#### Frontend Setup
```bash
cd octofit-tracker/frontend
npm install
npm run dev
```

The frontend will be available at `http://localhost:5173` and will proxy API calls to the backend at `http://localhost:8000`.

## Available Scripts

### Backend
- `npm run dev` - Start development server with hot reload
- `npm run build` - Build TypeScript to JavaScript
- `npm start` - Run compiled backend

### Frontend
- `npm run dev` - Start Vite development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build

## API Endpoints

- `GET /api/health` - Health check endpoint

## Environment Variables

Backend environment variables are managed in `.env` file. See `.env.example` for available options.

## Development Notes

- The frontend dev server automatically proxies `/api/*` requests to the backend
- MongoDB should be running on `localhost:27017` (or configured via MONGODB_URI)
- Both frontend and backend use TypeScript for type safety

---

Built with ❤️ using GitHub Copilot Agent Mode
