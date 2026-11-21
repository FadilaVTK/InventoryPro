# InventoryPro

> A modern, responsive inventory and stock management web application built with React, Vite, and Tailwind CSS.

---

## 📋 Overview

**InventoryPro** is a lightweight yet feature-rich inventory management application designed to help small-to-medium businesses, warehouses, and individuals track, organize, and monitor stock levels in real time.

It provides a clean, modern glassmorphic interface with instant search, interactive stock metric dashboards, low-stock warnings, and persistent browser storage.

---

## ✨ Features

- **🔐 Authentication & Protected Routes**
  - Simulated credential-based authentication system.
  - Protected dashboard routes with automatic redirects for unauthorized users.
  - Session state stored in `localStorage` with one-click logout.

- **📊 Real-Time Analytics Dashboard**
  - **Total Items**: Live count of unique catalog products.
  - **Total Quantity**: Sum of all physical units in inventory.
  - **Total Inventory Value**: Calculated aggregate value in ₹ (INR).
  - **Categories**: Distinct category classification count.
  - **Low Stock Tracker**: Real-time counter of items requiring restock.

- **📦 Inventory Management (Full CRUD)**
  - **Add Items**: Fast creation flow with name, category, quantity, and unit price.
  - **Edit Items**: Seamless modal-based inline item editing.
  - **Delete Items**: Safe deletion with an interactive confirmation modal dialog.

- **⚠️ Low Stock Highlighting**
  - Items with &le; 5 units in stock are automatically flagged with warning tags and highlighted in soft red for quick visual prioritization.

- **🔍 Live Search & Filter**
  - Real-time search by product name with instantaneous list updates.

- **💾 Data Persistence**
  - Automatically synchronizes all inventory updates to browser `localStorage`.
  - Pre-seeded with starter data (`data.json`) for quick out-of-the-box evaluation.

- **🎨 Modern Glassmorphic UI**
  - Styled with Tailwind CSS v4, gradients, backdrop blur effects, smooth animations, and responsive mobile-first layouts.

---

## 🛠️ Tech Stack

- **Framework**: [React 19](https://react.dev/)
- **Build Tool**: [Vite 7](https://vite.dev/)
- **Routing**: [React Router DOM v7](https://reactrouter.com/)
- **Styling**: [Tailwind CSS v4](https://tailwindcss.com/) (`@tailwindcss/vite`)
- **Language**: JavaScript (ES Modules)
- **Linter**: ESLint 9

---

## 🚀 Getting Started

### Prerequisites

Ensure you have [Node.js](https://nodejs.org/) installed (version 18 or higher recommended).

### Installation

1. Clone or open the project repository:
   ```bash
   cd Projects
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open your browser and navigate to the local URL displayed in the terminal (typically `http://localhost:5173`).

---

## 🔑 Default Login Credentials

Use the following credentials on the login screen to access the dashboard:

| Field | Value |
| :--- | :--- |
| **Username** | `admin` |
| **Password** | `1234` |

---

## 📂 Project Structure

```text
├── public/                 # Static assets
├── src/
│   ├── assets/             # Images and SVG assets
│   ├── components/         # Reusable UI components
│   │   ├── ConfirmDialog.jsx # Modal confirmation dialog for deletions
│   │   ├── InventoryList.jsx # Inventory item list with status badges
│   │   ├── ItemForm.jsx      # Form for adding and editing products
│   │   ├── Login.jsx         # Sign-in screen with glassmorphic design
│   │   ├── Modal.jsx         # Accessible overlay modal wrapper
│   │   └── SearchBar.jsx     # Live keyword search input
│   ├── pages/
│   │   └── Dashboard.jsx     # Overview statistics and metrics cards
│   ├── utils/
│   │   └── localStorage.js   # Local storage sync utilities
│   ├── App.css
│   ├── App.jsx               # Route definitions and auth guards
│   ├── data.json             # Initial seed product catalog
│   ├── index.css             # Tailwind CSS imports & global styles
│   ├── InventoryApp.jsx      # Core dashboard layout and inventory state
│   └── main.jsx              # React DOM root entry point
├── eslint.config.js          # ESLint configuration
├── index.html                # Main HTML entry point
├── package.json              # Project dependencies and npm scripts
└── vite.config.js            # Vite configuration with Tailwind CSS plugin
```

---

## 📜 Available Scripts

In the project directory, you can run:

- `npm run dev`: Runs the app in development mode with Hot Module Replacement (HMR).
- `npm run build`: Compiles and bundles production-ready files into the `dist/` directory.
- `npm run preview`: Locally previews the production build.
- `npm run lint`: Runs ESLint to identify code style and syntax issues.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
