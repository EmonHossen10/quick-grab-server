# 🚀 Quick Grab Server

[![Node.js](https://img.shields.io/badge/Node.js-18.x-green?style=for-the-badge&logo=node.js)](https://nodejs.org/)  
[![Express](https://img.shields.io/badge/Express-4.19.2-black?style=for-the-badge)](https://expressjs.com/)  
[![MongoDB](https://img.shields.io/badge/MongoDB-6.8.0-green?style=for-the-badge&logo=mongodb)](https://www.mongodb.com/)  
[![Stripe](https://img.shields.io/badge/Stripe-18.3.0-blue?style=for-the-badge&logo=stripe)](https://stripe.com/)  
[![License](https://img.shields.io/badge/License-ISC-blue?style=for-the-badge)](LICENSE)

---

## 📝 Description

Quick Grab Server is the backend of the Quick Grab food ordering app. It handles:  

- 🔹 **User authentication** with JWT  
- 🔹 **Secure payment processing** via Stripe  
- 🔹 **Database management** using MongoDB  
- 🔹 **Email notifications** using Mailgun & EmailJS  
- 🔹 **REST API endpoints** for frontend integration  

This server works seamlessly with the **Quick Grab Frontend**, enabling a complete food ordering and delivery experience.

---

## 🛠 Tech Stack

| Technology | Purpose |
|------------|---------|
| Node.js    | Runtime environment |
| Express.js | Server framework |
| MongoDB    | Database |
| JWT        | Authentication |
| Stripe     | Payment processing |
| Mailgun & EmailJS | Email notifications |
| Axios      | API requests |
| Nodemon    | Development server auto-restart |
| Dotenv     | Environment variable management |

---

## 📁 Folder Structure
```bash
quick-grab-server/
├─ index.js          # Main server entry point
├─ routes/           # API routes (auth, orders, payments)
├─ controllers/      # Request handling logic
├─ models/           # Database models (User, Order, etc.)
├─ services/         # External services (Stripe, Mailgun)
├─ utils/            # Helper functions
├─ package.json
└─ .env              # Environment variables
```

## ⚡ Installation & Run Locally

```bash
# Clone the repository
git clone https://github.com/EmonHossen10/quick-grab-server.git

# Navigate to the project folder
cd quick-grab-server

# Install dependencies
npm install

# Start the server
npm start

# For development with automatic reload
npm run dev
