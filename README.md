# Brazilian E-Commerce Data Analysis | Olist Analytics

## Project Overview

This project analyzes the Brazilian E-Commerce Public Dataset by Olist to explore sales performance, customer behavior, product performance, and order delivery operations.

The dataset contains e-commerce transactions and related information from 2016 to 2018. Using Python for data preparation and exploratory analysis and Power BI for interactive reporting, the project transforms raw data into business insights that can support data-driven decision-making.

The project follows a structured analytics workflow, from data loading and cleaning to business analysis, visualization, and dashboard development.

## Business Objectives

The main objectives of this project are to:

- Measure overall sales performance and order volume.
- Analyze customer purchasing behavior and repeat-purchase patterns.
- Identify top-performing and low-performing product categories.
- Compare sales performance across Brazilian states and cities.
- Evaluate order approval and delivery timelines.
- Analyze late deliveries and delivery performance.
- Explore payment methods and their contribution to sales.
- Build an interactive Power BI dashboard to communicate key findings.
- Translate analytical findings into actionable business recommendations.

## Dataset

**Source:** Brazilian E-Commerce Public Dataset by Olist

The dataset is publicly available on Kaggle:

[Access the Olist Dataset on Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

It contains multiple related tables describing customers, orders, products, payments, sellers, reviews, and geographic information.

### Dataset Tables

| Table                        | Description                                                   |
| ---------------------------- | ------------------------------------------------------------- |
| Customers                    | Customer identifiers and geographic information               |
| Orders                       | Order status and timestamps for the order lifecycle           |
| Order Items                  | Products purchased in each order, prices, and freight values  |
| Products                     | Product attributes, categories, and dimensions                |
| Payments                     | Payment methods, installments, and payment values             |
| Reviews                      | Customer review scores and comments                           |
| Sellers                      | Seller identifiers and locations                              |
| Product Category Translation | Portuguese-to-English product category translations           |
| Geolocation                  | Geographic coordinates associated with Brazilian postal codes |

The analysis focuses on the tables required to answer the project's business questions. Other tables are available for additional analysis where relevant.

**Dataset period:** 2016–2018.

**Important note:** This is a historical dataset. Its results describe the available data and should not be interpreted as a representation of the current e-commerce market.

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
- **Power Query** — Data transformation and preparation where applicable

### Development and Project Management

- **Jupyter Notebook** — Organizing the analytical workflow
- **Git and GitHub** — Version control and project documentation
- **SQLAlchemy and DuckDB** — Available analytical tools in the project environment

## Project Structure

```text
01-Ecommerce-Analytics/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── 01_Data_Loading_and_Exploration.ipynb
│   ├── 02_Data_Cleaning_and_Preparation.ipynb
│   ├── 03_Business_Analysis.ipynb
│   └── 04_Visualization_and_Insights.ipynb
│
├── dashboard/
│   └── Olist_Ecommerce_Analytics_Dashboard.pbix
│
├── screenshots/
│   ├── 01_Executive_Overview.png
│   ├── 02_Sales_Performance.png
│   ├── 03_Product_Analysis.png
│   ├── 04_Customer_Geographic_Analysis.png
│   └── 05_Orders_Delivery_Analysis.png
│
├── README.md
└── requirements.txt
```

## Analytical Workflow

### 1. Data Loading and Exploration

The initial stage focuses on understanding the dataset structure and assessing data quality.

Activities include:

- Loading the relevant CSV files into Pandas DataFrames.
- Inspecting dataset dimensions, column names, and data types.
- Reviewing summary statistics and unique values.
- Identifying missing values and potential data-quality issues.
- Exploring relationships between customers, orders, order items, and products.

### 2. Data Cleaning and Preparation

The data preparation stage focuses on making the datasets suitable for reliable analysis.

Activities include:

- Handling missing values where appropriate.
- Converting timestamp columns to datetime data types.
- Reviewing duplicates and data consistency.
- Preparing cleaned datasets for analysis and reporting.
- Creating or deriving fields needed for business metrics.
- Exporting processed datasets for reuse in the analytical workflow.

Cleaning decisions depend on the meaning of each column and its relevance to the analysis.

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

### 4. Visualization and Insights

Charts are used to communicate patterns, comparisons, and trends found during the analysis.

The visualizations support the interpretation of results and help identify areas that may require further investigation.

### 5. Power BI Dashboard

Power BI brings the main metrics and findings together in an interactive reporting experience.

The dashboard is designed to help users explore performance across relevant dimensions, including time, geography, products, customers, and order delivery.

## Power BI Dashboard

The dashboard is organized into five pages, covering the main analytical areas of the project.

### 1. Executive Overview

Provides a high-level summary of business performance through key performance indicators and an overview of the main metrics.



### 2. Sales Performance

Explores sales trends and performance across the available time period and relevant business dimensions.



### 3. Product Analysis

Examines product and category performance to identify leading contributors and areas for further investigation.



### 4. Customer and Geographic Analysis

Explores customer distribution and geographic performance across Brazilian states and cities.



### 5. Orders and Delivery Analysis

Examines order statuses, delivery timelines, and delivery performance, including late-delivery patterns.



## Key Findings

The project investigates the following business areas:

- **Customer behavior:** The distribution of one-time and repeat customers.
- **Sales performance:** Changes in sales and order activity over time.
- **Product performance:** Categories and products contributing most to sales.
- **Geographic performance:** Differences in sales and order activity across locations.
- **Payment behavior:** The distribution of payment methods and their relationship with order value.
- **Delivery operations:** Order approval times, delivery durations, and late-delivery patterns.

The final findings should be interpreted alongside the corresponding metrics and visualizations in the notebooks and dashboard.

## Business Recommendations

The analysis can support recommendations in several areas:

- **Customer retention:** Investigate repeat-purchase behavior and consider strategies to encourage customers to return.
- **Product strategy:** Review high-performing categories and investigate low-performing categories before making inventory decisions.
- **Geographic strategy:** Compare regional sales performance with order volume and delivery performance when prioritizing markets.
- **Delivery operations:** Investigate the factors associated with late deliveries and identify opportunities to improve the customer experience.
- **Payment analysis:** Use payment-method patterns to inform further investigation into customer preferences and order value.
- **Performance monitoring:** Track key metrics through the dashboard to support ongoing business review.

These are potential recommendations based on the questions explored in the project. Specific business actions should be supported by the validated analytical results.

## How to Run the Project

### Prerequisites

- Python installed on your computer.
- Git installed if you plan to clone the repository.
- Jupyter Notebook or JupyterLab.
- Power BI Desktop to open the `.pbix` dashboard file.

### 1. Clone the Repository

Replace `your-repo-name` with the actual GitHub repository name.

```bash
git clone https://github.com/Fatma460/your-repo-name.git
cd your-repo-name
```

### 2. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it on Windows PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

### 3. Install the Required Packages

```bash
python -m pip install -r requirements.txt
```

### 4. Add the Dataset

Download the dataset from Kaggle and place the CSV files in the appropriate data directory.

Use the folder paths expected by the notebooks. If the raw dataset is not included in the repository, download it separately before running the analysis.

### 5. Run the Notebooks

Open Jupyter Notebook from the project environment:

```bash
jupyter notebook
```

Run the notebooks in the following order:

1. `01_Data_Loading_and_Exploration.ipynb`
2. `02_Data_Cleaning_and_Preparation.ipynb`
3. `03_Business_Analysis.ipynb`
4. `04_Visualization_and_Insights.ipynb`

Make sure the dataset paths and the locations of processed files match your local project structure.

### 6. Open the Power BI Dashboard

Open the `.pbix` file inside the `dashboard/` folder using Power BI Desktop. If the dashboard uses local CSV files, update the data-source paths as needed.

## Limitations

- The dataset covers a historical period from 2016 to 2018.
- Some analyses may be affected by missing timestamps or other data-quality limitations.
- Delivery and approval metrics depend on the availability and validity of the relevant timestamps.
- Observed relationships do not necessarily imply causation.
- Recommendations should be evaluated against business context and additional data before implementation.

## Future Improvements

Potential extensions include:

- Adding SQL-based analysis for selected business questions.
- Improving customer segmentation and retention analysis.
- Investigating the relationship between delivery delays and review scores.
- Adding more detailed time-series analysis.
- Automating data validation and dashboard refresh preparation.
- Extending the analysis with additional datasets when appropriate.

## Author

**Fatma**

- **GitHub:** [Fatma460](https://github.com/Fatma460)
- **LinkedIn:** [LinkedIn Profile](https://www.linkedin.com/)

---

*This project was developed as part of a Data Analytics portfolio to demonstrate data preparation, exploratory analysis, business metrics, visualization, and dashboard reporting.*













9- Author
Fatma
GitHub: [fatmaelzahraa460](https://github.com/Fatma460)
LinkedIn: [Fatma Elzahraa](https://www.linkedin.com/in/fatma-elzahraa-4196181b8/)
Feel free to star ⭐️ this repository if you found it helpful!