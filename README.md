# BLACKCODE — Full Stack AI App

BLACKCODE is a **production-ready full-stack AI assistant** built with:
- **Frontend:** React + Vite + White Minimal UI + Nginx
- **Backend:** Node.js (Express) + MongoDB + JWT Authentication
- **AI Engine:** OpenAI (gpt-4o-mini by default)
- **Deployment:** Docker & Docker Compose
- **Domain:** Preconfigured for https://blackcode.lovable.app

---

## 📂 Project Structure
```
blackcode-ai-full/
├── backend/        # Node.js backend (Express, MongoDB, JWT)
├── frontend/       # React (Vite) frontend + Nginx
└── docker-compose.yml
```

---

## 🚀 Quick Start (Local)
1. Unzip the project
2. Run:
```bash
cd blackcode-ai-full
export OPENAI_API_KEY="your-openai-key"
export JWT_SECRET="super-long-random-secret"
docker-compose up --build
```
3. Access:
- Frontend → [http://localhost](http://localhost)
- Backend API → [http://localhost:5000/api/v1](http://localhost:5000/api/v1)

---

## 🌐 Lovable Deployment
This bundle is **Lovable-ready**:
- Default domain: `https://blackcode.lovable.app`
- All `/api/*` requests proxy to the backend automatically

### Steps:
1. Import this repo into Lovable
2. Set Environment Variables in Lovable Dashboard:
   - `OPENAI_API_KEY` → your OpenAI key
   - `JWT_SECRET` → a long random string
   - `CORS_ORIGIN` → `https://blackcode.lovable.app`
   - `VITE_API_BASE` → `https://blackcode.lovable.app/api/v1`
3. Deploy 🚀

---

## 🔑 Environment Variables

### Backend
```
MONGO_URI=mongodb://mongodb:27017/blackcode
JWT_SECRET=super-long-random-secret
JWT_EXPIRES_IN=90d
OPENAI_API_KEY=your-openai-key
PORT=5000
CORS_ORIGIN=https://blackcode.lovable.app
```

### Frontend
```
VITE_API_BASE=https://blackcode.lovable.app/api/v1
```

---

## 🛡️ Security
- **Helmet** for HTTP headers
- **Rate limiting** (120 requests/minute)
- **JWT auth** for sessions
- **MongoDB** persistence

---

## 🎨 UI Features
- White minimal theme (Lovable-style)
- Login / Signup in one clean screen
- Sidebar for conversations
- Chat bubbles for user & assistant messages
- Responsive layout

---

## 📄 License
This project is released for internal BLACKCODE / Lovable deployment.