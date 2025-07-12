# 🤖 Smarty OpenAI ChatBot
## Build with ♥ by REKAPALLI BHINDUSRI

---

## 🚀 Project Overview
Smarty AI Chatbot is a full-stack MERN application where users can:
- Register/Login securely
- Chat with an AI bot (powered by OpenAI's GPT / Google Gemini)
- Save, view, and delete chat history
- Manage profile and account settings

Built with modern technologies like React.js, Node.js, Express, MongoDB, TypeScript, JWT, and styled using Material UI (MUI) for a clean user interface.

---

## 🎯 Core Features
✅ User Authentication  
- Register (Sign up with email/password)  
- Login (Sign in with email/password)  
- Logout (secure session management)

✅ Chat System  
- Chat with AI (ChatGPT / Gemini API)  
- View saved chat history  
- Delete single chat messages  
- Clear entire chat history

✅ User Profile & Account Management  
- View profile  
- Edit profile (change email, password, name)  
- Delete account (removes all user data & chats)

---

## 🏗 Project Architecture

### 🖥 Frontend (React.js)
- Signup Page
- Login Page
- Chat Page
- Chat History Page
- Profile Page

📦 Tech Stack:
- React.js (with Redux / Context API)
- Axios (for API calls)
- React Router (page navigation)
- MUI (Material UI)

---

### 💾 Backend (Node.js + Express.js)
- Auth Routes: `/register`, `/login`, `/logout`
- Chat Routes: `/send-message`, `/get-history`, `/delete-message/:id`, `/clear-history`
- User Routes: `/profile`, `/edit-profile`, `/delete-account`

📦 Tech Stack:
- Node.js & Express.js
- JWT for secure authentication
- Middleware for validation
- TypeScript

---

### 📂 Database (MongoDB)
Using MongoDB Atlas with Mongoose ORM.

#### Users Collection
| Field     | Type     | Description                 |
|----------|---------|-----------------------------|
| _id      | ObjectId | Unique user ID              |
| email    | String   | Unique email                |
| password | String   | Hashed password             |
| name     | String   | User's name                 |
| createdAt| Date     | Registration timestamp     |

#### Chats Collection
| Field     | Type     | Description                              |
|----------|---------|-------------------------------------------|
| _id      | ObjectId | Unique message/chat ID                    |
| userId   | ObjectId | Reference to user                         |
| messages | Array    | [{ role: 'user' \| 'bot', content: '' }] |
| timestamp| Date     | Date of chat                               |

---

## 🔗 Third-Party Integrations
- ✅ OpenAI ChatGPT API
- ✅ Google Gemini API

---

## ✨ Optional Enhancements
- Google / Facebook OAuth login
- Dark mode UI
- Voice input for chat
- Chat image upload

---

## 📦 Tech Summary
- React.js
- Node.js
- Express.js
- MongoDB & Mongoose
- TypeScript
- JWT (JSON Web Token)
- MUI (Material UI)
- OpenAI / Gemini API

---

## 🌐 Demo
👉 [https://smarty-openai-chatbot.vercel.app/](https://smarty-openai-chatbot.vercel.app/)

---

## ⚙️ Deployment

## Deployment

To deploy this project run

BackEnd
```bash
    cd backend
    npm run build
    npm start
```

FrontEnd
```bash
    cd frontend
    npm start
```

## Authors

- [@bhindusri](https://www.github.com/bhindusri)

