# 🚖 Ola Ride Booking Analysis | Excel + SQL + Power BI

An end-to-end data analysis of **20,408 Ola ride bookings from July 2024**. I cleaned the raw data in Excel, solved 10 business problems in MySQL, and built a 5-page Power BI dashboard to understand bookings, cancellations, revenue and ratings.

## 📌 Table of Contents
- [Project Workflow](#-project-workflow)
- [Dataset](#-dataset)
- [Data Cleaning](#-data-cleaning-excel)
- [SQL Analysis](#-sql-analysis-mysql)
- [Power BI Dashboard](#-power-bi-dashboard)
- [Key Insights](#-key-insights)
- [Repository Structure](#-repository-structure)
- [Author](#-author)

## 🔄 Project Workflow
Raw data → **Excel** (cleaning) → **MySQL** (10 business problems) → **Power BI** (dashboard)

## 📂 Dataset
One month of Ola booking data (1st to 30th July 2024) with 19 columns:

## 🧹 Data Cleaning (Excel)
- Removed empty rows and errors
- Removed duplicate records so each booking is counted once.
- Trimmed extra spaces in text fields so categories (e.g. "UPI" vs "UPI ") group correctly.

## 🗄️ SQL Analysis (MySQL)
I solved 10 business problems using SQL queries saved as views:

| # | Business Problem | SQL Concepts Used |
|---|------------------|-------------------|
| 1 | Retrieve all successful bookings | `WHERE` |
| 2 | Average ride distance for each vehicle type | `AVG`, `GROUP BY` |
| 3 | Total rides cancelled by customers | `COUNT`, `WHERE` |
| 4 | Top 5 customers with the highest number of rides | `COUNT`, `GROUP BY`, `ORDER BY`, `LIMIT` |
| 5 | Rides cancelled by drivers due to personal and car-related issues | `COUNT`, `WHERE` |
| 6 | Max and min driver ratings for Prime Sedan bookings | `MAX`, `MIN`, `WHERE` |
| 7 | All rides paid using UPI | `WHERE` |
| 8 | Average customer rating per vehicle type | `AVG`, `GROUP BY` |
| 9 | Total booking value of successfully completed rides | `SUM`, `WHERE` |
| 10 | All incomplete rides along with the reason | `WHERE` |

📁 Query screenshots and output are in the `screenshots/` folder.

## 📊 Power BI Dashboard
A 5-page dashboard with a date slicer for filtering.

| Page | Problems Solved | Visuals |
|------|-----------------|---------|
| **Overall** | Ride volume over time, booking status breakdown (successful vs cancelled %) | KPI cards, line chart, pie chart |
| **Vehicle Type** | Total and successful booking value, average and total distance by vehicle type | Table |
| **Revenue** | Revenue by payment method, top 5 customers by booking value, ride distance per day | Bar charts, table |
| **Cancellation** | Cancelled ride reasons by customers and by drivers | KPI cards, pie charts |
| **Ratings** | Average driver and customer ratings by vehicle type | Rating cards |

## 💡 Key Insights
- **Bookings:** 62% were successful, 28% were cancelled (17.9% by drivers, 10.2% by customers), and 9.9% ended with no driver found
- **Customer cancellations:** the top reason is the driver not moving towards the pickup (29%)
- **Driver cancellations:** the top reason is personal and car-related issues (34%)
- **Payments:** Cash and UPI generate roughly 95% of revenue
- **Vehicles:** Prime Sedan has the highest total booking value (₹1.67M); Bike and E-Bike cover the most distance (48K and 47K km)
- **Distance:** Autos average about 10 km per ride vs about 25 km for other vehicles
- **Ratings:** driver and customer ratings are almost flat across vehicle types (about 2.4 to 2.5)

## 📁 Repository Structure
```
ola-ride-booking-analysis/
├── README.md
├── data/            # raw and cleaned datasets
├── sql/             # queries and views
├── powerbi/         # Power BI (.pbix) file
└── screenshots/     # SQL and dashboard screenshots
```

## 🛠️ Tools Used
Excel · MySQL · Power BI · DAX


## 👤 Author
**Syed Abdul Samad Ali Jaffery**
🔗 [LinkedIn](https://www.linkedin.com/in/syed-abdul-samad-ali-jaffery-4579b5395/) 
📧 inquiriesforsamad@gmail.com
