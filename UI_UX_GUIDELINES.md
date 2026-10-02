# UI/UX & Validation Guidelines

## Styling
- **Framework:** Tailwind CSS
- **Design Principles:** Modern, clean, user-friendly, fully responsive (Mobile, Tablet, Desktop).
- **Components:** Cards, Responsive Navbar, Admin Sidebar, Admin Tables, Toast messages, Loading states, Empty states, Confirmation dialogs for delete.
- **Rule:** Keep UI simple and professional. Avoid over-designing.

## Validation & Security
### Frontend & Backend
- Required fields check.
- Valid email format.
- Password minimum 6 characters.
- Unique email constraint.
- Positive product price.
- Stock cannot be negative.
- Valid category references.

### Security specifics
- JWT Authentication and protected admin routes.
- Password hashing (bcrypt).
- **Critical:** Never trust the product price sent from the frontend. Fetch the current price from MongoDB when creating an order.
