# Brazilian E-Commerce Data Analysis | Olist Analytics

## Project Overview

This project analyzes the Brazilian E-Commerce Public Dataset by Olist to explore sales performance, customer behavior, product performance, and order delivery operations.

Covering the period from 2016 to 2018, the dataset provides insights into e-commerce transactions and related business operations. Python is used for data preparation, exploratory data analysis, and business metrics, while Power BI is used to develop an interactive dashboard for business reporting.

The project follows a structured analytics workflow, from data loading and cleaning to business analysis, visualization, and business recommendations.

## Business Objectives

The main objectives of this project are to:

- Measure sales performance and order volume.
- Analyze customer purchasing behavior and repeat-purchase patterns.
- Identify high-performing and low-performing product categories.
- Compare sales performance across Brazilian states and cities.
- Evaluate order approval times and delivery performance.
- Analyze late deliveries and order fulfillment timelines.
- Explore payment methods and their contribution to order value.
- Build an interactive Power BI dashboard to communicate business metrics.
- Translate analytical results into actionable business recommendations.

## Dataset

**Source:** Brazilian E-Commerce Public Dataset by Olist

**Dataset link:** [Access the dataset on Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

The dataset contains multiple related tables describing customers, orders, products, payments, sellers, reviews, and geographic information.

### Dataset Tables

| Table | Description |
|---|---|
| Customers | Customer identifiers and geographic information |
| Orders | Order status and lifecycle timestamps |
| Order Items | Products purchased, item prices, and freight values |
| Products | Product attributes, categories, and dimensions |
| Payments | Payment methods, installments, and payment values |
| Reviews | Customer review scores and comments |
| Sellers | Seller identifiers and locations |
| Product Category Translation | Portuguese-to-English product category translations |
| Geolocation | Geographic coordinates associated with Brazilian postal codes |

The analysis focuses on the tables required to answer the project's business questions.

**Dataset period:** 2016–2018.

**Important:** This is a historical dataset. The findings describe the available data and should not be interpreted as a representation of the current e-commerce market.

The dataset is not included in this GitHub repository. See [How to Run the Project](#how-to-run-the-project) for setup instructions.

## Tools and Technologies

### Data Analysis

- **Python** — Data processing and exploratory analysis
- **Pandas** — Data cleaning, transformation, grouping, and aggregation
- **NumPy** — Numerical operations
- **Matplotlib** — Data visualization
- **Plotly** — Interactive visualizations

### Business Intelligence

- **Power BI** — Interactive dashboards and business reporting
- **DAX** — Measures and calculated metrics
- **Power Query** — Data transformation where applicable

### Development and Project Management

- **Jupyter Notebook** — Organizing the analytical workflow
- **Git and GitHub** — Version control and project documentation

## Repository Structure

```text
01-Ecommerce-Analytics/
│
├── dashboard/
│   └── Olist_Ecommerce_Analytics_Dashboard.pbix
├── notebooks/
│   ├── 01_Data_Loading_and_Exploration.ipynb
│   ├── 02_Data_Cleaning_and_Preparation.ipynb
│   ├── 03_Business_Analysis.ipynb
│   └── 04_Visualization_and_Insights.ipynb
│
├── screenshots/
│   ├── 01_Executive_Overview.png
│   ├── 02_Sales_Performance.png
│   ├── 03_Product_Analysis.png
│   ├── 04_Customer_Geographic_Analysis.png
│   └── 05_Orders_Delivery_Analysis.png
│
├── .gitignore
├── README.md
└── requirements.txt
```

**Note:** The original dataset files in the `data/` directory are excluded from this repository and must be downloaded separately.

## Analytical Workflow

### 1. Data Loading and Exploration

The first stage focuses on understanding the dataset structure and assessing data quality.

Activities include:

- Loading CSV files into Pandas DataFrames.
- Inspecting dataset dimensions, column names, and data types.
- Reviewing summary statistics and unique values.
- Identifying missing values and potential data-quality issues.
- Exploring relationships between customers, orders, order items, and products.

**Notebook:** `01_Data_Loading_and_Exploration.ipynb`

### 2. Data Cleaning and Preparation

This stage prepares the datasets for reliable analysis.

Activities include:

- Handling missing values where appropriate.
- Converting timestamp columns to datetime data types.
- Reviewing duplicates and data consistency.
- Preparing cleaned datasets for analysis and reporting.
- Creating derived fields required for business metrics.
- Exporting processed datasets for reuse.

Cleaning decisions depend on the meaning of each column and its relevance to the analysis.

**Notebook:** `02_Data_Cleaning_and_Preparation.ipynb`

### 3. Business Analysis

Python is used to investigate business questions through filtering, grouping, aggregation, and metric calculation.

The analysis covers:

- Sales and order performance.
- Customer purchasing frequency.
- Product and category performance.
- Geographic sales distribution.
- Order approval and delivery durations.
- Delivery performance and late orders.
- Payment method patterns.

**Notebook:** `03_Business_Analysis.ipynb`

### 4. Visualization and Insights

Charts are used to communicate patterns, comparisons, and trends identified during the analysis.

Visualizations support the interpretation of business metrics and help identify areas that may require further investigation.

**Notebook:** `04_Visualization_and_Insights.ipynb`

### 5. Power BI Dashboard

Power BI brings key metrics and analytical findings together in an interactive reporting experience.

The dashboard is designed to explore business performance across time, geography, products, customers, and order delivery.

## Power BI Dashboard

The dashboard is organized into five analytical pages.

### 1. Executive Overview

Provides a high-level summary of business performance through key performance indicators and core metrics.

![Executive Overview](screenshots/01_Executive_Overview.png)

### 2. Sales Performance

Explores sales trends and performance across the available time period and relevant business dimensions.

![Sales Performance](screenshots/02_Sales_Performance.png)

### 3. Product Analysis

Examines product and category performance to identify leading contributors and areas for further investigation.

![Product Analysis](screenshots/03_Product_Analysis.png)

### 4. Customer and Geographic Analysis

Explores customer distribution and geographic performance across Brazilian states and cities.

![Customer and Geographic Analysis](screenshots/04_Customer_Geographic_Analysis.png)

### 5. Orders and Delivery Analysis

Examines order statuses, delivery timelines, and delivery performance, including late-delivery patterns.

![Orders and Delivery Analysis](screenshots/05_Orders_Delivery_Analysis.png)

**Dashboard file:** [Olist_Ecommerce_Analytics_Dashboard.pbix](dashboard/Olist_Ecommerce_Analytics_Dashboard.pbix)

## Key Findings

The project investigates the following business areas:

### Customer Behavior

96.88% of customers (93,099 out of 96,096 total unique customers) are one-time buyers, while only 3.12% (2,997 customers) are repeat customers.

The most active customer placed 17 orders.

### Sales Performance

A total of 99,441 orders generated 13,591,643.70 BRL in net sales (excluding freight).

Average order value (AOV) per transaction is 137.75 BRL, with a peak single order value reaching 13,440.00 BRL.

Order volumes grew significantly over time: 329 orders in 2016, 45,101 in 2017, and 54,011 in 2018.

August was the peak sales month with 10,843 orders, followed by May (10,573) and July (10,318), whereas September was the lowest month with 4,305 orders.

### Product Performance

Most Sold Category by Units: cama_mesa_banho (Bed, Bath & Table) with 11,115 units sold.

Top Revenue-Generating Category: beleza_saude (Health & Beauty) generating 1,258,681.34 BRL, followed closely by relogios_presentes (1,205,005.68 BRL).

Top Best-Selling Product (Units): Product ID aca2eb7d00ea1a7b8ebd4e68314663af (527 units).

Top Revenue Product: Product ID bb50f2e236e5eea0100680137654686c generating 63,885.00 BRL.

### Geographic Performance

High revenue concentration in the Southeast region: São Paulo (SP) dominates the market with 47,820 orders, contributing 38.28% of total revenue (5,202,955.05 BRL).

Together, SP (38.28%), Rio de Janeiro (RJ - 13.42%), and Minas Gerais (MG - 11.66%) account for 63.36% of total platform sales.

State with the lowest sales: Roraima (RR) at 0.06% (7,829.43 BRL).

Paraíba (PB) recorded the highest Average Order Value (217.77 BRL), whereas São Paulo (SP) recorded the lowest (125.12 BRL).

### Payment Behavior

Total Payment Volume: 16,008,872.12 BRL across all methods with an average payment of 154.10 BRL.

Credit Card is the preferred choice, accounting for 73.92% of orders (76,795 payments) and generating 12,542,084.19 BRL (Average value: 163.32 BRL).

Boleto comes second at 19.04% (19,784 payments), followed by Vouchers (5.56%) and Debit Cards (1.47%).

50.58% of payments were made in a single installment, while the overall average installment count was 2.85.

### Delivery Operations

- Average order approval time: 10.28 hours.
- Average shipping preparation time (purchase-to-carrier dispatch): 2.81 days.
- Average carrier-to-customer delivery time: 9.33 days.
- Average total order delivery time: 12.56 days.
- Late deliveries: 7,827 orders (7.87%) missed the estimated delivery date.

- **Geographic Delivery Performance:** Average carrier-to-customer delivery time varied significantly across Brazilian states, ranging from 5.52 days in São Paulo (SP) to 24.57 days in Roraima (RR). These differences highlight opportunities to investigate regional logistics performance.

### Customer Reviews & Satisfaction

Average review score: 4.09 / 5.00.

77.07% positive ratings (4-5 stars), 8.24% neutral (3 stars), and 14.69% negative ratings (1-2 stars).

Only 41.30% of reviews included written comments. Customers leaving negative reviews were significantly more likely to leave comments (76.55% of 1-star reviews had comments vs. 35.85% of 5-star reviews).

## Business Recommendations

Based on the validated analytical results above, the following strategic business recommendations are proposed:

### Customer Retention & Loyalty

Insight: The purchase frequency rate is low, which necessitates an examination of opportunities for customer retention.

Action: Implement post-purchase loyalty programs, automated re-engagement email campaigns, and personalized product recommendations to boost repeat purchase rates beyond 3.12%.

### Product & Inventory Strategy

Insight: High-volume categories (cama_mesa_banho) differ from high-revenue categories (beleza_saude and relogios_presentes).

Action: Optimize inventory stock according to demand profile.

### Geographic Expansion & Logistics Focus

Insight: Average carrier-to-customer delivery time varied significantly across Brazilian states, ranging from 5.52 days in São Paulo (SP) to 24.57 days in Roraima (RR). These differences highlight opportunities to investigate regional logistics performance and identify potential areas for improvement.

**Action:** Investigate the factors contributing to longer carrier-to-customer delivery times in states such as Roraima (RR), Amapá (AP), and Amazonas (AM). Evaluate regional logistics performance and identify opportunities to reduce delivery times while maintaining service quality.

### Delivery Operations & Delay Reduction

**Insight:** 7.87% of all orders experienced delivery delays. The relationship between delivery delays and negative customer reviews requires further investigation.

**Action:** Investigate the relationship between delivery delays and review scores, improve estimated delivery-date accuracy during peak months, and evaluate regional logistics improvements to reduce delivery times and improve customer satisfaction.

### Payment Method Optimization

Insight: 73.92% of sales rely on credit cards, with single-payment transactions representing 50.58%.

Action: Introduce zero-interest installment promotions for high-ticket items and streamline the checkout experience for Boleto and Debit Card users to minimize drop-off rates.

### Performance Monitoring

Continuously track main KPIs (AOV, Late Delivery %, Repeat Purchase Rate, and CSAT scores) via the Power BI dashboard during routine executive business reviews

## How to Run the Project

### Prerequisites

- Python installed on your computer.
- Git installed.
- Jupyter Notebook or JupyterLab.
- Power BI Desktop to open the dashboard file included in this repository.

### 1. Clone the Repository

```bash
git clone https://github.com/Fatma460/01-Ecommerce-Analytics.git
cd 01-Ecommerce-Analytics
```

### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate the environment on Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 3. Install the Required Packages

```bash
python -m pip install -r requirements.txt
```

### 4. Download the Dataset

Download the Brazilian E-Commerce Public Dataset by Olist from [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce).

Create the required local directories and place the original CSV files in `data/raw/`. The processed datasets should be saved in `data/processed/` according to the paths expected by the notebooks.

The data files are excluded from this repository, so they must be downloaded separately.

### 5. Run the Notebooks

Start Jupyter Notebook:

```bash
jupyter notebook
```

Run the notebooks in the following order:

1. `01_Data_Loading_and_Exploration.ipynb`
2. `02_Data_Cleaning_and_Preparation.ipynb`
3. `03_Business_Analysis.ipynb`
4. `04_Visualization_and_Insights.ipynb`

Ensure that the dataset paths match your local directory structure and that the processed datasets required by later notebooks have been generated.

### 6. Open the Power BI Dashboard

Open the dashboard file using Power BI Desktop.

## Limitations

- The dataset covers a historical period from 2016 to 2018.
- Some analyses may be affected by missing timestamps and other data-quality limitations.
- Approval-time and delivery-time metrics depend on the availability and validity of the relevant timestamps.
- Observed relationships do not necessarily imply causation.
- Business recommendations should be evaluated against additional evidence and the specific business context.

## Future Improvements

Potential extensions include:

- Adding SQL-based analysis for selected business questions.
- Improving customer segmentation and retention analysis.
- Investigating the relationship between delivery delays and review scores.
- Adding more detailed time-series analysis.
- Automating data validation and dashboard refresh preparation.
- Extending the analysis with additional datasets where appropriate.

## Author

**Fatma Elzahraa**

- **GitHub:** [Fatma460](https://github.com/Fatma460)
- **LinkedIn:** [Fatma Elzahraa](https://www.linkedin.com/in/fatma-elzahraa-4196181b8/)

This project was developed as part of a Data Analytics portfolio to demonstrate data preparation, exploratory analysis, business metrics, visualization, and dashboard reporting.

If you find this project helpful, feel free to ⭐ star the repository.