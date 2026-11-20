# The Reading Room

A browser-only bookstore demonstration built with HTML5, CSS3, and vanilla JavaScript. Browse 36 seeded books, search and filter the catalogue, save a wishlist, manage a cart, place demo Cash on Delivery orders, and manage inventory and orders in the demo admin room. All transactions and data are simulated locally.

## Run locally

1. Open this folder in VS Code.
2. Install the Live Server extension, then right-click `index.html` and choose **Open with Live Server**.
3. Register a demo account, or use one of the accounts below. Use the same browser and origin to retain data. Google Fonts, Open Library covers, and editorial photography require an internet connection; fallback fonts and generated covers are available offline.

**Demo customer:** `reader@readingroom.demo` / `Reader123!`  
**Demo admin:** `admin@readingroom.demo` / `Admin123!`

## Features

- Login, registration, account profile, remembered or session sign-in, and access checks.
- Search, category and price filters, sorting, load more, product details and related titles.
- Account-specific persistent cart and wishlist, stock checks, checkout, order history and demo order statuses.
- Admin inventory and category management, users, orders, status updates and local demo revenue.
- Responsive layouts, empty states, confirmation dialogs and feedback messages.

## Structure

- `*.html` — independent page entry points sharing the application shell.
- `css/style.css` — responsive design system and page styles.
- `js/storage.js` — seed data and storage utilities.
- `js/app.js` — rendering, validation, navigation and interactions.
- `assets/` — reserved for additional local images and icons.

## Local storage and limitations

The app initializes the catalogue only when `bookstore_books` does not exist. Data is stored under `bookstore_users`, `bookstore_current_user`, `bookstore_books`, `bookstore_cart`, `bookstore_wishlist`, `bookstore_orders`, and `bookstore_categories`. Cart and wishlist entries are keyed by user ID. An optional newsletter interest list uses `bookstore_newsletter`. Remembered sign-in uses localStorage; otherwise sign-in lasts for the browser session. Clearing browser storage resets demo data.

This is an educational frontend simulation. Passwords and admin access are stored and checked in the browser and are **not secure**. Do not use real or reused passwords, sensitive personal data, or payment details. No real payment is processed, order transmitted, email sent, or delivery arranged. Data is local to one browser/origin and may be modified or cleared by the user. External images and fonts depend on their providers and network availability.