# MemeStream-API

Node.js + Express backend API for MemeStream.  
Provides authentication and CRUD endpoints for posts. Pairs with the **MemeStream-App** Android client.

![Cover](../docs/screenshots/MemeStream-API-cover.png)

## ✨ Features
- User registration + login (JWT-based)
- Authentication middleware
- CRUD for posts (create, read, update, delete)
- Input validation + error handling
- JSON responses with proper status codes

## 🧱 Tech Stack
- Node.js + Express
- MongoDB or SQL (depending on setup)
- JWT (jsonwebtoken)
- bcrypt for password hashing

## 🚀 Quick Start
### Prerequisites
- Node.js v20+
- Database (MongoDB or SQL)

### Run
```bash
npm install
npm run dev
