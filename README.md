# ☕ KapeRest UI

A modern, responsive frontend dashboard for the **KapeRest Café Management System**. Built with a focus on speed, type-safety, and intuitive user experience.

[Explore Backend Repository](https://github.com/Jesc06/KapeRest.Api.git)

## Core Features

* **Point-of-Sale (POS):** Streamlined interface for rapid order processing.
* **Inventory Tracking:** Real-time stock monitoring with low-inventory alerts.
* **Business Analytics:** Interactive dashboard for sales trends and insights.
* **Payment Integration:** Ready for digital payments (GCash integration).
* **Role-Based UI:** Dynamic navigation based on user permissions (Admin/Staff).

## Tech Stack

* **Core:** React 18 (Vite)
* **Language:** TypeScript
* **Styling:** Tailwind CSS
* **Routing:** React Router 6
* **State & Logic:** React Context API & Axios
* **Icons:** Lucide React

## 🚀 Quick Start

### Prerequisites

* Node.js (LTS Version)
* Running [KapeRest Backend API](https://github.com/Jesc06/KapeRest.Api.git)

### Installation

1. **Clone & Install**
```bash
git clone https://github.com/your-username/KapeRest.UI.git
cd KapeRest.UI
npm install

```


2. **Environment Setup**
Create a `.env` file in the root:
```env
VITE_API_BASE_URL=https://localhost:5001/api

```


3. **Run Development**
```bash
npm run dev

```



## 📂 Project Structure

```text
src/
├── components/   # Atomic & Reusable UI elements
├── pages/        # Main view containers
├── services/     # API integration (Axios instances)
├── context/      # Global state management
├── hooks/        # Custom business logic hooks
└── types/        # TypeScript interfaces/contracts

```


> **Development Note:** This UI is designed to work seamlessly with the KapeRest ASP.NET Core API, utilizing JWT-based authentication for all secure requests.

---

Built with ❤️ by Joshuaesc
