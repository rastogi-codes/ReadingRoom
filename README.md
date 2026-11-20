# The Reading Room

**The Reading Room** is a responsive, frontend-only online bookstore built with HTML5, CSS3, and vanilla JavaScript. It lets readers explore books, manage a wishlist and cart, and place simulated orders. A demo admin dashboard provides local inventory and order management.

> This project is an educational demonstration. It does not process real payments or place real orders.

## Features

### Reader experience

- Register, sign in, edit a profile, and sign out.
- Browse a catalogue initially populated with 36 books across nine categories.
- Search by title or author, filter by category or price, and sort results.
- View book details, ratings, descriptions, availability, and related titles.
- Add books to a wishlist or cart and update cart quantities.
- Complete a simulated Cash on Delivery checkout and view order history.
- Keep carts and wishlists separate for each demo account.

### Demo admin dashboard

- View book, user, order, and demo revenue totals.
- Add, edit, and delete books; update their prices and stock.
- Add, rename, and delete categories.
- View registered users and update demo order statuses.

The interface also includes responsive layouts, form validation, confirmation dialogs, toast notifications, and empty states.

## Built With

- **HTML5** - page structure
- **CSS3** - styling and responsive layouts
- **Vanilla JavaScript (ES6+)** - application logic and interactions
- **localStorage and sessionStorage** - browser-side demo data and sign-in state

No frontend framework, backend, database server, or package installation is required.

## Getting Started

1. Download the project or clone your repository and open the project folder in **Visual Studio Code**.
2. Install the **Live Server** extension in VS Code.
3. Right-click `index.html` and select **Open with Live Server**.
4. Register a demo account or sign in with one of the accounts below.

Use the same browser and local server address to retain saved data. Book covers, fonts, and editorial photographs load from external services; fallback covers and fonts are provided.

## Demo Accounts

| Account | Email | Password |
| --- | --- | --- |
| Customer | `reader@readingroom.demo` | `Reader123!` |
| Admin | `admin@readingroom.demo` | `Admin123!` |

## Project Structure

```text
The_Reading_Room/
├── index.html
├── login.html
├── register.html
├── home.html
├── books.html
├── book-details.html
├── cart.html
├── wishlist.html
├── checkout.html
├── orders.html
├── profile.html
├── admin.html
├── 404.html
├── css/
│   └── style.css
├── js/
│   ├── storage.js
│   └── app.js
├── assets/
│   ├── images/
│   └── icons/
└── README.md
```

## Browser Storage

The application stores demo records under these keys:

- `bookstore_users` and `bookstore_current_user`
- `bookstore_books` and `bookstore_categories`
- `bookstore_cart` and `bookstore_wishlist`
- `bookstore_orders`
- `bookstore_newsletter` for saved demo newsletter interest

Cart and wishlist data are keyed by user ID. The catalogue is seeded only when the books key is absent. **Remember me** stores sign-in state in localStorage; otherwise, sessionStorage is used. Clearing browser storage removes the demo data.

## Limitations

- Authentication and admin access are simulated in the browser and are **not secure**. Do not use real or reused passwords or sensitive personal data.
- Orders, Cash on Delivery, newsletter sign-ups, and revenue are demonstrations. No payment is collected, email sent, or delivery arranged.
- Data belongs to the current browser and origin; it is not shared across devices.
- External images and fonts depend on network availability.

## Project Team

- **Krishna Rastogi** - SAP ID: 1000024309
- **Ravneesh Singh** - SAP ID: 1000024245
- **Deepanshu Yadav** - SAP ID: 1000025573

**Course:** Front-End Engineering (CSN 371)  
**Institution:** DIT University, Dehradun  
**Guide:** Dr. Kamta Shukla
