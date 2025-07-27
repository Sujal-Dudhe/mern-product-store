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
mern-product-store/
├── backend/                  # Backend (Node.js/Express)
│   ├── config/
│   │   └── db.js             # MongoDB connection configuration
│   ├── controllers/
│   │   └── product.controller.js # Product business logic
│   ├── models/
│   │   └── Product.js        # Mongoose schema and model
│   ├── routes/
│   │   └── product.route.js  # API endpoints
│   └── server.js             # Server initialization
├── frontend/                 # Frontend (React + Vite)
│   ├── public/
│   │   └── vite.svg          # Vite logo
│   ├── src/
│   │   ├── assets/
│   │   │   └── react.svg     # React logo
│   │   ├── components/       # Reusable components
│   │   │   ├── Navbar.jsx    # Navigation bar
│   │   │   └── ProductCard.jsx # Product display card
│   │   ├── pages/            # Page components
│   │   │   ├── CreatePage.jsx # Product creation page
│   │   │   └── HomePage.jsx  # Main product listing page
│   │   ├── store/
│   │   │   └── product.js    # Zustand state management
│   │   ├── App.jsx           # Root component
│   │   └── main.jsx          # Entry point
│   ├── .gitignore
│   ├── eslint.config.js      # ESLint configuration
│   ├── index.html            # Main HTML template
│   ├── package-lock.json
│   ├── package.json          # Frontend dependencies
│   └── vite.config.js        # Vite configuration
├── .gitignore                # Global gitignore
├── package-lock.json
└── package.json              # Root project configuration
