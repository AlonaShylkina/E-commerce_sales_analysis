# E-commerce Sales Analysis Project

This repository contains the code and resources for a project conducted using Google Colab to analyze E-commerce sales data. The project involved direct connection from Google Colab to Google BigQuery, with SQL queries written to extract data, and Tableau used for visualizing the results in a dashboard. The final visualizations are hosted on Tableau Public.

## Table of Contents
- [Project Overview](#project-overview)
- [Key Tools and Technologies](#key-tools-and-technologies)
    - [Tableau Dashboard](#tableau-dashboard)
- [Dataset](#dataset)
- [Database Model](#database-model)
- [Python Libraries Used](#python-libraries-used)
- [Project Workflow](#project-workflow)
- [Results and Insights](#results-and-insights)

---

### Project Overview

The goal of this project is to analyze and understand patterns in E-commerce sales using a dataset extracted from a database. The project utilized a variety of tools and libraries, including Google BigQuery, Python (Google Colab), and Tableau, to derive insights from the data.

---

### Key Tools and Technologies
- **Google Colab**: A cloud-based Python environment used for running the analysis code and connecting to Google BigQuery.
- **Google BigQuery**: A data warehouse used to store and manage large datasets.
- **SQL**: Queries written in SQL were used to extract the required data from Google BigQuery.
- **Tableau**: Used for creating and sharing the interactive dashboard visualizing the analysis results.

---

#### Tableau Dashboard
The interactive dashboard created from the analysis is available on Tableau Public:  
[View Dashboard on Tableau Public](https://public.tableau.com/views/SalesSessionsAnalysis/SalesSessionsAnalysis?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

### Dataset
The dataset used in this project was extracted from a database and contains the following fields:
- **date**: Date of the sales session
- **ga_session_id**: Unique identifier for the session
- **continent**: Continent where the session occurred
- **country**: Country where the session occurred
- **device**: Device type used by the customer
- **browser**: Browser used during the session
- **mobile_model_name**: Mobile model name (if applicable)
- **operating_system**: Operating system of the device
- **traffic_source**: Source of website traffic
- **sales_channel**: Channel through which the sale was made
- **account_id**: Account identifier
- **mail_is_verified**: Whether the customer's email is verified
- **is_unsubscribed**: Whether the customer is unsubscribed
- **product_category**: Category of the product
- **product_name**: Name of the product sold
- **product_price**: Price of the product

---

### Database Model
The database model used in this project is provided as a PNG file. Refer to `database_model.png` for an overview of the data structure.

---

### Python Libraries Used
The following Python libraries were used to process and analyze the data in Google Colab:
- **Google Cloud BigQuery SDK**: `from google.cloud import bigquery`
- **Authentication**: `from google.oauth2 import service_account`
- **Data Manipulation**: `import pandas as pd`, `import numpy as np`
- **Visualization**: `import matplotlib.pyplot as plt`, `import seaborn as sns`, `import matplotlib.ticker as mticker`
- **Statistical Analysis**: `from scipy.stats import pearsonr`
- **Google Drive Integration**: `from google.colab import drive`

---

### Project Workflow
1. **Extract Data from Google BigQuery**: SQL queries were written and executed directly in Google Colab to extract the required sales data from Google BigQuery.
2. **Data Processing & Analysis**: Data was cleaned, processed, and analyzed using Python libraries such as Pandas, NumPy, and SciPy.
3. **Data Visualization**: The analyzed data was visualized using Matplotlib and Seaborn.
4. **Interactive Dashboard**: The results were exported to Tableau for creating a comprehensive dashboard that displays key insights from the analysis.

---

### Results and Insights
The results from the analysis include insights into sales trends, customer behavior, and product performance. The dashboard on Tableau Public provides detailed visualizations that allow for further exploration of the data.
