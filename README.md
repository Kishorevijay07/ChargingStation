# ⚡ Charging Station Management App

A full-stack web application to manage Electric Vehicle (EV) charging stations. This platform enables users to log in, view available charging stations, filter them by parameters like connector type or status, and visualize them on a map. Admins can also onboard new chargers and perform CRUD operations.

## 🔗 Live Demo

- **Frontend:** [charging-station-frontend](https://charging-station-frontend-sage.vercel.app)
- **Backend:** [charging-station-backend](https://chargingstation-backend-1.onrender.com)

---

## 🚀 Features

### 👥 Authentication
- Secure login with JWT-based authentication using cookies.
- Session handling via `httpOnly`, `secure`, `sameSite=None` cookies.

### 🔌 Charger Management
- View all EV charging stations.
- Filter by:
  - Status (Active/Inactive)
  - Connector Type
  - Power Output
- Perform CRUD operations on chargers.

### 🗺️ Map Integration
- View chargers on a live map using OpenStreetMap.
- Clickable markers to display station info.

---

## 🛠️ Tech Stack

### Frontend
- **Framework:** React (Vite)
- **UI:** Tailwind CSS, Heroicons
- **State Management:** React Query
- **Routing:** React Router DOM
- **API Calls:** `fetch`

### Backend
- **Runtime:** Node.js + Express
- **Database:** MongoDB + Mongoose
- **Auth:** JWT + Cookies (`httpOnly`, `secure`, `sameSite`)
- **Deployment:** Render

---

## 📁 Project Structure

### Frontend (`/frontend`)
