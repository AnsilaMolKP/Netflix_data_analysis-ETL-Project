🎬 Netflix Data Analysis Project

📌 Project Overview
This project demonstrates an end-to-end data analytics workflow using the Netflix Movies and TV Shows dataset from Kaggle.  
The goal was to extract raw data, clean and transform it using SQL, and answer meaningful business questions — simulating a real-world Data Analyst workflow.

---

📂 Dataset
- Source: Kaggle – Netflix Movies and TV Shows
- Format: CSV
- Records: 8,000+
- Description: Contains information about Netflix titles such as type, title, director, cast, country, date added, release year, rating, duration, and genre.

---

🛠 Tools & Technologies
- Python (Pandas)
- SQL Server (SSMS)
- SQLAlchemy & ODBC
- Jupyter Notebook
- Kaggle API

---

 🔄 ETL Workflow

 🔹 Extract
The dataset was extracted from Kaggle and loaded into Python using Pandas for initial inspection and validation.

Basic checks were performed to:
- Inspect data structure
- Identify missing values
- Validate text lengths
- Verify multilingual data

---

 🔹 Load (Raw Layer)
A raw staging table (`netflix_raw`) was created in SQL Server to store the original dataset without modifications.

The data was loaded from Python into SQL Server using SQLAlchemy, ensuring separation between raw and transformed data.

---

 🔹 Transform
All data transformations were performed in SQL Server to simulate a production analytics environment.

Key transformations included:
- Removing duplicate records using `ROW_NUMBER()` and CTEs
- Converting text-based date fields into proper DATE format
- Standardizing duration values for movies and TV shows
- Handling missing values in country and duration columns
- Populating missing country values using director-based relationships
- Normalizing data into separate tables for genres, directors, and countries using `STRING_SPLIT`

---

 🔹 Analyze
The cleaned dataset was used to answer analytical business questions such as:
- Directors who have created both Movies and TV Shows
- Country with the highest number of Comedy movies
- Directors with the most movies released each year
- Average duration of movies by genre
- Directors who have created both Comedy and Horror movies

Advanced SQL concepts used:
- CTEs
- Window functions
- Conditional aggregation
- String manipulation
- Date functions

---

 📊 Key Skills Demonstrated
- End-to-end ETL design
- Data cleaning and validation
- SQL-based data transformation
- Data normalization
- Analytical SQL querying
- Real-world problem solving

---

🚀 Future Enhancements
- Build dashboards using Power BI or Tableau
- Add advanced analytical queries
- Automate the ETL process

---

 👩‍💻 About
This project is part of my learning journey as an aspiring Data Analyst, focused on building strong foundations in Python, SQL, and data analytics workflows.
