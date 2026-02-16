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
Booked → Checked-In → Checked-Out
↘ Cancelled
### Front Desk Operations
- Check-in allowed only on booking date
- Check-out allowed after check-in
- Cancel reservation before arrival
### Analytics & Service Operations
- 7-day occupancy rate visualization
- Room service billing entry
- Daily operational dashboard for reception staff
- Real-time operational awareness for hotel management

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
### 🏠 Dashboard – Daily Operations & Occupancy
Displays:
- Guests checking in today
- Guests checking out today
- Room service section
- Occupancy rate visualization

![Dashboard](ScreenShots/Dashboard.png)

---

### 🛏 Room Management – Create Room
Allows Manager to:
- Add room number
- Configure adult & children capacity
- Set room pricing
- Assign amenities

![Create Room](ScreenShots/Create%20Rooms%20Preview.png)

---

### 📋 Room List – Inventory Overview
Displays:
- Room number
- Capacity (Adults / Children)
- Price per night
- Navigation to edit details

![Room List](ScreenShots/Rooms%20List%20Preview.png)

---

### 🧾 Booking Creation – Smart Availability Engine
Features:
- Guest information form
- Date validation
- Capacity validation
- "Get Available Room" logic

![Create Booking](ScreenShots/Create%20Bookings%20Preview.png)

---

### 📊 Booking List – Reservation Management
Includes:
- Search by guest name
- Filter by booking status
- Lifecycle tracking (Booked / Checked In / Checked Out)

![Booking List](ScreenShots/Bookings%20List%20Preview.png)

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
