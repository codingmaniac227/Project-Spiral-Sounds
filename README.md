# 🎵 Spiral Sounds 🎵

Welcome to **Spiral Sounds** — a full‑stack vinyl record store built with **Node.js, Express, SQLite, and Vanilla JavaScript**. This project combines a **dynamic frontend** with a **RESTful backend** to deliver a fully functioning e‑commerce‑style app where users can browse vinyl records by genre or search by title.



## This project highlights:

- **Express routing & middleware**

- **SQLite database integration**

- **RESTful API design**

- **Static file serving with Express**

- **Frontend consumption of backend data**



## ✨ Features

- **📀 Product Browsing**

&nbsp; - Displays a curated selection of vinyl albums with title, artist, price, and genre.

&nbsp; - Images for each album are dynamically loaded from the `/public/images` folder.



- **🔍 Search & Filter**

&nbsp; - A **search bar** filters albums by title, artist, or genre in real time.

&nbsp; - A **genre dropdown** dynamically populates from the database and filters albums when selected.



- **🌐 API-Driven Rendering**

&nbsp; - JavaScript fetches album data via `/api/products` and renders the product cards dynamically.

&nbsp; - The dropdown calls `/api/products/genres` to populate filter options.



- **🖱️ Event-Driven UI**

&nbsp; - Search input triggers real‑time filtering.

&nbsp; - Genre dropdown updates product display instantly when changed.



## 🧱 Key Backend Elements

- **✅ Express Router**

&nbsp; - `productsRouter` handles `/api/products` and `/api/products/genres`.

- **✅ Controllers**

&nbsp; - `getProducts()` & `getGenres()` manage SQL queries and send JSON responses.

- **✅ SQLite Database**

&nbsp; - `products` table stores all album info (title, artist, price, genre, etc.).

- **✅ Scripts**

&nbsp; - `createTable.js` → creates DB table.

&nbsp; - `seedTable.js` → seeds DB with sample vinyl data.

&nbsp; - `logTable.js` → logs DB contents for debugging.



## 🎨 Key Frontend Elements

- **📐 Dynamic Rendering**

&nbsp; - `index.js` fetches product JSON and dynamically builds product cards.

- **🎨 Styling**

&nbsp; - `index.css` uses clean, modern styles for the storefront layout.

- **🖼️ Images**

&nbsp; - All vinyl cover art and logos live in the `public/images` folder and are dynamically displayed.



## 🧠 Concepts Practiced

- **Express Basics**

&nbsp; - Serving static files, setting up routers, using middleware.

- **REST API Design**

&nbsp; - Created endpoints for `/api/products` and `/api/products/genres`.

- **SQL Queries**

&nbsp; - Used `SELECT`, `INSERT`, `DISTINCT` and `WHERE` clauses for flexible data retrieval.

- **Frontend-Backend Integration**

&nbsp; - Fetch API connects the frontend to the Express backend seamlessly.

- **Modular Structure**

&nbsp; - Split code into routes, controllers, and DB utilities for clarity.



## 🚀 Future Enhancements

- Add authentication for user accounts and carts.

- Implement Stripe or PayPal for **checkout and payments**.

- Add the ability to **add/remove items to a cart**.

- Deploy to a platform like Render, Railway, or Heroku for live demo access.



## 🪞 Reflection

This project represents my **transition from purely frontend apps** to **true full‑stack development**. It taught me:



- How to structure an Express project with routers and controllers.

- How to connect an SQLite database and write queries.

- How to serve a frontend and backend together in one app.



By building **Spiral Sounds**, I now have a **portfolio‑ready** example of a **real‑world full‑stack app** that combines everything I’ve learned so far — and sets the stage for future enhancements like authentication and payments.



