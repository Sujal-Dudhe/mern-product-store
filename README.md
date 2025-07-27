# MERN Product Store

This is a full-stack MERN (MongoDB, Express, React, Node.js) application that allows users to manage a product inventory. Users can create, read, update, and delete products.

---

## ✨ Features

* **View all products** on the homepage.
* **Create new products** with a name, price, and image.
* **Update existing products**.
* **Delete products**.
* **Responsive design** for both desktop and mobile.
* **Light and dark mode** toggle.

---

## 🚀 Technologies Used

* **MongoDB**: NoSQL database for storing product information.
* **Express**: Backend web application framework for Node.js.
* **React**: Frontend library for building the user interface.
* **Node.js**: JavaScript runtime for the backend.
* **Chakra UI**: Component library for React to build accessible and modern web apps.
* **Zustand**: State management library for React.
* **Vite**: Frontend build tool.

---

## 🏁 Getting Started

### Prerequisites

* Node.js and npm installed on your machine.
* MongoDB connection URI.

### Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/Sujal-Dudhe/mern-product-store.git
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd mern-product-store
    ```
3.  **Install backend dependencies:**
    ```bash
    npm install
    ```
4.  **Install frontend dependencies:**
    ```bash
    npm install --prefix frontend
    ```
5.  **Create a `.env` file** in the `backend` directory and add your MongoDB connection string:
    ```
    MONGO_URI=<your_mongodb_uri>
    ```

---

## Run this app locally
```bash
    npm run build
```
## Start the app
```bash
    npm run start
```
---

## 🔧 API Endpoints

The following API endpoints are available:

| Method | Endpoint | Description |
| --- | --- | --- |
| `GET` | `/api/products` | Get all products. |
| `POST` | `/api/products` | Create a new product. |
| `PUT` | `/api/products/:id` | Update a product. |
| `DELETE` | `/api/products/:id` | Delete a product. |

---

## 📂 Project Structure
```bash
mern-product-store/
├── backend/                   # Backend (Node.js/Express)
│   ├── config/                # Configuration files
│   │   └── db.js              # MongoDB connection
│   ├── controllers/           # Business logic
│   │   └── product.controller.js
│   ├── models/                # Database models
│   │   └── Product.js         # Product schema
│   ├── routes/                # API endpoints
│   │   └── product.route.js
│   └── server.js             # Server entry point
│
├── frontend/                  # Frontend (React + Vite)
│   ├── public/                # Static assets
│   │   └── vite.svg
│   ├── src/                   # Source code
│   │   ├── assets/            # Images/icons
│   │   │   └── react.svg
│   │   ├── components/        # UI components
│   │   │   ├── Navbar.jsx
│   │   │   └── ProductCard.jsx
│   │   ├── pages/             # Page components
│   │   │   ├── CreatePage.jsx
│   │   │   └── HomePage.jsx
│   │   ├── store/             # State management
│   │   │   └── product.js     # Zustand store
│   │   ├── App.jsx            # Root component
│   │   └── main.jsx           # Entry point   
│   ├── eslint.config.js       # Linting config
│   ├── index.html             # Main HTML
│   ├── package.json           # Frontend dependencies
│   └── vite.config.js         # Vite config
│
├── .gitignore                # Global ignore rules
├── package.json              # Root dependencies
└── package-lock.json         # Lock file
```
