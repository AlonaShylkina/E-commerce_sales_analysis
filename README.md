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

> **Note:** Sample data is provided for illustration purposes. Sensitive or proprietary information has been removed.
---

### Database Model
The database model used in this project is provided as a PNG file. Refer to `database_model.png` for an overview of the data structure.

---

### Python Libraries Used
The following Python libraries were used to process and analyze the data in Google Colab:
- **Google Cloud BigQuery SDK**: `google.cloud.bigquery`
- **Authentication**: `google.oauth2.service_account`
- **Data Manipulation**: `pandas`, `numpy`
- **Visualization**: `matplotlib`, `seaborn`
- **Statistical Analysis**: `scipy.stats`
- **Google Drive Integration**: `google.colab.drive`

---

### Project Workflow
1. **Extract Data from Google BigQuery**: SQL queries were written and executed directly in Google Colab to extract the required sales data from Google BigQuery.
2. **Data Processing & Analysis**: Data was processed and analyzed using Python libraries such as Pandas, NumPy, and SciPy.
3. **Data Visualization**: The analyzed data was visualized using Matplotlib and Seaborn.
4. **Interactive Dashboard**: The results were exported to Tableau for creating a comprehensive dashboard that displays key insights from the analysis.

---

### Results and Insights
General information:
- the analysis period is from 2020-11-01 to 2021-01-31
- the number of unique sessions is 349,545
- the total number of orders is 33,538
- the total number of customers with a registered account is 27,945
- the biggest number of customers with registered accounts is in United States - 12,384. This is the vast majority, as India and Canada took 2nd and 3rd place with 2,687 and 2,067 registered accounts, respectively.
- most of the user's sessions were conducted on desktops - 58,48%
- most of the user's sessions were conducted on Chrome browser - 68,22%  
- the company works with 107 countries on 5 continents
- the highest sales is in United States - $ 13,943,553.9. This is the vast majority, as India and Canada took 2nd and 3rd place with sales of $ 2,809,762.0 and             $ 2,437,921.0 respectively. The situation is the same for the number of orders: Uniter States - 14,673; India - 3,029; Canada - 2,560.
- the company sells 14 product categories
- the company sold the most in "Bookcases & shelving units" product category - 7630 units
- the most profitable product category is "Sofas & armchairs" with sales of $ 8,388,254.5
- the company generates the highest sales ($11,433,151.60) and the highest number of orders (11,921) from organic search.
- the company generates the highest sales ($18,864,039.00) and the highest number of orders (19,702) from desktop orders.

---

- a correlation of 0.79 indicates a strong positive relationship between Total Sessions and Total Sales, meaning that more sessions lead to more sales.
- the correlations between Americas and Asia, Americas and Europe, Asia and Europe are statistically significant. It suggests that there is a meaningful relationship between sales on the continents (which could be due to global trends, market interdependencies, economic, or even political events). They are not entirely independent, and business strategies should account for the interconnectedness of global markets.
- correlation range of 0.51 to 0.66 between sales of top 5 product categories (Beds, Bookcases & shelving units, Cabinets & cupboards, Chairs, Sofas & armchairs) indicates a moderate to strong positive correlation between sales across product categories. This means that when sales increase in one category, sales in the other category tend to increase as well. Since the p-value is less than 0.05, the correlation is statistically significant, meaning that the relationship observed is not due to randomness, and there is a real underlying connection between the sales of these product categories.

---

Customers subscribed to the company's marketing emails generally place more orders and spend more than those who are unsubscribed. This could indicate that email marketing makes a significant impact—when customers are aware of campaigns, discounts, etc., they are more likely to make purchases.

Sales dynamics, both overall and by continent/device, show spikes in the second half of December, likely due to pre-holiday purchases, and in early January, which may be related to the holiday weekend and discounts. The increase in sales on certain dates at the end of November is likely related to Black Friday and Cyber Monday discounts, along with Thanksgiving preparations in the US and Canada.
The spike on November 1st may mark the transition from Halloween sales to early promotions for the holiday shopping season. There may have been discounts on leftover Halloween items.




