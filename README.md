# 🏖️ Beach Resort - Hotel Room Booking System

A modern full-stack hotel room booking and management platform that enables customers to search, reserve, and manage hotel rooms while providing administrators with powerful management tools for handling rooms, bookings, users, and reviews.

---

## 🚀 Project Overview

Beach Resort is a comprehensive hotel reservation system developed using the MERN ecosystem and modern frontend technologies. The platform offers seamless room booking experiences for customers and a dedicated administration dashboard for hotel management operations.

The application focuses on security, scalability, responsive design, and efficient booking management.

---

## ✨ Features

### 🔐 Authentication & Authorization

* User Registration and Login
* JWT Authentication
* Refresh Token Support
* Email Verification
* Password Recovery & Reset
* Role-Based Access Control (Admin/User)
* Account Status Management

### 🏨 Room Management

* Create, Update, Delete Rooms
* Room Categorization
* Featured Rooms
* Room Availability Tracking
* Room Image Uploads
* Advanced Search & Filtering
* Pricing & Capacity Management

### 📅 Booking Management

* Real-Time Room Booking
* Date Validation
* Booking Status Tracking
* Booking History
* Booking Cancellation
* Administrative Booking Controls

### ⭐ Review & Rating System

* Room Reviews
* Star Ratings
* Review Editing
* Review Management
* Average Rating Calculation

### 👥 User Management

* User Profile Management
* Avatar Uploads
* User Role Assignment
* User Blocking/Unblocking
* Account Administration

### 📊 Admin Dashboard

* Total Users Statistics
* Room Statistics
* Booking Analytics
* Dashboard Reports
* User Monitoring
* Inventory Management

---

## 🛠️ Technology Stack

### Frontend

* Next.js 13
* React 18
* Redux Toolkit
* Ant Design
* Styled Components
* Axios
* Day.js
* React Icons

### Admin Dashboard

* React 18
* Redux Toolkit
* Tailwind CSS
* Ant Design
* React Router DOM
* React CountUp

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT
* Bcrypt.js
* Multer
* SendGrid
* Winston
* Morgan
* Helmet
* Express Rate Limit

---

## 🏗️ System Architecture

```text
Frontend (Next.js)
        │
        ▼
Backend API (Express.js)
        │
        ▼
MongoDB Database
        │
        ▼
Admin Dashboard (React.js)
```

---

## 📂 Project Structure

```bash
Beach-Resort/
│
├── backend/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   └── services/
│
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── redux/
│   └── styles/
│
├── admin-panel/
│   ├── components/
│   ├── pages/
│   ├── redux/
│   └── routes/
│
└── README.md
```

---

## 🗄️ Database Models

### User

```javascript
{
  userName,
  fullName,
  email,
  phone,
  password,
  avatar,
  role,
  verified,
  status
}
```

### Room

```javascript
{
  room_name,
  room_type,
  room_price,
  room_capacity,
  featured_room,
  room_images,
  room_status
}
```

### Booking

```javascript
{
  room_id,
  booking_dates,
  booking_status,
  booking_by
}
```

### Review

```javascript
{
  user_id,
  room_id,
  rating,
  message
}
```

---

## 🔌 REST API Endpoints

### Authentication

```http
POST /api/v1/auth/registration
POST /api/v1/auth/login
POST /api/v1/auth/logout
POST /api/v1/auth/forgot-password
POST /api/v1/auth/reset-password/:token
POST /api/v1/auth/change-password
POST /api/v1/auth/verify-email/:token
GET  /api/v1/auth/refresh-token
```

### Rooms

```http
GET    /api/v1/all-rooms-list
GET    /api/v1/get-room-by-id-or-slug-name/:id
GET    /api/v1/featured-rooms-list
POST   /api/v1/create-room
PUT    /api/v1/edit-room/:id
DELETE /api/v1/delete-room/:id
```

### Bookings

```http
POST /api/v1/placed-booking-order/:id
GET  /api/v1/get-user-booking-orders
PUT  /api/v1/cancel-booking-order/:id
GET  /api/v1/get-all-booking-orders
PUT  /api/v1/updated-booking-order/:id
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/yourusername/beach-resort.git
cd beach-resort
```

### Install Backend

```bash
cd backend
npm install
```

### Install Frontend

```bash
cd frontend
npm install
```

### Install Admin Dashboard

```bash
cd admin-panel
npm install
```

---

## 🔑 Environment Variables

### Backend (.env)

```env
PORT=5000
MONGODB_URI=your_mongodb_uri
JWT_SECRET=your_secret_key
SENDGRID_API_KEY=your_sendgrid_key
```

### Frontend (.env.local)

```env
NEXT_PUBLIC_API_URL=http://localhost:5000/api/v1
```

---

## ▶️ Run Application

### Backend

```bash
npm run dev
```

### Frontend

```bash
npm run dev
```

### Admin Dashboard

```bash
npm start
```

---

## 🔒 Security Features

* JWT Authentication
* Password Hashing (Bcrypt)
* Role-Based Access Control
* Input Validation
* Rate Limiting
* Secure File Uploads
* Helmet Security Headers
* Protected Routes

---

## 📱 Responsive Design

The platform is fully optimized for:

* Desktop Devices
* Tablets
* Mobile Phones
* Large Screens

---

## 🧪 Testing

```bash
npm test
npm run coverage
```

### Linting

```bash
npm run lint
```

---

## 🚀 Deployment

### Frontend

* Vercel
* Netlify

### Backend

* Railway
* Render
* AWS
* Heroku

### Database

* MongoDB Atlas

---

## 👨‍💻 Author

**Md. Samiur Rahman (Mukul)**

* GitHub: https://github.com/SamiurRahmanMukul
* LinkedIn: https://linkedin.com/in/SamiurRahmanMukul
* Email: [contact@srmukul.com](mailto:contact@srmukul.com)

---

## 📄 License

Licensed under the ISC License.

---

## ⭐ Support

If you found this project useful, consider giving it a star on GitHub.

⭐ Star the repository to support future development.
