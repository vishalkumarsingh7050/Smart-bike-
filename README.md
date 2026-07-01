# Smart Public Bicycle Sharing System 🚴‍♂️

A full-stack, real-time bicycle sharing platform built with the MERN stack (MongoDB, Express.js, React, Node.js). This system features a smooth SaaS-style UI, interactive maps, and real-time availability updates.

## 🚀 Features

### For Users
- **SaaS-style Landing Page**: Modern, responsive introduction to the service.
- **Interactive Map**: Locate nearby bicycle stations using Leaflet.
- **Real-time Availability**: View live counts of available bikes at each station via Socket.io.
- **Easy Booking**: Book and start a ride with a single click.
- **Ride History**: Performance-optimized list of past and active journeys with cost calculation.
- **User Profile**: Personal dashboard with ride statistics and account info.

### For Admins
- **Analytics Dashboard**: High-level overview of users, stations, bicycles, and total rides.
- **Station Management**: Add new stations with geospatial coordinates.
- **Bicycle Management**: Add and assign bicycles to specific stations.

### Technical Features
- **JWT Authentication**: Secure login and registration with role-based access control.
- **Geospatial Queries**: MongoDB `2dsphere` indexing for location-based station searches.
- **Real-time Engine**: Socket.io integration for instant UI updates when bikes are rented or returned.
- **Mobile Friendly**: Responsive design with a dedicated mobile bottom navigation bar.

## 🛠 Tech Stack

- **Frontend**: React.js, Vite, Tailwind CSS, Lucide React (Icons), Leaflet (Maps), Axios.
- **Backend**: Node.js, Express.js, Socket.io.
- **Database**: MongoDB (Mongoose).
- **Authentication**: JSON Web Tokens (JWT), Bcrypt.js.

## 📋 Prerequisites

- Node.js (v16+)
- MongoDB (Running locally on `127.0.0.1:27017` or a MongoDB Atlas URI)
- npm or yarn

## 📂 Project Structure

```text
project-mohit/
├── backend/
│   ├── config/         # Database configuration
│   ├── controllers/    # API logic (Auth, Station, Bicycle, Ride)
│   ├── middleware/     # Auth & Error handling middleware
│   ├── models/         # Mongoose schemas
│   ├── routes/         # API endpoints
│   ├── utils/          # Helper functions (JWT generation)
│   └── server.js       # Entry point & Socket.io setup
├── frontend/
│   ├── src/
│   │   ├── components/ # Reusable UI components (Navbar, etc.)
│   │   ├── context/    # AuthContext for global state
│   │   ├── pages/      # Page components (Home, Dashboard, Profile, etc.)
│   │   ├── utils/      # API (Axios) configuration
│   │   └── App.jsx     # Routing setup
│   └── index.html
└── README.md
```

## 🛡 License

Distributed under the MIT License. See `LICENSE` for more information.
