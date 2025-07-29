# 🔐 User Authentication Service

A simple user authentication service built using **Node.js**, **Express**, **MySQL**, and **JWT**. This project handles user registration and login, and protects routes using JSON Web Tokens.

---

## 🚀 Features

- ✅ User Registration (Sign Up)
- 🔑 Secure Login with JWT
- 🔐 Protected Routes
- 🧂 Password Hashing using bcrypt
- 🗃 MySQL Database Integration
- 📦 Environment Variable Support with dotenv

---

## 📁 Project Structure

user-auth-service/
├── db.js # MySQL connection setup
├── middleware/
│ └── auth.js # JWT verification middleware
├── routes/
│ └── auth.js # Register & Login routes
├── .env # Environment variables
├── package.json # Node.js dependencies
├── server.js # Entry point

---

## 🛠️ Tech Stack

- **Node.js**
- **Express**
- **MySQL (mysql2)**
- **JWT**
- **bcryptjs**
- **dotenv**

---

## ⚙️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/user-auth-service.git
   cd user-auth-service
   
2. Install dependencies
npm install

3. Create .env file

PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_mysql_password
DB_NAME=auth_db
JWT_SECRET=your_jwt_secret

4. Setup MySQL Database

CREATE DATABASE IF NOT EXISTS auth_db;

USE auth_db;

CREATE TABLE users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(100) UNIQUE,
  password VARCHAR(255)
);

5. Run the server
   npm start
