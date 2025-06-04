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

/src
- ├── components/ # Reusable components (ChargerList, MapView)
- ├── pages/ # Route pages (Login, Signup, Dashboard)
- ├── context/ # AuthContext for global user state
- ├── utils/ # Base URLs, helpers



### Backend (`/backend`)

- /routes # Auth and Charger station routes
- /controllers # Logic for login, CRUD, user info
- /models # Mongoose schemas
- /middleware # Protect routes with JWT


## 🧪 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/charging-station-app.git
cd charging-station-app

Setup Backend
    cd backend
    npm install
    npm start

Setup Frontend
    cd frontend
    npm install
    npm run dev


🛡️ Security
JWT stored in httpOnly cookies for secure auth.

CORS configured for Vercel and Render.

Secure cookie setup: secure: true, sameSite: 'None'.

📌 Notes
The backend uses cookie-based auth; ensure HTTPS is used in production (e.g., on Vercel + Render).

Frontend automatically invalidates and refetches user state on login/logout using React Query.
