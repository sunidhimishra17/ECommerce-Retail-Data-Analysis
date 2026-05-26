## ECommerce-Retail-Data-Analysis

Exploratory Data Analysis (EDA) on product dataset from Kaggle. Features data cleaning, handling missing values, IQR-based outlier detection, and univariate/bivariate visualizations using Pandas, Matplotlib, and Seaborn.

A comprehensive, production-grade Exploratory Data Analysis (EDA) pipeline developed in Python. This project utilizes the BigBasket Entire Product List dataset from Kaggle to perform automated data cleaning, statistical profiling, outlier detection, and advanced data visualization to uncover hidden market trends, pricing distributions, and brand relationships.

## Project Overview
In retail and e-commerce analytics, understanding data quality and product distribution is vital before building recommendation engines or predictive models. This project demonstrates an end-to-end data auditing framework that inputs a raw, uncurated e-commerce dataset and transforms it into actionable business intelligence using rigorous statistical methods.

## Key Features & Analysis Pipeline

* **Data Wrangling & Cleaning:** Automatically scans for, quantifies, and handles missing values (`Null` values) across product descriptions, brands, and categories.

* **Statistical Profiling:** Computes critical central tendency (Mean, Median, Mode) and dispersion metrics (Variance, Standard Deviation) for numerical values like ratings and pricing.

* **Advanced Outlier Management:** Employs the **Interquartile Range (IQR)** technique combined with data visualization to robustly identify and remove statistical anomalies.

* **Univariate Exploration:** Analyzes individual variables using customized histograms and boxplots to understand underlying feature spreads.

* **Bivariate & Multivariate Association:** Leverages scatter plots, bar plots, and correlation coefficients to evaluate constraints and patterns between multiple numerical and categorical variables.

## Tech Stack & Libraries

* **Language:** Python 3.x

* **Environment:** Jupyter Notebook / Google Colab

* **Data Manipulation:** `Pandas`, `NumPy`

* **Data Visualization:** `Matplotlib`, `Seaborn`

## Dataset Structure

The dataset processed in this analysis (`BigBasket Products.csv`) contains the following structural components:

* **Product Identifiers:** Product Name, Brand Name

* **Categorization Tags:** Main Category, Sub-Category

* **Commercial Metrics:** Sale Price, Market Price (MRP)

* **Customer Feedback:** Ratings, Product Descriptions

## Installation & Setup

### 1. Clone the Repository

    git clone https://github.com/sunidhimishra17/ECommerce-Retail-Data-Analysis.git

    cd ECommerce-Retail-Data-Analysis
### 2. Install Required Packages

    pip install pandas numpy matplotlib seaborn jupyter

## Usage & Insights

1. Launch your Jupyter Notebook environment:

       jupyter notebook

2. Open and run the EDA.ipynb script sequentially.

3. Core Insights Extracted:

   * Price vs. Rating distributions to identify premium brand groupings.

   * Visual proof of skewed price data before and after IQR filtering.

   * Correlation mapping determining whether heavy discounts directly influence customer product ratings.

## Sample Visualizations Summary

 '''text 
    
    [+] Executing Data Pipeline Diagnostics:
      
       - Missing Values Detected & Handled Successfully.
       
       - Outliers Removed via IQR: [X] data records cleaned.
       
       - Statistical Correlation Matrix Generated.

## Future Roadmap

1. Integrate Automated Feature Engineering to derive discount percentages (MRP - Sale Price) / MRP.

2. Apply Market Basket Analysis (Apriori Algorithm) to spot frequently co-purchased categories.

3. Build a lightweight interactive dashboard using Streamlit to visualize these metrics dynamically.
