# 🍔 Food Ordering System

A full-featured food ordering web application built with React, TypeScript, and Vite. Includes customer, restaurant, admin, and driver dashboards.

---

## Features

- **Customer App**
  - Browse restaurants and menus
  - Add items to cart and checkout
  - Payment method selection (card / cash)
  - Order tracking and order history
  - User profile management
  - Restaurant registration request

- **Restaurant Dashboard**
  - Order management (Pending → Confirmed → Preparing → Ready → Out for Delivery → Completed / Canceled)
  - Menu item management (add, edit, delete)
  - Category management
  - Restaurant profile & overview

- **Admin Dashboard**
  - Manage all restaurants and registration requests
  - User management (add users, roles, permissions)
  - Earnings overview
  - System settings

- **Driver Dashboard**
  - Delivery management with map integration (Leaflet / Google Maps)

---

## Tech Stack

| Technology | Purpose |
|---|---|
| React 18 | UI Library |
| TypeScript | Type Safety |
| Vite | Build Tool |
| Tailwind CSS | Styling |
| React Router DOM v7 | Routing |
| TanStack React Query | Server State |
| Zustand | Client State |
| Axios | HTTP Client |
| Framer Motion | Animations |
| Leaflet / React Google Maps | Maps |
| JWT Decode | Authentication |
| Yup | Form Validation |
| React Toastify / Sonner | Notifications |

---

## Prerequisites

- **Node.js** >= 18
- **Yarn** (recommended) or npm

---

## Getting Started

### 1. Clone the Repository

```bash
git clone <repository-url>
cd Food_Ordering_System
```

### 2. Install Dependencies

```bash
yarn install
```

### 3. Run the Development Server

```bash
yarn dev
```

The app will be available at `http://localhost:5173`

### 4. Build for Production

```bash
yarn build
```

### 5. Preview Production Build

```bash
yarn preview
```

### 6. Lint

```bash
yarn lint
```

---

## Project Structure

```
src/
├── components/        # Reusable UI components
│   ├── Home/          # Homepage sections (Hero, Features, Reviews, etc.)
│   ├── Payment/       # Payment-related components
│   ├── UI/            # Shared UI components (NavBar, Footer, Cards, etc.)
│   ├── admin/         # Admin dashboard components
│   └── restaurants/   # Restaurant dashboard components
├── context/           # React Context providers (Auth, Cart, Driver)
├── pages/             # Page components
│   ├── admin/         # Admin pages
│   ├── restaurants/   # Restaurant pages
│   └── Drivers/       # Driver pages
├── config/            # App configuration
├── constants/         # Constants (routes, etc.)
├── schema/            # Yup validation schemas
├── types/             # TypeScript type definitions
├── utils/             # Utility functions and API helpers
└── assets/            # Fonts and images
```

---

## Key Routes

| Route | Description |
|---|---|
| `/` | Home page |
| `/signin` | Sign in |
| `/signup` | Sign up |
| `/restaurants` | Browse restaurants |
| `/restaurant/:id/menu` | Restaurant menu |
| `/cart` | Shopping cart |
| `/checkout` | Checkout |
| `/orders` | Order history |
| `/account` | User profile |
| `/resturent-dashboard/*` | Restaurant dashboard |
| `/admin-dashboard/*` | Admin dashboard |
| `/driver-dashboard/*` | Driver dashboard |

---

## Environment Variables

Create a `.env` file in the root directory and add the required variables:

```env
VITE_API_BASE_URL=your_backend_api_url
VITE_GOOGLE_MAPS_API_KEY=your_google_maps_api_key
```

---

## License

This project is for educational purposes.
