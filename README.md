# Ready-To-Eat-Ordering-App
A browser-based food ordering prototype for a ready-to-eat food brand, with a **customer storefront** and an **admin dashboard**. Built with plain HTML, CSS and JavaScript. Data is stored in the browser using IndexedDB (no backend server).

## Features

**Customer side (`blossom-customer.html`)**
- Browse the menu by category, search items and use filters
- Item details pop-up, add to cart, change quantities
- Choose the order type, enter an address and place an order
- Register / log in and view your order history

**Admin side (`blossom-admin.html`)**
- Admin login
- Dashboard with order statistics
- View all orders, filter them and open order details
- Update order status
- View customers and their orders

## Tech stack
HTML · CSS · JavaScript (vanilla) · IndexedDB

## How to run
1. Download or clone this repository.
2. Start a local server in the folder so both pages share the same browser storage:
   ```
   python -m http.server 8000
   ```
3. Open `http://localhost:8000/blossom-customer.html` to order, and `http://localhost:8000/blossom-admin.html` for the admin view.

Demo admin login: `admin@blossom.com` / `admin123`

## Limitations and future work
- Data lives only in the browser's IndexedDB, so it is not shared between devices.
- Passwords are stored in plain text for demo purposes. A real version needs hashed passwords and server-side authentication.
- Planned: a Node.js + Express backend with a MySQL database, secure sessions and online payments.
## Note
This is a learning/demo project. The brand name, logo and images belong to their respective owners and are used here for demonstration only.
