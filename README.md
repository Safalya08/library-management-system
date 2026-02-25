# 📚Library Management System API
A RESTful Library Management API backend designed to manage users and book inventory with secure authentication and modular architecture.
Built using Node.js and Express.js with a modular architecture and secure authentication.

---

# Routes and the Endpoints

## /users
GET: Get all the list of users in the system
POST: Create/Register a new user

## /users/{id}
GET: Get a user by their ID
PUT: Updating a user by their ID
DELETE: Deleting a user by their ID (check if the user still has issued a book) && (is there any fine/penalty to be collected)

## /users/subscription-details/{id}
GET: Get the user details by their ID 
   >>Date of subscription
   >>Valid till?
   >>Fine if any?

## /books
GET: Get all the books in the system
POST: Add a new book to the system

## /book/{id}
GET: Get a book by its ID
PUT: Update a book by its ID
DELETE: Delete a book by its ID

## /book/issued

GET: Get all the issued books

## /books/issued/withFine

GET: Get all issued books with their amount

## Subscription Types

    >>Basic ( 3 months )
    >>Standard (6 months)
    >>Premium (12 months)

> >If a user missed the renewal date, then user should be collected with $100
> >If a user missed his subscription, then user is expected to pay $100
> >If a user misses both renewal and subscription, then collected amount should be $200

---

## Commands:
npm init
npm i express
npm i nodemon --save-dev

npm run dev

To restore node modules and package-lock.json ---> npm i/npm install
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
git clone https://github.com/Safalya08/library-management-system.git
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
