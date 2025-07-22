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

🧪 API Endpoints
🔐 Auth
Method	Endpoint	Description
POST	/jwt	Generate JWT token

👤 Users
Method	Endpoint	Description
GET	/users	Get all users (admin only)
GET	/users/admin/:email	Check if user is admin
POST	/users	Create a new user
DELETE	/users/:id	Delete a user (admin only)
PATCH	/users/admin/:id	Make user admin (admin only)

📋 Menu
Method	Endpoint	Description
GET	/menu	Get all menu items

🌟 Reviews
Method	Endpoint	Description
GET	/reviews	Get all customer reviews

🛒 Cart
Method	Endpoint	Description
GET	/carts?email=	Get cart items for a user
POST	/carts	Add item to cart
DELETE	/carts/:id	Remove item from cart

✅ Middleware
verifyToken: Verifies JWT token from request headers.

verifyAdmin: Checks if user has admin role.

🧾 Usage
bash
Copy
Edit
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

📃 License
This project is licensed under the MIT License.

yaml
Copy
Edit

---

et me know if you'd like this turned into a downloadable file or deployed to GitHub with setup instructions!
