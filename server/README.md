# 🛡️ MoneyMate 2.0 Backend (Node.js Server)

> **The Orchestration Layer.**  
> A high-performance Express.js server that manages user authentication, transaction persistence, and real-time connectivity across the platform.

---

## 🚀 Features

- **JWT Authentication**: Secure user login and encrypted session management.
- **RESTful API**: Standardized JSON endpoints for all financial operations.
- **Real-time Engine**: Socket.io integration for instant fraud alerts and sync notifications.
- **Payment Gateway**: Seamless Razorpay integration for manual balance top-ups.
- **Fraud Analysis Bridge**: Orchestrates data flow between the mobile app and the Python ML services.

---

## 🛠️ Tech Stack

- **Framework**: Express.js
- **Database**: MongoDB (via Mongoose)
- **Real-time**: Socket.io v4
- **Security**: Helmet, BCryptJS, Express-Rate-Limit
- **Payments**: Razorpay Node SDK

---

## 📂 Directory Structure

| Folder | Description |
|---|---|
| `/models` | Mongoose schemas for User, Transaction, and Ledger. |
| `/controllers` | Business logic for handling requests (Auth, Payments, Profile). |
| `/routes` | Endpoint registration and parameter validation. |
| `/middlewares` | JWT verification, logging, and security headers. |
| `/services` | Third-party integrations (Email, Fraud API client). |

---

## ⚙️ Configuration

Create a `.env` file in the root of the `/server` directory:

```env
PORT=5000
MONGODB_URI=your_mongo_url
JWT_SECRET=your_super_secret_key
RAZORPAY_KEY_ID=your_key
RAZORPAY_KEY_SECRET=your_secret
```

---

## 🏃 Getting Started

1. **Install Dependencies**:
   ```bash
   npm install
   ```

2. **Run in Development**:
   ```bash
   npm run dev
   ```

3. **Check Connection**:
   The server will default to `http://localhost:5000` or `http://10.0.2.2:5000` for Android emulators.

---

*MoneyMate Backend — Scalable Financial Infrastructure.*
