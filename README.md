# 🏨 Hotel Reservation System (Java + JDBC + MySQL)

A simple **console-based Hotel Reservation Management System** built using **Java, JDBC, and MySQL**.  
This project allows hotel staff to manage reservations (CRUD operations) from the terminal.

---

## ✨ Features
- **Reserve a Room** → Add a new reservation for a guest.
- **View Reservations** → Display all current reservations in a tabular format.
- **Get Room Number** → Find a guest's room number using reservation ID and guest name.
- **Update Reservation** → Modify guest details, room number, and contact info.
- **Delete Reservation** → Remove an existing reservation.
- **Exit System** → Graceful exit with countdown.

---

## 🛠️ Technologies Used
- **Java (JDK 21+)**
- **JDBC (Java Database Connectivity)**
- **MySQL (Database)**
- **Maven / IDE (IntelliJ / Eclipse / VS Code)**

---

## 📂 Database Setup
1. Create a database in MySQL:
   ```sql
   CREATE DATABASE hotel_db;
   USE hotel_db;


CREATE TABLE reservations (
    reservation_id INT AUTO_INCREMENT PRIMARY KEY,
    guest_name VARCHAR(100) NOT NULL,
    room_number INT NOT NULL,
    contact_number VARCHAR(20),
    reservation_date TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

