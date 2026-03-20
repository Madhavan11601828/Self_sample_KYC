# KYC Automation — Agentic AI

End-to-end KYC workflow for Bengaluru East: document verification → biometric → sanctions screening → risk scoring → human-in-the-loop case management.

## Stack
- **Backend**: Python 3.11 + FastAPI + SQLAlchemy async + Alembic (managed with `uv`)
- **Frontend**: React 18 + Vite + TypeScript + Tailwind CSS
- **Agent**: LangGraph + Claude (Module 9)

## Quick Start

### Backend
```bash
cd backend
uv venv --python 3.11
uv pip install -e ".[dev]"
cp .env.example .env
uv run uvicorn app.main:app --reload --port 8000
```

### Frontend
```bash
cd frontend
npm install
npm run dev        # http://localhost:5173
```

### Tests
```bash
cd backend
uv run pytest -v
```

## Module Status
| # | Module | Status |
|---|--------|--------|
| 1 | Project Scaffold & Infrastructure | ✅ Complete |
| 2 | Customer Onboarding & Data Capture | Pending |
| 3 | Document Authenticity & OCR | Pending |
| 4 | Biometric Liveness & Face Match | Pending |
| 5 | Identity Enrichment | Pending |
| 6 | Sanctions / PEP Screening | Pending |
| 7 | Adverse Media Screening | Pending |
| 8 | Risk Scoring & Decision Engine | Pending |
| 9 | Agentic Orchestration (LangGraph) | Pending |
| 10 | Case Management & Human Review UI | Pending |
| 11 | Final Outcome & Notifications | Pending |
| 12 | Auth, Rate Limiting & Production | Pending |

## API Docs
With backend running: http://localhost:8000/docs
