# 🏅 Olympics Big Data Pipeline
**Modern Data Architectures for Big Data I — Group Project**

This project demonstrates a real-world big data architecture to extract, store, and analyze data related to Olympic athletes and events using Apache NiFi, HDFS, and Spark.


## 🎯 Project Objective

To build an end-to-end big data solution by applying modern data architecture tools to a real dataset, providing meaningful insights about Olympic performance, participation, and trends.


## 📁 Dataset

We used a publicly available dataset from Kaggle containing historical data of Olympic athletes, events, and results.

- **Source**: https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results
- **Format**: CSV
- **Size**: ~271K records, 15 columns
- **Key Fields**: Athlete name, sex, age, sport, medal, NOC, year, season, team, and event


## 🛠️ Technologies Used

| Component      | Tool/Service     |
|----------------|------------------|
| Ingestion      | **Apache NiFi**  |
| Storage        | **HDFS**         |
| Processing     | **Apache Spark** |
| Development    | **Jupyter Notebook (PySpark)** |


## 🔁 Big Data Pipeline

1. **Data Ingestion**
   - Ingested CSV data from local system using **Apache NiFi**
   - Cleaned and pushed files to HDFS for storage

2. **Data Storage**
   - HDFS directory structure:
     ```
     /olympics_project/
       └── raw/
           └── olympics_data.csv
     ```

3. **Data Processing with Spark**
   - Used **PySpark** to perform:
     - Data cleaning and schema enforcement
     - Null value handling and filtering
     - Transformations: filtering by country, year, medal status
     - Aggregations by sport, athlete, and year
   - Performed data analysis on participation and medal trends


## 📊 Key Insights

- 🥇 Top medal-winning countries and athletes
- 🧑‍🤝‍🧑 Gender representation trends over time
- 🏃 Most common sports by participation
- 🕰️ Historic performance evolution across Olympic years


## 📂 Project Structure


## 👥 Team Members

Group 4 — IE University  
- Ana Cortés
- Margarida Pereira
- Enrico Miguel Tajanlangit
- Kevin Tochkov
- Vibhushan Balaji Neethi Mohan


## 📌 Notes

> This project is part of the **Modern Data Architectures for Big Data I** course. All technologies applied were selected based on course guidelines. Dataset access is public and licensed for academic use.
