# Database Models

We use MongoDB with Mongoose.

## 1. User
- `name` (String, required)
- `email` (String, required, unique)
- `password` (String, required, min 6 chars)
- `role` (String, enum: ['customer', 'admin'], default: 'customer')

## 2. Category
- `name` (String, required)
- `description` (String)

## 3. Product
- `name` (String, required)
- `description` (String)
- `price` (Number, required, positive)
- `image` (String)
- `category` (ObjectId, ref: 'Category')
- `stock` (Number, required, non-negative)

## 4. Order
- `user` (ObjectId, ref: 'User')
- `products` (Array of objects containing product ObjectId and quantity)
- `totalAmount` (Number)
- `shippingAddress` (Object: Name, Phone, Address, City, Pincode)
- `status` (String, enum: ['Pending', 'Confirmed', 'Shipped', 'Delivered', 'Cancelled'], default: 'Pending')
- `createdAt` (Date, default: Date.now)
