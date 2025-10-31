# 📈 MATs (Multi-Agent Trading Assistant)

An AI-powered financial assistant designed for everyday investors and beginners who want to understand how stocks are performing without needing to know technical jargon.
Whether you’re curious about short-term momentum, long-term growth potential, or the overall market sentiment, this chatbot gives you clear, easy-to-understand answers backed by real financial data.

---

## 🎥 Demo Video  

![Demo](demo.gif)

---

## 🚀 Features

- **Simple Language Queries** – Ask natural questions like:  
  - “Is Apple looking good for the next few months?”  
  - “What’s the outlook for Tesla in the long term?”  
- **Multi-Agent AI System** – Specialized agents for sentiment, fundamentals, technical indicators, portfolio health, and risk.  
- **Real-Time Insights** – Live stock and market data via Alpha Vantage, cached with Redis for faster responses.  
- **AI-Powered Routing** – Queries are intelligently routed to the right analysis agents using OpenAI tool-calling.  
- **Interactive Web App** – Beginner-friendly frontend with charts, summaries, and portfolio analysis.  
- **Dockerized Deployment** – Quick setup, scalable, and reproducible.  

---

## 🧱 Architecture Overview

Frontend (React.js + TailwindCSS)  
↓  
FastAPI Backend  
├── Dispatcher Agent (OpenAI Tool Calling)  
├── SentimentAgent  
├── TechnicalAgent  
├── FundamentalAgent    
├── PortfolioAgent  
├── RiskAgent  
↓  
External APIs (Alpha Vantage, News, etc.)

---

## ⚙️ Setup Instructions

### 🔧 Prerequisites

- Docker & Docker Compose  
- Python 3.10+  
- Node.js 18+  
- Alpha Vantage API Key  
- OpenAI API Key  

### 🐳 Backend (FastAPI)
```bash
cd backend  
cp .env.example .env  # Add your keys here  
docker compose up
```

### 💻 Frontend (React.js)
```bash
cd frontend  
npm install  
npm run dev  
```
---

## 📚 Example Queries

- "How is Nvidia expected to perform in the short term?”  
- “Tell me the long-term growth potential of Tesla.”
- "Give me the RSI and MACD for TSLA."  
- “What’s the market sentiment around Microsoft right now?” 

---

## 📦 Technologies Used

- Backend: FastAPI, Redis, Docker
- AI: OpenAI Tool Calling, JSON Agent Outputs
- Data: Alpha Vantage API
- Frontend: React.js, TailwindCSS

---

## 📄 License

This project is licensed under the MIT License.

---
