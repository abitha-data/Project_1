# Project_1
## 📱💸📊 PhonePe Transaction Insights – End-to-End Data Analytics Project
  ###  Interactive Dashboard • SQL Analysis • Python EDA • Streamlit App

### 📊 PhonePe Transaction Insights – Project Overview

   PhonePe Transaction Insights is an end-to-end data analysis project built using the open-source PhonePe Pulse dataset. It covers the complete workflow — extracting raw JSON files, transforming and loading them into SQL, analyzing the data with SQL & Python, and visualizing the results through an interactive Streamlit dashboard. The project provides clear state-wise and district-wise insights on transactions, user growth, app engagement, and insurance trends across different years and quarters. Overall, this project highlights digital payment patterns across India and demonstrates strong skills in ETL, SQL analytics, data visualization, and dashboard development.
   
### 📌 Domain: Finance / Digital Payments
### 📌 Dataset Source: PhonePe Pulse GitHub Repository

### 🎯 Project Goal

The main goal of this project is to analyze India’s digital payment trends using the PhonePe Pulse dataset by converting raw JSON data into meaningful insights through ETL processing, SQL analysis, Python-based visualizations, and an interactive Streamlit dashboard. The project aims to clearly understand transaction patterns, user adoption, app engagement, and insurance usage across states and districts, helping identify top-performing regions and overall digital payment growth in India.

### ✨ Features

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

### 🛠️ Technologies Used 
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

### Installation:
▶️ How to Run This Project
1. Clone the repository
git clone <your-repo-url>

2. Install dependencies
pip install -r requirements.txt

3. Run Streamlit Dashboard
streamlit run app.py



### Prerequisites:
Python 3.x installed on your system.

PostgreSQL installed and running 🗄️

pip package manager

Git installed for cloning the PhonePe Pulse repository

Stable internet connection for fetching data 🌐

### 🔄 Project Workflow:
### 1️⃣ Data Extraction:

The PhonePe Pulse GitHub repository is cloned automatically using a Python script.

All JSON files containing state-wise, district-wise, and category-wise data are collected.

Files are organized by year and quarter, ready for transformation.

### 2️⃣ Data Transformation:

Using Python + Pandas, the raw JSON data is cleaned and normalized.

Nested JSON structures are flattened into tabular format.

Columns such as state, year, quarter, transaction_count, transaction_amount, users, app_opens, etc. are properly structured.

Missing or inconsistent values are handled to ensure accuracy.

### 3️⃣  Database Insertion (PostgreSQL):

The transformed data is inserted into PostgreSQL tables using a connector like psycopg2.

Separate tables are created for transactions, users, insurance, and top metrics.

SQL schema ensures fast filtering, grouping, and aggregation during analysis.

### 4️⃣  Dashboard Creation (Streamlit + Plotly):

An interactive Streamlit dashboard is built to visualize insights.

Plotly is used to create India maps, bar charts, line charts, heatmaps, and comparison graphs.

Users can filter data by year, state, category, and type of metric.

Dashboard updates dynamically based on the selected filters.

### 5️⃣ Data Retrieval & Live Updates:

When the dashboard loads, data is fetched from PostgreSQL.

SQL queries supply updated values for maps, tables, and charts.

Users always see the latest insights since the data is pulled directly from the database.

### 🗄️ Folder Structure:
📁 phonepe-Transaction/

│── 📁 data/                  

│── 📁 sql/                 

│── 📁 src/                  

│── app.py                    

│── Transform.py              

│── requirements.txt

│── README.md

