# 🌱 Async Errors – Farm & Product Management App

A **Node.js + Express** web application with **MongoDB (Mongoose)** and **EJS templates**, built to practice and demonstrate **async error handling** in Express.

---

## 🚀 Features
- 🌾 **Farm Management** – Create, list, and view farms
- 🛒 **Product Management** – Add, edit, list, and show products
- ⚡ **Custom Error Handling** – Centralized error middleware with `AppError.js`
- 🌐 **EJS Templates** – Dynamic frontend rendering with clean templates
- 🌱 **Seed Script** – Populate sample farms/products using `seeds.js`

---

## 📂 Project Structure
async-errors/
├── models/ # Database models (Mongoose schemas)
│ ├── farm.js
│ └── product.js
│
├── views/ # EJS templates
│ ├── farms/
│ │ ├── index.ejs # List all farms
│ │ ├── new.ejs # Form to create a new farm
│ │ └── show.ejs # Show farm details
│ │
│ └── products/
│ ├── index.ejs # List all products
│ ├── new.ejs # Form to create a new product
│ ├── edit.ejs # Edit product details
│ └── show.ejs # Show product details
│
├── .gitignore # Ignored files (node_modules, .env, etc.)
├── AppError.js # Custom error class for async handling
├── index.js # Main Express server
├── seeds.js # Database seeding script
├── package.json # Dependencies and scripts
└── README.md # Project documentation

---

## ⚙️ Installation & Setup

1. **Clone the repo**
   ```bash
   git clone https://github.com/YatharthChamoli/async-errors.git
   cd async-errors

2. **Install dependencies**
    npm install

3. **Set up environment variables**
    Create a .env file in the root:
    PORT=3000
    MONGODB_URI= mongodb://localhost:27017/farmStand2

4. **Seed the database**
    node seeds.js

5. **Start the server**
    npm start
    # or for dev with nodemon
    npm run dev

6. **Open in browser:**
   👉 http://localhost:3000 


7. **📜 Scripts**
| Command         | Description                     |
| --------------- | ------------------------------- |
| `npm start`     | Start the server                |
| `npm run dev`   | Start with nodemon (hot reload) |
| `node seeds.js` | Populate DB with sample data    |


🛠 Tech Stack
Backend: Node.js, Express
Database: MongoDB, Mongoose
Frontend: EJS Templates
Utilities: dotenv, nodemon

⚡ Error Handling
This project demonstrates async error handling using:
AppError.js → Custom error class
Centralized error middleware in index.js
Cleaner async functions with try/catch and next(err)
