#  SkillSync Pro

##  Overview

SkillSync Pro is a full-stack web application that bridges the gap between job seekers' resumes and employer requirements using advanced NLP analysis.

##  Features

-  **Dynamic Skill Gap Analysis** - Extract and compare skills using NLP
-  **AI-Powered Recommendations** - Get relevant skill suggestions
-  **Match Percentage** - See how well you match the job requirements
-  **Modern UI** - Clean, responsive interface built with React and Tailwind CSS
-  **Fast API** - High-performance backend with FastAPI
-  **CI/CD Pipeline** - Automated testing and deployment

## 🛠️ Tech Stack

### Backend
- **FastAPI** - Modern, fast web framework for building APIs
- **Python 3.11** - Programming language
- **Pydantic** - Data validation using Python type annotations
- **pytest** - Testing framework
- **Docker** - Containerization

### Frontend
- **React 18** - UI library
- **TypeScript** - Type-safe JavaScript
- **Vite** - Build tool
- **Tailwind CSS** - Utility-first CSS framework
- **Zustand** - State management
- **Vitest** - Testing framework

### DevOps
- **GitHub Actions** - CI/CD pipeline
- **Render** - Backend hosting
- **Vercel** - Frontend hosting
- **Docker** - Containerization

##  Getting Started

### Prerequisites

- Python 3.11+
- Node.js 18+
- Docker (optional)

### Local Development

#### Backend Setup

```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
pip install -r requirements-dev.txt  # For development
uvicorn app.main:app --reload
```
Backend will be available at http://localhost:8000

#### Frontend Setup
```bash
cd frontend
npm install
npm run dev
```
Frontend will be available at http://localhost:5173
#### Using Docker
```bash
bashdocker-compose up
```
###  Testing
Backend Tests
```bash cd backend
pytest ```
Frontend Tests
``` bash cd frontend
npm run test
```
 API Endpoints
EndpointMethodDescription/GETAPI information/healthGETHealth check/docsGETSwagger documentation/api/v1/analysis/analyzePOSTAnalyze resume against job description/api/v1/analysis/statusGETCheck analysis service status
 CI/CD Pipeline
Every push to main triggers:

Backend CI - Linting, type checking, unit tests
Frontend CI - Linting, type checking, unit tests, build verification
Auto-deployment - Deploy to Render (backend) and Vercel (frontend)

