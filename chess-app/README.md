# Chess AI Application

A full-stack Chess application where you can play against a Python-based AI agent.

## Features
- **Frontend**: React + Vite + Tailwind CSS
- **Backend**: FastAPI + python-chess
- **Engine**: Custom Minimax algorithm with Alpha-Beta pruning and positional evaluation.
- **Features**:
  - Play as White or Black.
  - Adjustable difficulty (Easy, Medium, Hard).
  - Move history log.
  - Engine thought process explanation.
  - Legal move validation.

## Project Structure
- `backend/`: Python FastAPI application.
- `frontend/`: React Vite application.

## Setup Instructions

### Prerequisites
- Python 3.8+
- Node.js 16+

### 1. Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   # Windows
   .\venv\Scripts\activate
   # Linux/Mac
   source venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the server:
   ```bash
   uvicorn main:app --reload --port 8000
   ```
   The API will be available at `http://localhost:8000`.

### 2. Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Run the development server:
   ```bash
   npm run dev
   ```
   The application will be available at `http://localhost:5173`.

## How to Play
1. Open the frontend URL in your browser.
2. The game starts automatically with you as White.
3. Click a piece to select it, then click a destination square to move.
4. The engine will think and reply.
5. Use the controls on the right to start a new game, switch sides, or change difficulty.

## Difficulty Levels
- **Easy**: Depth 2. Fast but makes mistakes.
- **Medium**: Depth 3. Reasonable play for casual players.
- **Hard**: Depth 4. Stronger tactical awareness.
