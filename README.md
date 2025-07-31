# 🌦️ Climate Data Dashboard using AWS S3, Snowflake & Power BI

This project demonstrates an end-to-end Business Intelligence solution where climate data is stored in AWS S3, processed in Snowflake, and visualized using Power BI. The dashboard provides interactive insights on Rainfall, Temperature, Humidity, Crop Impact, and Seasonal Patterns.

---

## 🚀 Tech Stack

- **AWS S3** – Cloud storage for raw climate data (.csv)
- **Snowflake** – Cloud data warehouse for data processing
- **Power BI** – Visualization & dashboard creation
- **SQL** – For data transformation and loading

---

## 🔁 Data Flow Architecture

```text
CSV (Raw Data)
     ↓
AWS S3 Bucket
     ↓
Snowflake (External Stage + Table)
     ↓
Power BI (Direct Connection to Snowflake)
     ↓
Interactive Dashboard with Filters, Cards, and Charts
```


## 📊 Key Insights from the Dashboard

📌 **Rainfall Trends**
- Displays region-wise and season-wise rainfall totals.
- Highlights areas with excessive or deficient rainfall.

📌 **Temperature Analysis**
- Shows average temperature by season and region.
- Detects extreme weather variations impacting agriculture.

📌 **Humidity Levels**
- Compares humidity levels across months and seasons.

📌 **Crop Category Insights**
- Visualizes how weather patterns affect crop growth.
- Helps in identifying crop suitability by region and weather.

📌 **Interactive Filters**
- Region, Crop, Month, and Year filters for customized exploration.

---

## 📁 Project Structure
````
climate-dashboard-aws-snowflake-powerbi/
├── dataset/
│ └── climate_data.csv
├── aws/
│ └── s3_upload_steps.md
│ └── s3_bucket_structure.png
├── snowflake/
│ └── create_table.sql
│ └── copy_into_snowflake.sql
│ └── snowflake_stage_setup.md
├── powerbi/
│ └── ClimateDashboard.pbix
├── screenshots/
│ └── rainfall_dashboard.png
│ └── temperature_dashboard.png
│ └── humidity_dashboard.png
├── README.md
````
---

## 🧾 Setup & Implementation Steps

### ✅ 1. Upload CSV to AWS S3
- Created S3 bucket `climate-data-abhay`
- Uploaded `climate_data.csv` to the bucket

### ✅ 2. Load into Snowflake
- Created external stage pointing to S3
- Used `COPY INTO` command to load into `climate_table`
- SQL scripts: `create_table.sql`, `copy_into_snowflake.sql`

### ✅ 3. Connect Power BI to Snowflake
- Configured Snowflake connector in Power BI
- Imported required tables
- Created charts, slicers, and cards in Power BI

---



## 🧠 Skills Applied

- SQL (DDL & DML in Snowflake)
- Data Modeling & Transformation
- Cloud Integration (AWS + Snowflake)
- Power BI DAX, Filters, and Visuals
- End-to-End Data Pipeline Understanding

---

## 📬 Contact

**Abhay Dahe**    
🌐 [GitHub](https://github.com/Abhaydahe)  
🔗 [LinkedIn](https://linkedin.com/in/abhaydahe)

---

## 📌 License

This project is for educational and portfolio purposes. Data is either public or anonymized.

