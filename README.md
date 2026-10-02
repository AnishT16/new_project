# Mini E-Commerce Demo Project

A complete Mini E-Commerce Demo Project built using the **MERN Stack** (MongoDB, Express.js, React.js, Node.js).

## Tech Stack
* **Frontend:** React.js + Vite + JavaScript
* **Styling:** Tailwind CSS
* **Backend:** Node.js + Express.js
* **Database:** MongoDB + Mongoose
* **Authentication:** JWT + bcrypt
* **API Calls:** Axios

## Features

### 1. Authentication
- JWT authentication with bcrypt for password hashing.
- Customer: Register, Login, Logout.
- Admin: Admin Login, JWT protected admin routes.

### 2. Admin Panel
- **Categories:** Add, edit, delete, view.
- **Products:** Add, edit, delete, view.
- **Orders:** View all customer orders, view details, change status (Pending, Confirmed, Shipped, Delivered, Cancelled).

### 3. Public Website
- Pages: Home, Products, Product Details, Cart, Checkout, Login, Register, My Orders.
- Products display (image, name, price, category, add to cart).
- Category filter and product search.

### 4. Cart & Checkout
- Add/remove products, adjust quantity (validated against stock).
- Checkout with Cash on Delivery.
- Order creation flow: Cart -> Validate Stock -> Create Order -> Save in DB -> Reduce Stock -> Clear Cart.

## Project Structure
```text
/client   → React frontend
/server   → Node.js + Express backend
```
