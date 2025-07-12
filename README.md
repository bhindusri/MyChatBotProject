# 🤖 Smarty OpenAI ChatBot
## Build with ♥ by REKAPALLI BHINDUSRI

A full-stack AI chatbot MERN application where users can securely register, chat with AI (powered by OpenAI GPT / Google Gemini), view & delete chat history, and manage their profiles — all built using modern technologies like React.js, Node.js, Express, MongoDB, TypeScript, JWT, and styled with Material UI (MUI).

---

## 🚀 Project Overview
Smarty AI Chatbot lets users:
- 🔐 Register/Login securely
- 💬 Chat with an AI bot (ChatGPT / Gemini API)
- 📜 View, save, and delete chat history
- 👤 Manage profile & account settings

---

## 🎯 Core Features
✅ **User Authentication**
- Register (email & password)
- Login (email & password)
- Logout (secure session management)

✅ **Chat System**
- Chat with AI (OpenAI ChatGPT / Gemini)
- View saved chat history
- Delete single chat messages
- Clear all chat history

✅ **User Profile & Account Management**
- View profile
- Edit profile (email, password, name)
- Delete account (removes all user data & chats)

---

## 🏗 Project Architecture

### 🖥 Frontend (React.js)
**Key Pages:**
- Signup Page
- Login Page
- Chat Page
- Chat History Page
- Profile Page

**Tech Stack:**
- React.js (with Redux / Context API for state)
- Axios (API calls)
- React Router (navigation)
- Material UI (MUI) for styling
- TypeScript

---

### 💾 Backend (Node.js + Express.js)
**API Endpoints:**
- **Auth:** `/register`, `/login`, `/logout`
- **Chat:** `/send-message`, `/get-history`, `/delete-message/:id`, `/clear-history`
- **User:** `/profile`, `/edit-profile`, `/delete-account`

**Tech Stack:**
- Node.js & Express.js
- TypeScript
- JWT (JSON Web Token) for secure authentication
- Middleware for validation & error handling

---

### 📂 Database (MongoDB)
Using MongoDB Atlas with Mongoose ORM.

#### 🧩 Users Collection
| Field     | Type     | Description             |
|----------|---------|-------------------------|
| _id      | ObjectId | Unique user ID          |
| email    | String   | Unique email            |
| password | String   | Hashed password         |
| name     | String   | User's name             |
| createdAt| Date     | Registration timestamp |

#### 💬 Chats Collection
| Field     | Type     | Description                                |
|----------|---------|----------------------------------------------|
| _id      | ObjectId | Unique chat ID                              |
| userId   | ObjectId | Reference to user                           |
| messages | Array    | [{ role: 'user' \| 'bot', content: '...' }] |
| timestamp| Date     | Date of chat                                 |

---

## 🔗 Third-Party Integrations
- ✅ OpenAI ChatGPT API
- ✅ Google Gemini API

---

## ✨ Optional Enhancements
- Google / Facebook OAuth login
- Dark mode interface
- Voice input for chat
- Chat image upload

---

## 📦 Tech Summary
- React.js
- Node.js
- Express.js
- MongoDB & Mongoose
- TypeScript
- JWT (authentication)
- MUI (Material UI)
- OpenAI / Gemini API

---

## 🌐 Live Demo
👉 [https://smarty-openai-chatbot.vercel.app/](https://smarty-openai-chatbot.vercel.app/)

---

## ⚙️ Deployment

### 📦 Backend
```bash
cd backend
npm install
npm run build
npm start

cd frontend
npm install
npm start

👤 Author
@bhindusri
