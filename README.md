# library-management-system
A RESTful Library Management API backend designed to manage users and book inventory with secure authentication and modular architecture.

# 📚 Library Management System API

A RESTful backend API for managing users and book inventory in a Library Management System.  
Built using Node.js and Express.js with a modular architecture and secure authentication.

---

## 🚀 Features

- User Registration & Login
- JWT-Based Authentication
- Add, Update, Delete Books
- View Book Inventory
- Role-Based Access (Admin/User)
- Secure Password Hashing (bcrypt)
- RESTful API Design

---

## 🛠 Tech Stack

- Node.js
- Express.js
- JWT (Authentication)
- bcrypt

---

## 📂 Project Structure

```
library-management-system/
│
├── src/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   └── config/
│
├── .env.example
├── .gitignore
├── package.json
├── server.js
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/yourusername/library-management-system.git
cd library-management-system
```

### 2️⃣ Install dependencies

```bash
npm install
```

### 3️⃣ Create a `.env` file

Create a `.env` file in the root directory using the following format:

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

### 4️⃣ Start the server

```bash
npm start
```

Server will run on:

```
http://localhost:5000
```

---

## 📌 API Endpoints

### 🔐 Authentication
- `POST /api/auth/register`
- `POST /api/auth/login`

### 📚 Books
- `GET /api/books`
- `POST /api/books`
- `PUT /api/books/:id`
- `DELETE /api/books/:id`

---


---

## 📈 Future Enhancements

- Fine calculation system
- Book availability tracking
- Due date management
- Docker containerization
- Cloud deployment (AWS / Render)

---

## 👩‍💻 Author

Safalya Barik  
BTech CSE | Backend & Cloud Enthusiast  
