# 🤖 AI Resume Analyzer

A **production-grade AI Resume Analysis platform** powered by FastAPI and Google Gemini 2.5 Flash.
Analyze resumes against job descriptions in real time with **intelligent scoring, explainability, and actionable insights**.

---

## 🚀 Overview

Upload a resume, paste a job description, and instantly get:

* 🎯 Job Match Score
* 🧠 AI-powered insights
* 📊 Skill gap analysis
* 🛠 Actionable improvement suggestions

Built as a **real-world SaaS-ready system**, not just a demo.

---

## ✨ Features

### 🧩 Core Analysis

* **Match Score** — Accurate job-fit percentage with animated visualization
* **Fit Status** — `🟢 Ideal` / `🟡 Overqualified` / `🔴 Underqualified`
* **Skills Breakdown** — Clearly categorized matched vs missing skills

---

### 🚀 Advanced (Unique Features)

#### 🔍 1. WHY Score (Explainability Engine)

Breaks down score into:

* Skills Match %
* Experience Alignment %
* Gap Penalty %

---

#### 🔄 2. Role Switch (Dual Perspective)

Toggle between:

* 👤 Candidate View → Improvement tips
* 🧑‍💼 Recruiter View → Hiring insights

---

#### 🗺 3. Skill Gap Roadmap

* Priority-based missing skills
* Estimated score impact per skill

---

#### 🧪 4. What-If Simulator

* Simulate adding skills
* Instantly see score improvement

---

#### ✨ 5. Auto Resume Improver

* AI rewrites weak bullet points
* Uses **STAR method + quantifiable metrics**

---

## 🎨 UX & Design

* 🌗 Light / Dark Mode (persistent)
* 📱 Fully responsive (mobile + desktop)
* ⚡ Smooth animations and transitions
* 🔄 No page reloads (SPA experience)

---

## 🛠 Tech Stack

| Layer       | Technology                           |
| ----------- | ------------------------------------ |
| Frontend    | React 19 + TypeScript + Vite         |
| Styling     | Tailwind CSS v4 + Framer Motion      |
| Backend     | FastAPI (Python 3.10+)               |
| AI Engine   | Google Gemini 2.5 Flash              |
| PDF Parsing | PyPDF2                               |
| Deployment  | Vercel (Frontend) + Render (Backend) |

---

## ⚙️ Local Setup

### 🔧 Prerequisites

* Node.js 18+
* Python 3.10+
* Gemini API Key

---

### 📦 Clone Repo

```bash
git clone https://github.com/your-username/ai-resume-analyzer.git
cd ai-resume-analyzer
```

---

### 🔙 Backend Setup

```bash
cd backend
python -m venv venv

# Windows
.\venv\Scripts\activate

# macOS/Linux
source venv/bin/activate

pip install -r requirements.txt
```

Create `.env`:

```env
LLM_API_KEY=your_api_key
ALLOWED_ORIGINS=http://localhost:5173
```

Run backend:

```bash
uvicorn main:app --host 0.0.0.0 --port 10000 --reload
```

---

### 🌐 Frontend Setup

```bash
cd ai-resume-analyzer
npm install
```

Create `.env`:

```env
VITE_API_URL=http://localhost:10000
```

Run frontend:

```bash
npm run dev
```

Open:

```
http://localhost:5173
```

---

## 🔐 Environment Variables

### Backend

| Variable        | Description           |
| --------------- | --------------------- |
| LLM_API_KEY     | Gemini API Key        |
| ALLOWED_ORIGINS | Allowed frontend URLs |

---

### Frontend

| Variable     | Description     |
| ------------ | --------------- |
| VITE_API_URL | Backend API URL |

---

## 🌍 Deployment

### Backend (Render)

* Root: `backend/`
* Build: `pip install -r requirements.txt`
* Start: `uvicorn main:app --host 0.0.0.0 --port 10000`
* Add env variables

---

### Frontend (Vercel)

* Root: `ai-resume-analyzer/`
* Framework: Vite
* Add env: `VITE_API_URL`

---

## 📊 Usage

1. Upload resume (PDF)
2. Paste job description
3. Click **Analyze**
4. Explore:

   * 📊 Overview
   * 🗺 Roadmap
   * ✨ Improve
5. Toggle **Candidate / Recruiter view**
6. Switch themes 🌗

---

## ⚠️ Important Notes

* Free-tier Gemini API has request limits
* System includes fallback + caching for stability
* AI output may vary slightly due to model behavior

---

## 📸 Screenshots

>
> ### 🖥 Dashboard
> <img width="1297" height="630" alt="Screenshot (11)" src="https://github.com/user-attachments/assets/49ed6ee3-157c-4da8-8825-7635c5dd23a3" />
### 📊 Analysis Result
<img width="1297" height="621" alt="Screenshot (15)" src="https://github.com/user-attachments/assets/a8db9beb-8a1b-4817-8253-e65b2f323573" />

### 📸 FEATURES
<img width="1309" height="625" alt="Screenshot (12)" src="https://github.com/user-attachments/assets/016426da-ae4e-402a-abac-842395023bf3" />

### 📊 LIVE DEMO
<img width="1300" height="630" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/af57c2b3-f9c1-4005-a50a-a6f6d6ee7f51" />


 ### 🖥 FOOTER
 <img width="1323" height="621" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/36a01890-8f0b-4e35-a899-1a54c1e7686e" />

---

## 📄 License

MIT License — free to use and modify.
