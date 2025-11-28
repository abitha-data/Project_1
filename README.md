# Project_1
## 📱💸📊 PhonePe Transaction Insights – End-to-End Data Analytics Project
  ###  Interactive Dashboard • SQL Analysis • Python EDA • Streamlit App

### ⭐ 📊 PhonePe Transaction Insights – Project Overview

   PhonePe Transaction Insights is an end-to-end data analysis project built using the open-source PhonePe Pulse dataset. It covers the complete workflow — extracting raw JSON files, transforming and loading them into SQL, analyzing the data with SQL & Python, and visualizing the results through an interactive Streamlit dashboard. The project provides clear state-wise and district-wise insights on transactions, user growth, app engagement, and insurance trends across different years and quarters. Overall, this project highlights digital payment patterns across India and demonstrates strong skills in ETL, SQL analytics, data visualization, and dashboard development.
   
### 📌 Domain: Finance / Digital Payments
### 📌 Dataset Source: PhonePe Pulse GitHub Repository

### ⭐ 🎯 Project Goal

The main goal of this project is to analyze India’s digital payment trends using the PhonePe Pulse dataset by converting raw JSON data into meaningful insights through ETL processing, SQL analysis, Python-based visualizations, and an interactive Streamlit dashboard. The project aims to clearly understand transaction patterns, user adoption, app engagement, and insurance usage across states and districts, helping identify top-performing regions and overall digital payment growth in India.

### ⭐ ✨ Features

🗺️ State-wise transaction analysis across India

👥 User growth & app engagement insights

🛡️ Insurance purchase trends visualization

🗾 Interactive India choropleth maps

🔥 Year-wise digital payment heatmaps

🏆 Top 10 performing states for quick comparison

🎛️ Easy filters for year, state, and data type

📊 Interactive Streamlit dashboard

🔄 Complete ETL pipeline (Extract → Transform → Load → Visualize)

📂 Uses real PhonePe Pulse open-source dataset

### 🗂️ Project Architecture Diagram
### 🧩 High-Level Flowchart
                +------------------------+
                |  Clone PhonePe Repo    |
                +-----------+------------+
                            |
                            v
                +------------------------+
                |   Extract JSON files   |
                +-----------+------------+
                            |
                            v
                +------------------------+
                |   Transform (ETL)      |
                | Clean + Normalize JSON |
                +-----------+------------+
                            |
                            v
                +------------------------+
                |     Load to SQL DB     |
                |  (Aggregated, Map, Top)|
                +-----------+------------+
                            |
                            v
                +------------------------+
                |  SQL Analysis & Views  |
                +-----------+------------+
                            |
                            v
                +------------------------+
                | Python EDA + Charts    |
                | Pandas / Seaborn / PX  |
                +-----------+------------+
                            |
                            v
                +------------------------+
                | Streamlit Dashboard UI |
                +------------------------+

### ⭐ 🛠️ Technologies Used 
### Python:
The core programming language used for developing the data extraction and processing scripts.

### PostgreSQL 🗄️:
Main SQL database used for storing tables and running analytical queries

### Pandas:
For data manipulation and transformation. To install this package:

          pip install Pandas

### PostgreSQL 🗄️ -Connector: 
PostgreSQL-Connector was used to establish a connection between Python and the PostgreSQL database.
It allows Python scripts to execute SQL queries, insert data, fetch results, and manage the ETL workflow smoothly, 
To install this package:

       pip install psycopg2

### Streamlit:
Streamlit is an open-source Python library designed to create and share custom web applications for data science and machine learning projects with minimal effort. Its simplicity and focus on rapid prototyping make it a popular choice among data scientists and developers who need to quickly visualize and interact with data. Also you can download the data as csv file from the web application. To install this package:

           pip install streamlit


Plotly & Altair – for charts and visualizations

### Git & GitHub:
Git & GitHub are used for version control and project management.
Git helps track changes in the code, while GitHub is used to store the project online, collaborate, and fetch the PhonePe Pulse dataset directly from the official repository.

### JSON: 
JSON is a simple text-based format used to store and exchange data.
It holds data in key–value pairs, making it easy to read, write, and convert into tables for analysis.

### ⭐ Prerequisites:
Python 3.x installed on your system.

PostgreSQL installed and running 🗄️

pip package manager

Git installed for cloning the PhonePe Pulse repository

Stable internet connection for fetching data 🌐

### ⭐ 🔄 Workflow:
### 1️⃣ Data Extraction

A custom Python script is used to clone the PhonePe Pulse GitHub repository and automatically collect all the raw JSON files.
This ensures the project always works with the latest dataset published by PhonePe.

### 2️⃣ Data Transformation

Using Python and Pandas, the raw JSON files (which contain nested and scattered information) are:

cleaned,

normalized,

flattened, and

converted into structured DataFrames.
This step prepares the data to be stored in a database in a clean, analyzable format.

### 3️⃣ Database Insertion (PostgreSQL)

The transformed data is loaded into a PostgreSQL database.
Tables are created for different categories such as transactions, users, and insurance.
In this stage, INSERT queries are executed to store the data efficiently for future querying and analysis.

### 4️⃣ Dashboard Creation

An interactive dashboard is built using Streamlit and Plotly.
This dashboard displays:

choropleth maps,

heatmaps,

top-state comparisons,

totals and summaries,
allowing users to visually explore India’s digital payment trends.

### 5️⃣ Data Retrieval (Dynamic Updates)

Whenever a user selects a year, state, or category,
the dashboard sends a query to the PostgreSQL database,
fetches the latest data,
and updates the visualizations instantly.
This makes the dashboard dynamic, responsive, and user-friendly.

### 🗄️ Folder Structure:
📁 phonepe-Transaction/

│── 📁 data/                  

│── 📁 sql/                 

│── 📁 src/                  

│── app.py                    

│── Transform.py              

│── requirements.txt

│── README.md

