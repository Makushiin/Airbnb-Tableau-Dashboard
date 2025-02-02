# Airbnb Business Analysis Project

Welcome to my Airbnb Business Analysis Project repository! This project explores data analysis using Tableau to help someone interested in starting an Airbnb business determine the optimal location to purchase a home and convert it into an Airbnb rental. The analysis focuses on key factors such as the number of bedrooms, location (zipcode), and price, all with the goal of optimizing for profit.

---

## Project Overview

- **Data Integration:**  
  Joined the provided files correctly to create a comprehensive dataset.

- **Use Case:**  
  The primary objective is to assist a potential Airbnb entrepreneur in answering the question:  
  *"Where should I buy a home and convert it into an Airbnb rental?"*  
  The decision is based on optimizing for profit by analyzing factors such as:
  - Number of Bedrooms
  - Location (Zipcode)
  - Price

---

## Visualizations

### Visualization 1: Bar Chart – Average Price by Zipcode
- **Data Transformation:**  
  Changed the measure from `SUM(Price)` to `AVG(Price)` to better reflect the average pricing.
- **Chart Details:**  
  - A bar chart that displays the average price per zipcode.
  - Sorted from highest to lowest average price, providing insight into premium areas versus more affordable regions.

### Visualization 2: Map – Zipcode Analysis
- **Map Setup:**  
  Utilized zipcode data to create a geographic visualization.
- **Data Cleanup:**  
  Excluded null zipcode values to ensure accurate mapping.
- **Chart Details:**  
  - Each zipcode is labeled with its corresponding average price, offering a clear view of price distribution geographically.

### Visualization 3: Weekly Revenue Analysis
- **Chart Setup:**  
  - Configured columns to represent weeks and rows to represent price.
  - Adjusted the date field from a yearly to a weekly granularity.
- **Data Filtering:**  
  - Filtered out data for 1/1/17 due to it having only one data point.
- **Insights:**  
  - Observed that the first few months showed low revenue, indicating a potential ramp-up period.

### Visualization 4: Bedroom Analysis – Listings and Average Price
- **Data Transformation:**  
  - Converted the `Bedrooms` field from a numeric measure to a dimension.
  - Changed the measure from `SUM(Price)` to `AVG(Price)` to get average pricing per bedroom count.
  - Excluded null values for bedrooms.
- **Data Analysis:**  
  - Filtered out null values to maintain data integrity.
  - Counted the number of listings per bedroom category.
  - Modified the ID field to be an attribute, applied a `COUNT(DISTINCT)` to it, and labeled the marks accordingly for clear visualization.

### Dashboard Adjustments
- **Responsive Design:**  
  - Set the dashboard size to **Automatic** to ensure that it adjusts smoothly to different screen sizes and devices.

---

## Repository Contents

- **Tableau Workbook:**  
  The main Tableau workbook (e.g., `Tutorial.twb`) which contains all of the above visualizations and analysis.

- **Data Files:**  
  - `directory.csv`  
  - `vgsales.csv`  
  These files were used to compile and analyze the data in this project.

- **Dashboard Image:**  
  - `Dashboard 1.png` – A snapshot of the final dashboard.
