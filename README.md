# 🌦️ Live Weather Data Pipeline (Python + PostgreSQL)

This project is a simple **data engineering pipeline** that collects live weather data from an external API and stores it in a PostgreSQL database for further analysis and visualization.

It demonstrates how real-time data can be ingested, structured, and prepared for analytics dashboards.

---

## 📌 Project Overview

The system connects to the **Open-Meteo API** to retrieve current weather conditions based on geographic coordinates. The data is then processed in Python and stored in a PostgreSQL database with a timestamp, creating a time-series dataset.

This allows for comparisons between live weather conditions and historical trends.

---

## ⚙️ Technologies Used

- Python
- PostgreSQL
- psycopg2 (PostgreSQL connector)
- requests (API calls)
- Open-Meteo API
- Jupyter Notebook

---

## 🔄 Workflow

1. Connect to PostgreSQL database
2. Request live weather data from Open-Meteo API
3. Extract relevant fields (temperature, wind speed)
4. Insert data into a structured SQL table (`live_weather`)
5. Store timestamped records for time-series analysis

---

## 🗄️ Database Structure

Table: `live_weather`

| Column       | Type      | Description                  |
|--------------|----------|------------------------------|
| timestamp    | TIMESTAMP | Time of data collection     |
| temperature  | FLOAT     | Current temperature (°C)     |
| windspeed    | FLOAT     | Wind speed (km/h)           |

---

## 📊 Use Cases

- Real-time weather monitoring dashboard
- Comparison between live and historical weather data
- Foundation for ETL/data pipeline projects
- Power BI or Tableau visualization integration

---

## 🧠 Key Skills Demonstrated

- API integration with Python
- SQL database management
- ETL pipeline development (Extract, Transform, Load)
- Working with real-time data
- Data engineering fundamentals

---

## 🚀 Future Improvements

- Automate data collection using scheduled jobs (cron or Task Scheduler)
- Add error handling and logging system
- Expand dataset (humidity, precipitation, forecasts)
- Build Power BI dashboard for live visualization
- Optimize schema using star model (fact/dimension tables)

---

## 📷 Example Output

*(Optional: Add screenshots of your notebook or Power BI dashboard here)*

---

## 👤 Author

Developed as part of a data engineering learning project focused on building real-world ETL pipelines and analytics workflows.

---

## 📌 Note

This project uses free weather data from Open-Meteo and is intended for educational and portfolio purposes.
