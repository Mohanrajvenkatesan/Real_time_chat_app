# 💬 Real-Time Chat Application

A modern **Real-Time Chat Application** built using the **MERN Stack** with **Socket.IO** for instant messaging and **Redis** for high-performance caching. The application provides secure authentication, one-to-one and group messaging, media sharing, typing indicators, read receipts, and push notifications while delivering a fast and responsive user experience.

---

# 🚀 Project Overview

The Real-Time Chat Application is designed to enable seamless communication between users through instant messaging. Built with **React.js**, **Node.js**, **Express.js**, **MongoDB**, and **Socket.IO**, the application supports real-time message delivery with minimal latency.

To improve performance, **Redis** is integrated for caching frequently accessed data, reducing API response time by approximately **40%**. The application uses **JWT-based authentication** to ensure secure access and implements modern messaging features such as typing indicators, read receipts, online/offline status, media sharing, and push notifications.

The project follows a scalable client-server architecture and is fully responsive across desktop and mobile devices.

---

# 🛠️ Tech Stack

## Frontend
- React.js
- Redux Toolkit
- Tailwind CSS
- React Router
- Axios

## Backend
- Node.js
- Express.js
- Socket.IO
- JWT Authentication
- Redis
- MongoDB
- Mongoose


---

# ✨ Key Features

## Authentication
- User Registration
- Secure Login
- JWT Authentication
- Password Encryption using bcrypt
- Protected Routes

## Real-Time Messaging
- Instant One-to-One Chat
- Group Chat
- Live Message Delivery
- Online/Offline User Status

## Chat Features
- Read Receipts
- Typing Indicators
- Message Timestamps
- Media Sharing
- Emoji Support 

## Notifications
- Push Notifications
- New Message Alerts
- Unread Message Counter

## Performance
- Redis Caching
- Optimized API Response Time
- Efficient Socket Connection Management

## UI
- Fully Responsive Design
- Modern Chat Interface
- Mobile Friendly

---

# 🏗️ System Architecture

```text
                     +----------------------+
                     |      React Client    |
                     |----------------------|
                     | Authentication       |
                     | Chat Interface       |
                     | Redux State          |
                     +----------+-----------+
                                |
                           REST API
                                |
                                v
                  +-----------------------------+
                  | Express + Node.js Server    |
                  |-----------------------------|
                  | JWT Authentication          |
                  | Chat Controllers            |
                  | User Controllers            |
                  | Media Upload APIs           |
                  +------+--------------+-------+
                         |              |
                 Socket.IO              |
          Real-Time Communication       |
                         |              |
                         |              |
                +--------+--------+     |
                | Socket Server   |     |
                +--------+--------+     |
                         |              |
                Real-Time Events        |
                         |              |
          ------------------------------
                         |
              +----------+----------+
              |                     |
              v                     v
      MongoDB Database         Redis Cache
      ----------------         -------------
      Users                    Cached Chats
      Messages                 User Sessions
      Groups                   Frequently Used Data
```

---

# ⚙️ Workflow

1. User registers or logs into the application.
2. JWT token is generated after successful authentication.
3. User joins personal and group chat rooms.
4. Messages are transmitted instantly through Socket.IO.
5. Chat history is stored in MongoDB.
6. Frequently accessed data is cached in Redis.
7. Read receipts and typing indicators are synchronized in real time.
8. Push notifications notify users about new messages.

---

# 📂 Project Structure

```
Chat-Application/
│
├── client/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── redux/
│   │   ├── services/
│   │   ├── socket/
│   │   ├── utils/
│   │   └── App.jsx
│   │
│   └── package.json
│
├── server/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── sockets/
│   ├── uploads/
│   ├── server.js
│   └── package.json
│
├── README.md
└── package.json
```

---

# 📦 Installation

## Clone Repository

```bash
git clone https://github.com/Mohanrajvenkatesan/real-time-chat-app.git

cd real-time-chat-app
```

## Install Dependencies

### Backend

```bash
cd server

npm install
```

### Frontend

```bash
cd client

npm install
```

---


# ▶️ Run the Application

## Backend

```bash
npm run dev
```

## Frontend

```bash
npm run dev
```

Open:

```
http://localhost:5173
```

---

# 📊 Performance Highlights

- 🚀 Reduced API response latency by **40%** using Redis caching.
- ⚡ Real-time communication powered by Socket.IO.
- 🔒 Secure JWT-based authentication.
- 📱 Fully responsive UI across devices.
- 📂 Optimized database queries for faster chat retrieval.

---

# 📸 Screenshots

- Login Page
- Register Page
- Chat Dashboard
- Group Chat
- Media Sharing
- Notifications
- User Profile
- Mobile View

*(Add screenshots here after deployment.)*

---

# 🔮 Future Enhancements

- Voice Calling
- Video Calling (WebRTC)
- End-to-End Encryption
- Message Reactions
- Message Search
- AI Chat Assistant
- Multi-language Support
- File Sharing
- Screen Sharing

---


## ⭐ If you found this project useful, consider giving it a star!
