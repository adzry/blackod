# 🖤 BLACKCODE AI  

> **Secure. Minimal. Precise.**  
> A full-stack AI companion built for professionals who demand **trust, performance, and elegance**.  

![BLACKCODE Banner](https://dummyimage.com/1200x300/000000/ffffff&text=BLACKCODE+AI)  

---

## ✨ Features
- 🔑 Authentication – JWT-based, secure by design  
- 💬 Conversations – Persistent AI chat with OpenAI GPT  
- 🛡 Security – Hardened backend with Helmet & rate limiting  
- ⚡ Fast Frontend – React + Vite + Tailwind + Nginx  
- 🗄 Data Layer – MongoDB with schema-driven persistence  
- 🐳 Deployment Ready – Docker Compose + Lovable AI support  

---

## 📂 Project Layout
\`\`\`
blackod/
├── backend/         # Express + MongoDB + JWT
├── frontend/        # React + Vite + Tailwind + Nginx
├── docker-compose.yml
├── lovable.yaml     # Lovable deployment config
├── .env.example     # Env placeholders
└── README.md
\`\`\`

---

## ⚙️ Environment Variables
Sensitive values live **outside GitHub**.

\`\`\`env
OPENAI_API_KEY=your-openai-api-key-here
JWT_SECRET=your-generated-secret-here
CORS_ORIGIN=http://localhost:5173
VITE_API_BASE=http://localhost:5000/api/v1
\`\`\`

---

## 🖥 Local Development (Termux/Node)
\`\`\`bash
git clone https://github.com/adzry/blackod.git
cd blackod
cp .env.example .env
nano .env   # fill real keys
export $(grep -v '^#' .env | xargs)
cd backend && npm install && npm run dev
cd ../frontend && npm install && npm run dev
\`\`\`

---

## 🚀 Deployment (Lovable)
1. Import repo → `adzry/blackod`  
2. Branch → `main`  
3. Add env vars in Lovable:  
   \`\`\`env
   OPENAI_API_KEY=sk-your-openai-key
   JWT_SECRET=your-32-byte-secret
   CORS_ORIGIN=https://blackod.lovable.app
   VITE_API_BASE=https://blackod.lovable.app/api/v1
   \`\`\`
4. Deploy → https://blackod.lovable.app  

---

## ✅ Post-Deploy Checklist
- [ ] Sign up → new user stored in MongoDB  
- [ ] Login → JWT session works  
- [ ] Chat → AI response saved in DB  
- [ ] Refresh → conversation persists  

---

## 🛡 Security Design
- JWT auth  
- Bcrypt password hashing  
- Helmet + CORS enforcement  
- Rate limiting  
- `.dockerignore` + `.gitignore`  

---

## 🧩 Tech Stack
- **Frontend:** React, Vite, TailwindCSS, Nginx  
- **Backend:** Node.js, Express, JWT, Mongoose  
- **Database:** MongoDB 7.0  
- **AI Engine:** OpenAI GPT  
- **Deployment:** Docker Compose + Lovable AI  

---

## 🖤 BLACKCODE Philosophy
> We don’t just write code.  
> We **encrypt ideas**.  
> BLACKCODE is a **digital fortress** — minimal surface, maximal power.  
