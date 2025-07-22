# 🍔 Quick Grab Backend Server

This is the backend server for the **Quick Grab** application. It is built with **Node.js**, **Express**, **MongoDB**, and **JWT** for authentication and authorization.

---

## 🚀 Features

- 🔐 JWT-based authentication & role-based access (Admin/User)
- 📦 RESTful APIs for:
  - Users management
  - Menu items
  - Reviews
  - Cart operations
- 🛡 Middleware for token verification & admin checking
- 📡 MongoDB Atlas integration

---

## 🛠 Tech Stack

- **Node.js**
- **Express.js**
- **MongoDB (Atlas)**
- **JWT (jsonwebtoken)**
- **dotenv**
- **CORS**

---

## 📁 Folder Structure

project-root/
│
├── server.js # Main entry point (your file)
├── .env # Environment variables (DB credentials, JWT secret)
└── package.json # Project metadata and dependencies

# install dependencies
npm install

# start the server
npm run start
Server will run at: http://localhost:5000

📌 Notes
MongoDB client connection is left open to keep performance high during development. In production, implement graceful connection management.

All admin-only routes are protected via both verifyToken and verifyAdmin middleware.

🧑‍💻 Author
MD Emon Hossen
Backend Developer @ Quick Grab
Available for freelance and collaboration.

