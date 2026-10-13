
# Ola Ride Booking Analysis | Excel + SQL + Power BI

Analysis of 20,408 Ola bookings from July 2024. I cleaned the data in Excel, solved 10 business problems in MySQL, and built a 5-page Power BI dashboard covering overall performance, vehicle type, revenue, cancellations and ratings.

## Workflow
Raw data → **Excel** (cleaning) → **MySQL** (10 queries) → **Power BI** (dashboard)

## Data Cleaning (Excel)
- Removed empty rows and errors
- Removed duplicate records
- Trimmed extra spaces in text fields

## SQL Analysis
Solved 10 business problems using MySQL views, including successful bookings, average distance and rating by vehicle type, top 5 customers, driver and customer cancellations, UPI payments, successful booking value and incomplete rides with reasons.

## Power BI Dashboard
Pages: **Overall · Vehicle Type · Revenue · Cancellation · Ratings**

## Key Insights
- 62% of bookings were successful, 28% were cancelled (17.9% by drivers, 10.2% by customers), and 9.9% found no driver
- Top customer cancellation reason: driver not moving towards pickup (29%)
- Top driver cancellation reason: personal and car-related issues (34%)
- Cash and UPI generate roughly 95% of revenue
- Prime Sedan has the highest booking value (₹1.67M)
- Autos average ~10 km per ride vs ~25 km for other vehicles
- Customer and driver ratings are flat across vehicle types (~2.4 to 2.5)

## Repository
- `sql/`: queries and views
- `powerbi/`: .pbix file
- `screenshots/`: SQL and dashboard screenshots

## Author
Syed Abdul Samad Ali Jaffery | https://www.linkedin.com/in/syed-abdul-samad-ali-jaffery-4579b5395/ | inquiriesforsamad@gmail.com
