# Fullstack Real-time Chat App

A complete real-time chat application featuring instant messaging, secure authentication, and online presence tracking. Designed with a clean separation between the **frontend** and **backend**, this project offers a scalable architecture suitable for production environments.

---

## 🚀 Features

- **Real-time communication** using Socket.IO
- **Secure authentication** with JWT
- **User presence tracking** (online/offline status)
- **Persistent chat history** stored in MongoDB
- **Responsive design** for both mobile and desktop devices
- **Typing indicators** and message timestamps

---

## 🛠 Tech Stack

- **Frontend:** React, Tailwind CSS
- **Backend:** Node.js, Express.js
- **Realtime Engine:** Socket.IO
- **Database:** MongoDB with Mongoose
- **Authentication:** JSON Web Tokens (JWT)
- **Tooling:** npm, concurrently (for dev scripts)

---

## 📂 Project Structure

fullstack-real-time-chat-app/ ├── backend/       # API & WebSocket server
                              ├── frontend/      # React client application
                              └── README.md      # Project documentation

---

## ⚙️ Setup Instructions

### 1️⃣ Prerequisites

- Node.js (LTS recommended)
- npm or yarn
- MongoDB instance (local or hosted via MongoDB Atlas)

### 2️⃣ Clone the Repository

```bash
git clone https://github.com/AnshMeshram/fullstack-real-time-chat-app.git
cd fullstack-real-time-chat-app
```
### 3️⃣ Install Dependencies

Backend:
- cd backend
- npm install

Frontend:
- cd ../frontend
- npm install

### 4️⃣ Environment Variables

Create a .env file in the backend directory with:

- PORT=5000
- MONGO_URI=your_mongo_connection_string
- JWT_SECRET=your_secret_key
- CLIENT_URL=http://localhost:3000

### 5️⃣ Run the Application (Development)

Backend:
- cd backend
- npm run dev

Frontend
- cd frontend
- npm run dev

  🔌 API Endpoints (Sample)

POST /api/auth/register – Register new user

POST /api/auth/login – Authenticate user

GET /api/users – Retrieve list of users

GET /api/messages/:conversationId – Fetch conversation messages

📡 Socket.IO Events (Sample)

Client → Server:

join – Join a specific chat room

sendMessage – Send a chat message

typing – Notify when a user is typing

Server → Client:

message – Broadcasts a new message

user-online / user-offline – Update user presence

typing – Typing indicator updates
