# Online Retail Sales Analysis

## 1. Introduction

This project presents a comprehensive data analysis of an online retail dataset. The primary objective of this project is to extract meaningful insights into sales performance, customer behavior, and geographical distribution to inform business strategies. Specifically, it aims to answer key business questions such as revenue trends over time, top-performing countries and customers, and the geographical spread of sales units, providing actionable data for decision-makers.

## 2. Data Source and Preparation

The data for this project was obtained from [https://www.kaggle.com/datasets/lakshmi25npathi/online-retail-dataset]. The dataset contains 541910 rows and 8 columns including InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, and Country.

## 3. Data Cleaning and Transformation:
The raw data underwent several crucial cleaning and transformation steps to ensure accuracy, consistency, and suitability for analysis. This included:
* **Calculating Revenue:** A 'Revenue' field was added by multiplying 'Quantity' by 'Unit Price'
* **Removing negative values:** Negative values were addressed  in 'Quantity' and 'Unit Price' to provide accurate analysis to decision-makers 

## 4. Analysis and Methodology

The analysis was performed using Power BI Desktop. The methodology involved creating various interactive visualizations to explore sales data from different perspectives, focusing on seasonal trends, geographical distribution, and top customers and countries that are driving majority of the revenue. Filters were extensively used to refine data views, such as focusing on specific years, top categories, or excluding certain regions.

## 5. Answering Key Business Questions with Visualizations

This section presents the visualizations created to answer specific business questions, along with their key findings.

### Question 1: What is the trend of revenue over time?

* **Objective:** To visualize the revenue trend to understand seasonality or significant changes.
* **Visualization Type:** Line Chart
* **Chart Details:**
    * X-axis: Invoice Date
    * Y-axis: Revenue (Quantity * Unit Price) 
    * **Filter**: Data for the year 2011 only
   
* **Key Insights:**
    The revenue trend for 2011 shows a significant increase  from September until November where it reached its peak followed by a notable dip which could indicate holiday season sales. 
* **Visual:**
    ![Revenue by Month Line Chart](./images/Screenshot%20(251).png)
    *This line chart displays the monthly revenue trend for 2011, calculated by multiplying quantity by unit price.*

### Question 2: What are the revenue and quantity for each country?

* **Objective:** To compare sales performance (both revenue and quantity) across different countries
* **Visualization Type:**  Clustered Column Chart
* **Chart Details:**
    
    * X-axis: Country
    * Y-axis: Quantity and Revenue
    * **Filter 1:** Only the top 10 countries by revenue are displayed
    * **Filter 2:** The United Kingdom is excluded from the visual
* **Key Insights:**
     This chart effectively highlights the top 10 contributing countries (excluding the UK) in terms of both revenue and quantity. We can observe that countries like Netherlands and EIRE consistently lead in both metrics, indicating strong market presence and customer base in these regions.
* **Visual:**
    ![Quantity and Revenue by Country Clustered Column Chart](./images/Screenshot%20(252).png)
    *This clustered column chart compares the quantity of items sold and total revenue for the top 10 countries (excluding the UK).*

### Question 3: Which customers generate the most revenue?

* **Objective:** To identify the top 10 revenue-generating customers.
* **Visualization Type:** Column Chart.
* **Chart Details:**
    * **X-axis**: Represent Individual customer by ID.
    * **Y-axis**: Represent Total Revenue contributed by Individual customer.
    * **Filter:** Only the top 10 customers by revenue are displayed.
    * **Sorting:** Customers are sorted in descending order based on their total revenue.
* **Key Finding/Insight:**
     The analysis clearly identifies the top 10 revenue-contributing customers. Customer ID [14646] stands out significantly as the highest contributor, followed by [17453] and [14911]. This insight is critical for understanding customer loyalty and targeting high-value clients.
* **Visual:**
    ![Revenue by Customer ID Bar Chart](./images/Screenshot%20(253).png)
    *This bar chart displays the top 10 customers by the revenue they generated, excluding those without customer IDs and sorted in descending order.*

### Question 4: How are sales units distributed geographically?

* **Objective:** To visually represent the global distribution of sales units and identify key countries
* **Visualization Type:** Map Chart
* **Chart Details:**
    * The map highlights each country and shows either the total number of units sold or the name of the country.
    * **Filter:** The United Kingdom is filtered out.
* **Key Finding/Insight:**
    * The map visualization effectively shows that while sales are globally distributed, there are clear clusters of high unit sales in European countries (excluding the UK), with notable activity in countries like Netherlands, Germany, and France. This indicates a strong market presence in these regions.
* **Visual:**
    ![Quantity by Country Map Chart](./images/Screenshot%20(254).png)
    *This map chart visually represents the total units sold per country, excluding the United Kingdom, to highlight global sales distribution.*

## 6. Recommendations

Based on the insights derived from this analysis, here are some actionable recommendations:

* **Capitalize on Peak Seasons:** The sharp revenue increase in late 2011 suggests strong seasonal demand. Marketing and inventory efforts should be intensified leading up to and during these periods .
* **Focus on Top Countries:** Given the significant contribution of countries like Netherlands and Germany, targeted marketing campaigns or localized strategies could further boost sales in these regions.
* **Customer Loyalty Programs:** The identification of top-revenue customers provides an opportunity to implement loyalty programs or personalized marketing to retain and further engage these high-value clients.
* **Geographical Expansion:** While European countries show strong performance, the map also highlights other regions with potential. Further analysis could explore untapped markets or areas with lower current sales to identify growth opportunities.

