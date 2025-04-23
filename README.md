# fulfillment-center-sql-practice

This project explores operational analytics using SQL, based on a simulated dataset of scanned items in a fulfillment center.

### Dataset Columns
- **Region**  
- **Site**  
- **Machine**  
- **Date**  
- **EventTimestamp**  
- **LoginID**  
- **CaseID**  
- **ItemID**

---

### Business Questions Explored

1. **Average time between item-to-item scans**  
   Measures how frequently items are scanned by a user each day.

2. **Average time between case transitions**  
   Captures the average time between finishing one case and starting the next.

3. **Average case completion time**  
   Tracks how long it takes to complete a case (from first to last item scan) per user per day.

---

### SQL Techniques Used
- **Common Table Expressions (CTEs)** to break complex steps into readable chunks  
- **Window functions** (`LAG`, `LEAD`, `ROW_NUMBER`, `MIN`, `MAX`, etc.) to calculate time differences and track transitions  
- **Aggregate functions** to compute daily and per-login metrics

---

### How to Use
These queries are written in standard SQL and should work in most SQL engines (PostgreSQL, Snowflake, BigQuery, etc.) with minor adjustments.

Each SQL file corresponds to one of the questions above and is named accordingly.

---

### License
MIT — feel free to use, modify, and build upon this work.
