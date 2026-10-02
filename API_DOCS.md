# REST API Documentation

## Authentication
- `POST /api/auth/register` : Register a new customer
- `POST /api/auth/login` : Login user/admin

## Categories
- `GET /api/categories` : Get all categories
- `POST /api/categories` : Create a new category (Admin)
- `PUT /api/categories/:id` : Update a category (Admin)
- `DELETE /api/categories/:id` : Delete a category (Admin)

## Products
- `GET /api/products` : Get all products. Supports query parameters: `?category=electronics&search=phone`
- `GET /api/products/:id` : Get single product details
- `POST /api/products` : Add a new product (Admin)
- `PUT /api/products/:id` : Update a product (Admin)
- `DELETE /api/products/:id` : Delete a product (Admin)

## Orders
- `POST /api/orders` : Create a new order (Checkout)
- `GET /api/orders/my-orders` : Get logged-in user's orders
- `GET /api/admin/orders` : Get all orders (Admin)
- `PATCH /api/admin/orders/:id/status` : Update order status (Admin)
