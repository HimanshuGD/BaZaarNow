# 🛒 E-Commerce Backend API

This is a **Node.js + Express** backend for an e-commerce platform that sells mobile phones. The API supports core features such as product listings, user authentication, cart management, order processing, and a mock payment system. It follows **SOLID principles**, uses clean code architecture, and supports pagination for both products and order history.

---

## 🚀 Features

- ✅ Product listing with pagination
- 🔍 Product detail view
- 👤 User registration and login
- 🛒 Cart management
- 📦 Order placement and history
- 💳 Mock payment processing
- 🔐 Simple authentication (header-based)
- ✅ Clean architecture with service separation
- 🧪 Basic error handling and modular design

---

## 🧱 Tech Stack

- **Node.js**
- **Express.js**
- **In-memory storage** (for simplicity)
- **Postman** for API testing

---


Each folder contains a modular service class for handling business logic related to its domain.

---

## 🧪 API Endpoints

### 🔹 Product

| Method | Endpoint               | Description               |
|--------|------------------------|---------------------------|
| GET    | `/api/products?page=1` | List all products (paginated) |
| GET    | `/api/products/:id`    | Get product detail by ID  |

### 🔹 User

| Method | Endpoint            | Description       |
|--------|---------------------|-------------------|
| POST   | `/api/users/register` | Register user     |
| POST   | `/api/users/login`    | Login user        |

### 🔹 Cart

| Method | Endpoint      | Description            |
|--------|---------------|------------------------|
| POST   | `/api/cart`   | Add product to cart    |
| GET    | `/api/cart`   | View user cart         |

### 🔹 Order

| Method | Endpoint         | Description                        |
|--------|------------------|------------------------------------|
| POST   | `/api/orders`    | Place order (from cart)            |
| GET    | `/api/orders`    | View user's order history (paginated) |

### 🔹 Payment

| Method | Endpoint            | Description          |
|--------|---------------------|----------------------|
| GET    | `/api/test-payment` | Simulated payment    |

---

## 🖼️ Postman Screenshots

### 📦 List of Products
![alt text](/backend/postman/1.png)

### 🔍 Particular Product
![alt text](/backend/postman/2.png)

### 📝 User Registration
![alt text](/backend/postman/3.png)

### 🔐 User Login
![alt text](/backend/postman/4.png)

### 🛒 Add to Cart
![alt text](/backend/postman/5.png)

### 🧾 View Cart
![alt text](/backend/postman/6.png)

### ✅ Place Order
![alt text](/backend/postman/7.png)

### 📜 View Orders
![alt text](/backend/postman/8.png)

### 💳 Payment Success
![alt text](/backend/postman/9.png)

---

## 🔐 Authentication

For protected routes like `/api/cart` and `/api/orders`, add a header:
```http
user_id: your_user_id


