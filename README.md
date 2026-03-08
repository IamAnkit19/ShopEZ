# ShopEZ – Premium MERN Ecommerce Application

ShopEZ is a high-end, full-stack ecommerce platform built with the MERN stack. It features a completely custom, stunning dark-mode aesthetic utilizing glassmorphism and smooth micro-animations. It includes a dynamic product catalog, an immersive split-screen authentication flow, order tracking, and a fully stylized admin dashboard.

## 🚀 Tech Stack

- **Frontend**: React + Vite, React Router DOM, Tailwind CSS (Custom Design System)
- **Backend**: Node.js, Express, Mongoose
- **Database**: MongoDB (Local or Atlas)
- **Authentication**: JWT (JSON Web Tokens) & bcryptjs

## 📁 Project Structure

- `Server/` – Express API (models, controllers, routes, middleware)
- `Client/` – React SPA (pages, components, context, styling)

## ✨ Premium Features

- **Stunning UI/UX**: Custom `glass-card` design system with dynamic gradients, hover effects, and modern typography (sans-serif).
- **Dynamic HomePage** (`/`): Immersive hero section with real-time "Featured Products" fetched from the backend.
- **Immersive Authentication** (`/login`, `/register`): Dedicated 100vh split-screen layouts with animated background abstract art and centered authentication cards.
- **Product Catalog** (`/products`): Browse items with hover-reveal add-to-cart functionality and image fallbacks.
- **Advanced Cart System** (`/cart`): Fully backend-synced cart with realtime quantity updates, subtotals, and seamless removal.
- **Checkout Flow** (`/checkout`): Multi-step inspired modern layout covering shipping and stylized payment methods.
- **User Profile & Orders** (`/profile`, `/orders`): Check your account details and track order status with beautiful cards.
- **Premium Admin Console** (`/admin`):
  - Glowing metric cards for total items and orders.
  - Organized, custom-scrollbar data tables for tracking customer purchases.
  - Layered product creation forms.

---

## 🛠️ Installation & Setup

### 1. Backend Setup (`Server`)

1. Navigate to the `Server` directory:
```bash
cd Server
```

2. Create a `.env` file from the example:
```bash
cp .env.example .env
```
Update `.env` with at least:
- `MONGODB_URI` – your MongoDB connection string
- `JWT_SECRET` – any long random string

3. Install dependencies:
```bash
npm install
```

4. **Seed the Database** (Highly Recommended):
This will insert the primary admin user and sample products so you can immediately see the UI.
```bash
npm run seed
```
- Admin Email: `admin@shopez.local`
- Admin Password: `admin123`

5. Start the backend Server:
```bash
npm run dev
```
The API will run on `http://localhost:5000`.

### 2. Frontend Setup (`Client`)

1. Navigate to the `Client` directory:
```bash
cd Client
```

2. Create a `.env` file from the example:
```bash
cp .env.example .env
```
*By default `VITE_API_BASE_URL` is configured to `http://localhost:5000/api`.*

3. Install dependencies:
```bash
npm install
```

4. Start the Vite React app:
```bash
npm run dev
```
The application will run on `http://localhost:5173`. Open this in your browser to experience ShopEZ.

---
*Note: Payments are currently simulated visually. Orders are instantly marked as confirmed and saved to the database.*
