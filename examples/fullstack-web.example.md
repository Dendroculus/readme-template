<div align="center">

# 🏨 StayFlow

### A realtime hotel reservation platform for guests and staff

</div>

## 🚀 Why StayFlow

StayFlow combines guest booking, payment tracking, room availability, and an administrative dashboard in one application. Realtime events keep booking and room state synchronized between staff sessions.

## 🎯 Features

### Guest experience

- Account registration and JWT authentication
- Room search and availability checks
- Booking creation and cancellation
- Payment submission
- Self check-in and check-out
- Reviews

### Administration

- Room and room-type management
- Booking confirmation and lifecycle updates
- Guest management
- Payment-method management
- Revenue statistics

### Realtime

- Booking-created events
- Booking-status events
- Room-availability events
- Payment updates
- Staff presence

## 🧠 Architecture Highlights

- React owns page state, reusable hooks, and live updates
- Express owns REST routes and authorization
- Sequelize maps PostgreSQL entities
- Socket.IO delivers scoped realtime events
- PostgreSQL notifications can bridge database changes to sockets
- JWT protects guest and admin operations

## 🔄 Booking Flow

1. Guest checks dates and room type
2. Backend validates availability
3. Booking and selected services are stored transactionally
4. Staff clients receive a booking-created event
5. Payment and booking status update over time
6. Room availability is recalculated and broadcast

## ⚙️ Environment Variables

```env
# Backend
DATABASE_URL=
JWT_SECRET=
ALLOWED_ORIGINS=http://localhost:5173

# Frontend
VITE_API_URL=http://localhost:3000/api
VITE_SOCKET_URL=http://localhost:3000
```

## 🧪 Testing

```bash
npm --prefix backend test
npm --prefix frontend run lint
npm --prefix frontend run build
```
