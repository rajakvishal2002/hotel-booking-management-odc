# 🏨 Hotel Booking Management System (OutSystems ODC)

A full-stack low-code web application that simulates a real hotel Property Management System (PMS).  
The system manages room inventory, guest reservations, availability validation, and operational workflows such as check-in and check-out.

Built using **OutSystems Developer Cloud (ODC)** with relational data modeling and SQL-based business logic.

---

## 🚀 Live Business Scenario

Hotels must prevent double bookings, manage guest flow, and track room occupancy daily.

This application solves:

• Room allocation  
• Availability detection  
• Booking lifecycle management  
• Front desk operations  
• Daily arrivals & departures dashboard  

---

## 🧠 Core Features

### Room Management
- Create, update and maintain rooms
- Capacity and price configuration
- Room amenities support

### Smart Booking Engine
- Automatic cheapest available room detection
- Overlapping booking prevention
- Capacity validation (Adults + Children)
- Date validation rules

### Booking Workflow

### Front Desk Operations
- Check-in allowed only on booking date
- Check-out allowed after check-in
- Cancel reservation before arrival

### Dashboard
Shows:
- Guests arriving today
- Guests leaving today

---

## 🏗 System Architecture

### Entities
| Entity | Purpose |
|------|------|
| Room | Hotel room inventory |
| Booking | Guest reservation |
| Status | Booking lifecycle state |
| Amenities | Room facilities |
| RoomService | Extra services |

---

## 🔐 Roles & Authorization

| Role | Permissions |
|----|----|
| Manager | Full control |
| Clerk | Operational tasks only |

---

## ⚙️ Business Logic Implemented

### Availability Validation (SQL Logic)
- Prevents overlapping bookings
- Filters cancelled reservations
- Validates room capacity

### Data Validation Rules
- Check-out date must be after check-in
- At least one adult required
- Children cannot be negative
- Room cannot be double-booked

---

## 🛠 Tech Stack

**Platform**
- OutSystems Developer Cloud (ODC)

**Backend Logic**
- SQL Queries
- Aggregates
- Server Actions

**Frontend**
- Reactive Web UI
- Role-based navigation

**Concepts Applied**
- Transaction workflow
- State machine logic
- Data integrity validation
- Business rule enforcement

---

## 📸 ScreenShots
Screenshots are available in ScreenShot folder you can find there.

---

## 📂 Project Structure
hotel-booking-management-odc
├── odc-export
│ └── HotelBookingSystem.oml
├── ScreenShots
└── README.md

---

## 🎯 Learning Outcomes

- Designed relational database schema
- Implemented real business workflows
- Wrote SQL for real-world constraints
- Applied role-based authorization
- Built transactional UI application

---

## 👨‍💻 Author

**Vishal Rajak**

---

## 📥 How to Run

1. Download `.oml` file from `odc-export`
2. Open in OutSystems Service Studio
3. Publish module
4. Run application

---

## ⭐ If you found this useful
Give the repository a star — it helps visibility!
