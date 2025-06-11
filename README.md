# 🧠 AI-Powered PR Agent Platform

This project is an AI-powered platform to help Vietnamese and foreign SMEs create and distribute press releases efficiently. It features a chatbot-based UI to gather input from users and uses AI to draft, distribute, and track press releases.

## 🚀 Project Overview

- **Frontend**: Chatbot interface (Web-based)
- **Backend**: Flask/FastAPI APIs running on AWS Lambda
- **Storage**: AWS S3 for files and structured content
- **ML/NLP**: Keyword extraction, draft generation using OpenAI or custom models
- **Pipeline**: CI/CD with GitHub Actions (Lint, Test, Deploy)
- **Architecture**: Serverless + microservice-oriented

---

## 🏗️ File Structure

ai-pr-agent/
│
├── backend/ # Flask/FastAPI APIs
│ ├── main.py # API entrypoint
│ ├── routes/
│ │ ├── chat.py # Chatbot message handling
│ │ └── draft.py # PR generation routes
│ ├── services/
│ │ ├── storage.py # S3 interaction etc
│ │ └── db.py # DB setup and operations
│ └── utils/
│      └── session.py # Session/token handling
│
├── frontend/ # Chatbot frontend interface
│ ├── public/
│ ├── src/
│ │ ├── components/
│ │ ├── App.jsx
│ │ └── chatbot/ # Bot logic & state
│ │ └── ChatBot.tsx
│ └── package.json
│
├── scripts/ # Deployment & setup scripts
│ ├── deploy.sh
│ └── init_ci.yml # GitHub Actions workflow
│
├── tests/ # Unit & integration tests
│ ├── test_chat.py
│ └── test_draft.py
│
├── .github/
│ └── workflows/
│ └── ci.yml # Linting, tests, build pipeline
│
├── requirements.txt # Python backend dependencies
├── README.md # This file
└── .env.example # Env variables sample
