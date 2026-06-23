# 🚖 OLA Ride-Booking Data Analysis Project

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Excel](https://img.shields.io/badge/Microsoft%20Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)

## 📌 Project Overview

An end-to-end data analysis project on **OLA ride-booking data** for Bengaluru city (July 2024). The project involves SQL-based data extraction and a multi-page interactive Power BI dashboard covering booking trends, revenue patterns, cancellation analysis, and customer/driver ratings.

---

## 📊 Dashboard Pages

| Page | Key Visuals |
|------|-------------|
| **Overall** | Ride Volume Over Time, Booking Status Breakdown |
| **Vehicle Type** | Booking Value, Success Value, Avg & Total Distance by Vehicle |
| **Revenue** | Revenue by Payment Method, Top 5 Customers, Daily Ride Distance |
| **Cancellation** | Cancellation reasons by Customer & Driver |
| **Ratings** | Driver Ratings & Customer Ratings by Vehicle Type |

---

## 📸 Dashboard Screenshots

### Overall View
![Overall](screenshots/overall.png)

### Vehicle Type View
![Vehicle Type](screenshots/vehicle_type.png)

### Revenue View
![Revenue](screenshots/revenue.png)

### Cancellation View
![Cancellation](screenshots/cancellation.png)

### Ratings View
![Ratings](screenshots/ratings.png)

### SQL Queries (MySQL Workbench)
![SQL](screenshots/sql_workbench.png)

---

## 🔑 Key Insights

- **Total Bookings:** 20,407 | **Total Booking Value:** ₹7M
- **Booking Success Rate:** ~62% of all rides completed successfully
- **Cancellation Rate:** 28.10% — top reason by customers: *"Driver not moving towards pickup"* (29.31%)
- **Top Driver Cancellation Reason:** *"Personal & Car related issues"* (34.56%)
- **Revenue:** Cash dominates at ₹3.8M, followed by UPI at ₹2.8M
- **Ratings:** All vehicle types consistently rated between 3.98–4.02 by both drivers and customers
- **E-Bike** had the highest success booking value (₹995K) among all vehicle types

---

## 🗄️ SQL Analysis

10 business queries answered using **MySQL Views**:

1. Retrieve all successful bookings
2. Average ride distance per vehicle type
3. Total cancelled rides by customers
4. Top 5 customers by number of rides
5. Driver cancellations due to personal/car issues
6. Max & Min driver ratings for Prime Sedan
7. All UPI payment rides
8. Average customer rating per vehicle type
9. Total booking value of successful rides
10. All incomplete rides with reasons

> Full SQL script: [`ola_analysis.sql`](ola_analysis.sql)

---

## 📁 Dataset

| Detail | Value |
|--------|-------|
| **File** | `Bookings-20000-Rows-July.csv` |
| **Rows** | 20,000 |
| **Period** | July 1–30, 2024 |
| **City** | Bengaluru |
| **Columns** | 19 (Date, Time, Booking_ID, Status, Vehicle_Type, Pickup/Drop Location, Ratings, etc.) |

---

## 🛠️ Tech Stack

- **Data Storage & Querying:** MySQL 8.0 (MySQL Workbench)
- **Visualization:** Microsoft Power BI Desktop
- **Dataset Preparation:** Microsoft Excel / ChatGPT (synthetic data)

---

## 📂 Project Structure

```
OLA-Data-Analysis/
│
├── Bookings-20000-Rows-July.csv     # Raw dataset
├── ola_analysis.sql                 # All SQL queries & views
├── OLA_Dashboard.pbix               # Power BI file (add yours here)
│
└── screenshots/
    ├── overall.png
    ├── vehicle_type.png
    ├── revenue.png
    ├── cancellation.png
    ├── ratings.png
    └── sql_workbench.png
```

---

## 🚀 How to Run

**SQL Part:**
1. Install MySQL & MySQL Workbench
2. Import `Bookings-20000-Rows-July.csv` into a table named `bookings`
3. Run `ola_analysis.sql` to create all views

**Power BI Part:**
1. Open `OLA_Dashboard.pbix` in Power BI Desktop
2. Update the data source path to your local CSV file
3. Refresh and explore the dashboard

---

## 👤 Author

**Mobasshir**
- 🎓 BCA Final Year — Amity University, Greater Noida
- 💼 Aspiring Data Analyst
- 🔗 [LinkedIn](#) | [GitHub](#)

---

> ⭐ If you found this project useful, please give it a star!
