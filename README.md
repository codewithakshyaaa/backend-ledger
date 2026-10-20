# Banking Ledger Backend

A backend application built using Node.js, Express.js, and MongoDB to manage accounts and financial transactions using a ledger-based approach.

## 🚀 Features

- User Authentication using JWT
- Password Hashing using bcrypt
- Account Management
- Transaction Management
- Ledger-Based Transaction Recording
- Balance Calculation using MongoDB Aggregation
- Idempotency Support for Transaction Requests
- Transaction Status Tracking
- RESTful API Development

## 🛠️ Tech Stack

- **Runtime:** Node.js
- **Framework:** Express.js
- **Database:** MongoDB
- **ODM:** Mongoose
- **Authentication:** JSON Web Tokens (JWT)
- **Password Security:** bcrypt

## 📋 Prerequisites

Before running this project, make sure you have installed:

- Node.js
- npm
- MongoDB or a MongoDB Atlas account
- Git

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone <https://github.com/codewithakshyaaa/backend-ledger.git>
cd backend-ledger
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory and add the following variables:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

Replace the placeholder values with your actual configuration.

**Important:** Never commit your `.env` file or expose your database credentials and JWT secret.

### 4. Run the Application

Start the server using the script configured in your `package.json`.

```bash
npm start
```

If your project uses a development script, you can run:

```bash
npm run dev
```

## 🧠 How It Works

The application follows a REST API architecture to handle account operations and financial transactions.

1. Clients send requests to the backend through API endpoints.
2. Express.js routes direct requests to the appropriate handlers.
3. Authentication middleware verifies access where required.
4. MongoDB stores account and transaction records.
5. Ledger records provide a structured history of financial activity.
6. MongoDB aggregation can be used to calculate account balances from transaction records.

The exact transaction flow depends on the implemented application logic.

## 📚 Key Concepts

### Authentication
JWT-based authentication is used to verify user identity, while bcrypt helps protect passwords through hashing.

### Ledger-Based Transaction Recording
A ledger maintains structured records of financial transactions, making account activity easier to track.

### Balance Calculation
MongoDB aggregation can calculate balances from transaction records, depending on the ledger design.

### Idempotency
Idempotency helps prevent duplicate transaction processing when requests are retried, provided the implementation correctly enforces it.

## 🧪 Testing

API endpoints can be tested using Postman or another API testing tool.

Recommended test cases include:

- Authentication with valid and invalid credentials
- Account creation and retrieval
- Valid and invalid transaction requests
- Balance calculation
- Transaction status verification
- Repeated transaction requests to check idempotency

## 🔐 Security Disclaimer

This project is intended for educational purposes and backend development practice.

It is not a production-ready banking system and should not be used to process real financial transactions.

## 🎯 Learning Objectives

- Building RESTful APIs using Express.js
- Connecting Node.js applications to MongoDB
- Implementing authentication and password hashing
- Understanding ledger-based transaction systems
- Calculating account balances using database aggregation
- Managing transaction records and statuses
- Exploring idempotency in financial APIs

## 👩‍💻 Author

**AKSHYA TIWARY**

Student Developer | Backend Development | FinTech

---

Built as a learning project to explore backend development and ledger-based financial systems.
