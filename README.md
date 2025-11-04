# ✈️ Airport Management System

This project is a simple **Airport Management System** with **ticket booking** as its main feature.  
It was developed using **React** for the frontend and **Express.js** for the backend.  
For database operations, I used **Sequelize ORM**, which made it easier to manage queries and relationships.  
The system runs on **MySQL**, chosen because it’s simple, familiar, and performs well for read/write operations — making it suitable for transaction-based applications that might scale later.

---

## 🧩 Database Design

The database consists of several tables with defined relationships between them:

1. **Account** — Stores user account data.  
2. **Employee** — Stores airport employee data and links to the Account table.  
3. **Passenger** — Stores additional account information used for ticket purchases.  
4. **Airline** — Stores airline information.  
5. **Aircraft** — Stores aircraft data belonging to specific airlines.  
6. **Flight** — Stores flight schedules.  
7. **Ticket** — Stores tickets related to specific flights.  
8. **Booking** — Stores ticket purchase transactions made by passengers.  
9. **Departure** — Stores updated takeoff data and status for flights.  
10. **Arrival** — Stores updated landing data and status for flights.

---

## 🔗 Relationships

The database includes several **one-to-one** relationships, such as:
- `Account ↔ Employee`  
- `Account ↔ Passenger`  
- `Flight ↔ Arrival`  
- `Flight ↔ Departure`

These are modeled as one-to-one because each record in the related table corresponds to only one entry in the main table (the foreign key is unique).

The rest are **one-to-many** relationships — for example, one airline can have multiple aircraft, and one flight can have multiple tickets.

---

## ⚙️ Tech Stack

- **Frontend:** React  
- **Backend:** Express.js (Node.js)  
- **ORM:** Sequelize  
- **Database:** MySQL  

---

## 💡 Summary

This project helped me understand how to:
- Design and build relational databases for real-world use cases  
- Implement **one-to-one** and **one-to-many** relationships using Sequelize  
- Connect a React frontend with an Express backend  
- Work with MySQL efficiently in a transactional system  

---

## 👨‍💻 Author

**Choirul Anam**  
Computer Science Student — Software Engineering Fundamentals Assignment
