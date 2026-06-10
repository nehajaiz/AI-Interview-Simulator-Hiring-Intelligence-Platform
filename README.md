🚀 AI Interview Simulator & Hiring Intelligence Platform

📌 Overview

AI Interview Simulator & Hiring Intelligence Platform is an AI-powered recruitment solution designed to help candidates prepare for interviews and assist recruiters in making data-driven hiring decisions.

The platform combines Resume Intelligence, AI Mock Interviews, Speech Analysis, Video Analytics, Skill Gap Detection, and Candidate Scoring into a single system that enhances both candidate preparation and hiring efficiency.

✨ Key Features

📄 Resume Intelligence
Resume Upload (PDF/DOCX)
Resume Parsing & Information Extraction
Skill, Education, Experience & Project Detection
ATS Compatibility Scoring
Job Description Matching
🤖 AI Interview Simulator
HR Interview Simulation
Technical Interview Simulation
Behavioral Interview Questions
Dynamic Follow-up Questions
Real-Time Feedback
🎤 Speech Intelligence
Speech-to-Text Conversion
Filler Word Detection
Speaking Speed Analysis
Communication & Confidence Scoring
📹 Video Intelligence
Face Detection
Eye Contact Tracking
Emotion Recognition
Attention & Engagement Analysis
📊 Hiring Intelligence Engine
Candidate Ranking System
Performance Evaluation
Strength & Weakness Analysis
Hiring Recommendations
🎯 Skill Gap Analysis
Missing Skill Identification
Personalized Learning Roadmap
Certification Recommendations
📈 Recruiter Dashboard
Candidate Analytics
Interview Performance Tracking
Ranking Leaderboard
Hiring Insights & Reports
🛠 Tech Stack

## Project Structure

```
ai-interview-platform/
├── backend/
│   ├── app/
│   │   ├── api/v1/endpoints/      # Route handlers
│   │   │   ├── auth.py            # Login, signup, JWT, /me
│   │   │   ├── resumes.py         # Upload, list, delete, set-primary
│   │   │   ├── questions.py       # Question generation endpoints
│   │   │   └── recruiter_dashboard.py  # Ranking, analytics, history
│   │   ├── core/
│   │   │   ├── config.py          # Pydantic settings (env vars)
│   │   │   └── security.py        # JWT, password hashing, role deps
│   │   ├── db/session.py          # Async SQLAlchemy engine + session
│   │   ├── models/                # SQLAlchemy ORM models
│   │   │   ├── user.py
│   │   │   ├── resume.py
│   │   │   ├── interview.py
│   │   │   ├── interview_score.py
│   │   │   ├── skill.py
│   │   │   ├── job_role.py
│   │   │   └── analytics.py
│   │   ├── schemas/               # Pydantic request/response models
│   │   ├── services/
│   │   │   ├── ai/                # Resume intelligence, ATS, questions
│   │   │   │   ├── resume_intelligence_service.py
│   │   │   │   ├── ats_scorer.py
│   │   │   │   ├── question_generator.py
│   │   │   │   ├── education_extractor.py
│   │   │   │   ├── experience_extractor.py
│   │   │   │   ├── project_extractor.py
│   │   │   │   ├── skills_extractor.py
│   │   │   │   └── embeddings.py
│   │   │   ├── analytics/         # Candidate scoring, dashboard queries
│   │   │   │   ├── candidate_scoring_service.py
│   │   │   │   ├── dimension_scorers.py
│   │   │   │   ├── evidence_collector.py
│   │   │   │   └── dashboard_query_service.py
│   │   │   ├── interview/         # Speech & webcam analysis
│   │   │   │   ├── speech_analysis_service.py
│   │   │   │   ├── transcription_engine.py
│   │   │   │   ├── filler_detector.py
│   │   │   │   ├── speech_metrics.py
│   │   │   │   ├── confidence_scorer.py
│   │   │   │   ├── webcam_analytics_service.py
│   │   │   │   ├── face_detector.py
│   │   │   │   ├── eye_contact_analyser.py
│   │   │   │   └── emotion_detector.py
│   │   │   └── storage/           # S3 / local file storage
│   │   │       ├── storage_service.py
│   │   │       └── extraction_service.py  # PyMuPDF + python-docx
│   │   └── main.py                # FastAPI app factory, middleware
│   ├── migrations/                # Alembic migration scripts
│   ├── requirements.txt
│   ├── alembic.ini
│   ├── Dockerfile
│   └── Dockerfile.dev
│
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   │   ├── auth/AuthPage.jsx           # Login + signup UI
│   │   │   ├── candidate/ResumeUploadPage.jsx
│   │   │   └── recruiter/RecruiterDashboard.jsx
│   │   ├── services/api/index.ts           # Axios + all API calls
│   │   ├── store/slices/authStore.ts       # Zustand auth state
│   │   ├── App.tsx                         # Router
│   │   ├── main.tsx                        # Entry point
│   │   └── index.css
│   ├── public/index.html
│   ├── package.json
│   ├── vite.config.ts
│   ├── tailwind.config.ts
│   ├── tsconfig.json
│   ├── nginx.conf                          # Production Nginx config
│   ├── Dockerfile
│   └── Dockerfile.dev
│
├── infrastructure/
│   ├── postgres/init.sql          # Extensions + app_user role
│   └── redis/redis.conf           # Persistence, memory policy
│
├── docker-compose.yml             # Production stack
├── docker-compose.dev.yml         # Dev overrides (hot-reload, pgAdmin, Flower)
├── .env.docker                    # Environment template
├── .dockerignore
└── README.md
```

---

📸 Screenshot


🌐 Live Demo

https://github.com/nehajaiz/AI-Interview-Simulator-Hiring-Intelligence-Platform/


📧 Contact

Email: nehajaiswal593593@gmail.com


⭐ If you like this project, give it a star!
