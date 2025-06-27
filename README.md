# 🍜 ChenEats

**ChenEats** is a full-stack food ordering platform inspired by services like SkipTheDishes or Uber Eats. This is a functioning **MERN stack Minimum Viable Product (MVP)** with fully working customer and restaurant experiences, complete with authentication, data persistence, real-time analytics, and order tracking.  

This project was developed with a focus on building an end-to-end product lifecycle: database design, backend API routing, frontend UX, and real-time feature integration.

---

## ⚙️ Technologies

- **Frontend:** React, Bootstrap, Axios, React Router, Cookie-based session handling
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (tested via Compass), Mongoose ODM
- **Dev Tools:** Postman, VS Code, MongoDB Compass
- **Architecture:** RESTful API, Component-based structure, Dev-only bypass routes for testing

---

## 📸 Web Site Overview

### 🧾 Login & Database

![Login Page](images/SignIn.jpg)  
- Dev Buttons to auto sign in and verify either employee or customer accounts  
- Standard login page (uses cookies for persistent sessions)

![MongoDB Collection](images/mongodbCollection.jpg)  
- MongoDB Compass overview of test data and collections  
- All main tables for restaurants, customers, orders, menus, and staff

---

## 👤 Customer Side Features

### 🏠 Homepage

![Customer Side Homepage](images/CustomerHome.jpg)  
- View all available restaurants  
- Access and monitor active orders  
- Sticky navigation bar for easy access throughout the app  

---

### 🍽️ Restaurant Menu & Order Page

![Customer Side Order](images/StoreMenuOrder.jpg)  
- Dynamic, responsive ordering page for a selected restaurant  
- Real-time carting system, with menu data from MongoDB  
- Uses cookies to track customer and order session

---

### ✅ Order Confirmation

![Customer Side Order Confirmation](images/CustOrderConfirmation.jpg)  
- Schedule pickup time  
- Choose between delivery or pickup  

---

### 📦 Order History

![Customer Side Order History](images/CustOrderHistory.jpg)  
- View all historical orders for the logged-in customer  
- Pulls from MongoDB based on user session and ID  

---

## 🍽️ Restaurant Side Features

### 📊 Dashboard Homepage

![Restaurant Side Homepage Dashboard](images/RestaurantsHome.jpg)  
- View real-time updates of current active orders  
- Access sticky nav bar site-wide for efficient navigation  
- Dashboard summary of restaurant operations  

---

### 🧾 Order Tracking

![Restaurant Order Tracking](images/ResponsiveOrderTracking.jpg)  
- Update order statuses (e.g., processing, ready, completed)  
- Dynamically changes based on staff-side interactions  

---

### 🧑‍🍳 Edit Menu

![Restaurant Side Menu Edit](images/EditMenuPage.jpg)  
- Ability to edit and update restaurant menu items  
- Includes dish names, descriptions, and prices  
- Updates reflect in real-time for customer viewing  

---

### 🧾 Restaurant Order History

![Restaurant Side Order History](images/RestaurantOrderHistory.jpg)  
- See full order history for the restaurant  
- Sorted and stored via MongoDB for staff-level access  

---

### 📈 Analytics

![Restaurant Analytics](images/AnalyticsPage.jpg)  
- Real-time summary of restaurant performance:  
  - Most popular menu items  
  - Net revenue calculations  
  - Peak ordering times (breakfast, lunch, dinner)  
- Filters available for Daily, Monthly, and Yearly breakdowns  

---

## 🧪 Dev Features & Testing Notes

- Dev buttons included for quick sign-in bypass for customer and restaurant views
- All routes protected by session cookies
- Designed for local testing with `localhost:8000` API endpoints
- MongoDB seeded with test data via Compass and tested using Postman

---

## 🗂️ Project Structure Overview

### 🖥 Frontend (React)
- `App.jsx` – Main router
- `routes/` – Contains all customer and employee page routes
- `.store/ThemeContext.jsx` – Used for cross-component state (IDs, sessions)
- Bootstrap + Tailwind for UI structure and styling

### 🛠 Backend (Express)
- `index.js` – Express app bootstrap
- `routes/` – API routes (e.g., `/customer`, `/staff`, `/order`)
- `services/database.service.js` – MongoDB connection logic

---
