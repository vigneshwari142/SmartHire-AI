# SmartHire AI — Intelligent Resume Screening

AI-powered resume screening system using **SmartHire AI Engine** (Groq API + LLaMA 3.3 70B).

## Quick Start

### 1. Get Groq API Key (Free)
1. Go to https://console.groq.com
2. Sign up → Create API Key
3. Copy the key

### 2. Setup Backend
```bash
cd smarthire-ai/backend
cp .env.example .env
# Edit .env → add GROQ_API_KEY=your_key_here
npm install
npm run dev
```

### 3. Setup Frontend
```bash
# New terminal
cd smarthire-ai/frontend
npm install
npm start
```

### 4. Open App
Go to http://localhost:3000 → Register → Start screening!

## .env Configuration
```
MONGODB_URI=mongodb://localhost:27017/smarthire_ai
JWT_SECRET=your_secret_key
GROQ_API_KEY=your_groq_api_key_here
GROQ_MODEL=llama-3.3-70b-versatile
PORT=5000
```

## AI Engine
- **Provider**: Groq API
- **Model**: LLaMA 3.3 70B Versatile
- **Speed**: ~2-3 seconds per resume (Groq is extremely fast)
- **Scoring**: 6 dimensions — Skills, Experience, Education, Keywords, ATS, Overall

## Features
- Upload PDF/DOCX resumes (up to 20 at once)
- Create job descriptions with custom scoring weights
- AI evaluation with detailed reports
- Candidate ranking and shortlisting
- Analytics dashboard with charts
- PDF report export

## Tech Stack
- **Backend**: Node.js + Express + MongoDB
- **Frontend**: React (White + Sky Blue theme)
- **AI**: Groq API (LLaMA 3.3 70B)
- **Charts**: Recharts
