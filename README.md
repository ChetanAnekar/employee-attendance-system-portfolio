# Employee Attendance & Geofencing System

A production-ready, real-time employee attendance tracking system with GPS-based geofencing, photo verification, and comprehensive admin analytics. Built with Node.js, MongoDB, and vanilla JavaScript.

---

## 🎯 Project Overview

This is a full-stack attendance system that prevents buddy punching through:

- **GPS Geofencing**: Employees can only check in/out within authorized locations
- **Photo Verification**: Camera capture during check-in for identity confirmation
- **Real-Time Tracking**: Live map showing all checked-in employees
- **Auto-Checkout**: Automatic session termination after 14 hours
- **Cloud Storage**: Photos auto-upload to Cloudinary with 48-hour retention

---

## ✨ Key Features

### 🔐 Multi-Role Authentication
- **Admin Portal**: Full system management and oversight
- **Employee Portal**: Personal dashboard with attendance history
- JWT-based authentication with 8-hour session tokens

### 📍 Geofencing & Location
- **Multiple Work Locations**: Define geofence zones with custom radii
- **GPS Validation**: Real-time location verification during check-in/out
- **Interactive Maps**: Built with Leaflet.js showing employee positions
- **Distance Calculation**: Haversine formula for accurate proximity detection

### 📸 Photo Verification
- **Camera Integration**: HTML5 Media API for direct photo capture
- **Cloudinary Storage**: Automatic upload with privacy-focused auto-deletion
- **Base64 Compression**: Client-side image optimization before upload

### 📊 Real-Time Dashboard
- **Live Status**: See who's checked in/out at a glance
- **Attendance Analytics**: Days present, hours worked, performance metrics
- **Recent Activity Feed**: Timestamped log of all actions with photos
- **Export Ready**: Data structured for Excel/PDF reporting

### 🤖 Automated Processes
- **Auto-Logout**: Employees auto-checked-out after 14 hours
- **Photo Cleanup**: Cloudinary storage cleared every 48 hours
- **Data Retention**: Secure, temporary photo storage for privacy compliance

---

## 🛠️ Technology Stack

| Technology | Purpose |
|------------|---------|
| **Node.js + Express** | RESTful API backend server |
| **MongoDB + Mongoose** | NoSQL database for users, logs, locations |
| **JWT** | Secure token-based authentication |
| **Cloudinary** | Cloud storage for verification photos |
| **Leaflet.js** | Interactive mapping and geofence visualization |
| **HTML5 Geolocation API** | Browser-based GPS tracking |
| **HTML5 Media API** | Camera access for photo capture |
| **bcryptjs** | Password hashing (10 rounds) |
| **node-cron** | Automated scheduled tasks |

---

## 📐 System Architecture
