# Foodiego

Foodiego is a responsive online food delivery management system built with plain HTML, CSS, and JavaScript. The project demonstrates customer ordering and delivery tracking together with an admin dashboard for managing food items, categories, customers, and orders.

> This project is designed for a front-end academic/demo environment. It uses browser `localStorage` instead of a backend database or payment gateway.

## Features

### Customer module

- Customer signup and login
- Role-based navigation after login
- Browse food items by category
- Search by dish, restaurant, or cuisine
- Add food items to a cart
- Increase, decrease, and remove cart quantities
- Select delivery address
- Select a demo payment method
- Place orders
- Track order status through a delivery timeline
- View order history
- Submit ratings and reviews after delivery
- Logout

### Admin module

- Admin login
- Dashboard statistics for food items, orders, customers, and revenue
- Add food items
- Edit food items
- Delete food items
- Manage food categories
- View customer details
- View all customer orders
- Update order status:
  - Placed
  - Preparing
  - Out for delivery
  - Delivered
  - Cancelled

## Technology

This project intentionally uses only:

- HTML5
- CSS3
- Vanilla JavaScript
- Browser localStorage

No PHP, MySQL, React, Node.js, or external framework is required.

## Getting started

### Option 1: Open directly in a browser

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Use the navigation to create a customer account or open the login page.

### Option 2: Open through Visual Studio Code

1. Open the project folder in Visual Studio Code.
2. Open `index.html` in a browser using your preferred static HTML preview workflow.
3. No build command or package installation is required.

## Demo credentials

### Admin

- Email: `admin@kleats.com`
- Password: `admin123`

### Customer

Create a customer account from `register.html` or `signup.html`. Customer accounts are saved in the current browser's localStorage.

## Project structure

```text
Foodiego/
├── index.html       # Landing page and featured food
├── login.html       # Login and role-based redirect
├── register.html    # Customer registration
├── signup.html      # Signup compatibility entry point
├── user.html        # Customer dashboard
├── menu.html        # Searchable and filterable food menu
├── cart.html        # Cart and checkout
├── orders.html      # Order history, tracking, and reviews
├── admin.html       # Admin management dashboard
├── style.css        # Responsive layout, grid, flexbox, and animations
├── script.js        # Application logic and localStorage data model
└── README.md        # Project documentation
```

## localStorage data

Foodiego stores demo data in the browser using these localStorage keys:

- `kleats_users` — registered users and admin account
- `kleats_foods` — food catalogue
- `kleats_categories` — food categories
- `kleats_orders` — customer orders and status updates
- `kleats_reviews` — submitted ratings and reviews
- `kleats_session` — currently logged-in user
- `kleats_cart_<email>` — cart items for each logged-in user

To reset the demo, open the browser developer tools and clear localStorage for the page.

## Suggested demonstration flow

1. Open the landing page.
2. Register a customer account.
3. Log in as the customer.
4. Search or filter the menu.
5. Add two or more food items to the cart.
6. Update quantities and place an order.
7. Open **My orders** and show the tracking timeline.
8. Log out.
9. Log in using the admin credentials.
10. Add or edit a food item.
11. Update the order status to **Preparing**, **Out for delivery**, and **Delivered**.
12. Log in again as the customer and submit a review.

## Screenshot guidance

For a project review or presentation, capture these screens:

1. Landing page — hero section, categories, and popular dishes
2. Registration page — signup form
3. Customer dashboard — popular dishes and recent orders
4. Menu page — search and category filter in use
5. Cart page — selected items and checkout summary
6. Order tracking — delivery timeline and order details
7. Admin dashboard — statistics and food catalogue
8. Admin order management — status update controls
9. Review section — rating and comment after delivery
10. GitHub repository — committed project files and README

## Limitations

- Data is stored only in the current browser.
- Clearing browser storage removes demo accounts, carts, orders, and reviews.
- Payments are simulated and do not process real transactions.
- Authentication is intended for demonstration only and is not production-grade security.
- Restaurant data is represented by seeded sample restaurants and food items.

## License

This project is intended for educational and demonstration purposes.
