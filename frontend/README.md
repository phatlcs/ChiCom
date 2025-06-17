# 📰 ChiCom AI PR Agent

An AI-powered PR automation tool for SMEs that streamlines the press release lifecycle—from content drafting to media distribution—using natural language interfaces and machine learning.

## 🚀 Project Overview

The AI PR Agent helps Vietnamese and foreign SMEs create and distribute high-quality bilingual (EN/VN) press releases. It uses a conversational chatbot UI for input and provides AI-generated drafts, intelligent media recommendations, and automated report tracking.

Core technologies:
- 🧠 AI (OpenAI/GPT) for press release drafting and keyword analysis
- 💬 Chatbot UI for seamless interaction
- ☁️ AWS (Lambda, S3, API Gateway) for scalable infrastructure
- 🧰 FastAPI/Flask backend with modular architecture
- 📊 n8n workflows for automation

## ✨ Key Features

- Conversational chatbot to gather PR info
- Bilingual press release draft generation (EN/VN)
- Upload supporting docs (.doc/.pdf)
- Intelligent keyword extraction
- AWS-powered file storage and APIs
- Template-based drafting system
- Scalable and testable codebase

---

## 📁 Project File Structure

<pre><code>ai-pr-agent/
│
├── backend/                      # Flask/FastAPI APIs
│   ├── main.py                   # API entrypoint
│   ├── routes/
│   │   ├── chat.py               # Chatbot message handling
│   │   └── draft.py              # PR generation routes
│   ├── services/
│   │   ├── storage.py            # S3 interaction
│   │   └── db.py                 # DB setup and operations
│   └── utils/
│       ├── parser.py             # Text parsing utilities
│       └── session.py            # Session/token handling
│
├── frontend/                     # Chatbot frontend interface
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── App.jsx
│   │   └── chatbot/              # Bot logic & state
│   │       └── ChatBot.tsx
│   └── package.json
│
├── scripts/                      # Deployment & setup scripts
│   ├── deploy.sh
│   └── init_ci.yml               # GitHub Actions workflow
│
├── tests/                        # Unit & integration tests
│   ├── test_chat.py
│   └── test_draft.py
│
├── .github/
│   └── workflows/
│       └── ci.yml                # Linting, tests, build pipeline
│
├── requirements.txt              # Python backend dependencies
├── README.md                     # This file
└── .env.example                  # Env variables sample
</code></pre>

---

## 🛠️ Setup Instructions

### 1. Clone the repository
```bash
git clone https://github.com/phatlcs/ChiCom.git
cd ChiCom
TODO
