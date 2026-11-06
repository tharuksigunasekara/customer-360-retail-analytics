# Customer 360° – Retail Purchase Analytics

A customer-focused retail analytics dashboard developed using **Microsoft Fabric, SQL, Power BI, and DAX** to analyse individual customer purchasing behaviour and generate rule-based product recommendations.

## Project Overview

In retail, understanding customer purchasing habits can help sales consultants provide a more personalised shopping experience.

This project demonstrates how customer membership and transaction data can be transformed into an interactive Customer 360° dashboard.

Instead of analysing overall store performance, the dashboard focuses on **individual customers**, helping identify their purchase history, spending patterns, preferred product categories, and shopping branches.

## Objectives

- Analyse individual customer purchasing behaviour.
- Track customer spending and purchase frequency.
- Identify frequently purchased product categories.
- Understand customer spending across different branches.
- Display detailed customer purchase history.
- Generate simple rule-based next-purchase recommendations.

## Technologies Used

| Technology | Purpose |
|---|---|
| Microsoft Fabric | Data storage and management using Lakehouse |
| SQL | Data validation and querying |
| Power BI | Interactive dashboard and data visualisation |
| DAX | Business calculations and recommendation rules |
| CSV | Synthetic customer and transaction datasets |

## Dataset

The project uses **100% synthetic data** created for learning and demonstration purposes.

The dataset contains:

- 5 fictional customers
- 5 product categories
- 3 illustrative retail branches
- 60 sample purchase transactions

### Data Model

Four tables are used:

| Table | Description |
|---|---|
| customers | Customer and membership information |
| products | Product details, categories, and prices |
| branches | Retail branch information |
| transactions | Customer purchases, quantities, dates, and amounts |

The tables are connected using one-to-many relationships in the Power BI semantic model.

## Dashboard Features

### 1. Customer Selection

Select an individual customer to view their purchasing behaviour.

### 2. Total Spending

Calculate the total amount spent by the selected customer.

### 3. Purchase Frequency

Display the number of purchase transactions associated with the customer.

### 4. Favourite Product Category

Identify the customer's most frequently purchased category based on total item quantity.

Categories include Shirts, Pants, Polos, T-Shirts, and Blazers.

### 5. Branch Spending Analysis

Visualise customer spending across different retail branches.

### 6. Purchase History

Display individual purchases, including purchase dates, products, categories, quantities, branches, and transaction amounts.

### 7. Rule-Based Next Purchase Recommendation

The dashboard includes a **rule-based recommendation system implemented using DAX**.

Recommendations are generated using predefined business rules based on the customer's favourite product category.

Example recommendation rules:

| Favourite Category | Recommended Product |
|---|---|
| Shirts | Pants |
| Pants | Shirts |
| Polos | Chino Pants |
| T-Shirts | Polos |
| Blazers | Formal Shirts |

For example, if a customer frequently purchases shirts, the system recommends pants as a complementary product.

**Important:** This feature uses predefined recommendation rules. It does not use machine learning, predictive modelling, or AI-based forecasting.

Recommendations are illustrative and are not validated predictions of future purchases.

## Data Processing Workflow

1. Generate synthetic customer and purchase data.
2. Upload CSV files into Microsoft Fabric Lakehouse.
3. Create a Power BI semantic model.
4. Establish relationships between customer, product, branch, and transaction tables.
5. Create DAX measures for customer analytics.
6. Develop interactive Power BI visualisations.
7. Implement rule-based product recommendations.

## Future Improvements

Potential enhancements include:

- Python-based customer purchasing analysis.
- Machine-learning models for next-purchase prediction.
- Customer segmentation using RFM analysis.
- Purchase frequency and recency analysis.
- Snowflake integration for cloud data warehousing.
- Expanded synthetic datasets for more realistic analysis.

These enhancements are planned and are not part of the current implementation.

## Disclaimer

This is an independent educational and portfolio project inspired by common retail membership and sales processes.

All customer names, membership details, transactions, and branch records are fictional or illustrative.

No real customer information, confidential company data, or proprietary transaction records have been used.

This project is not affiliated with or endorsed by POLITIX.

## Project Status

**Version 1.0 — Minimum Viable Product (MVP)**

Core customer analytics dashboard and rule-based recommendation logic implemented.

## Author

Tharuksi Gunasekara

Developed as a hands-on learning project focused on retail analytics, business intelligence, and data-driven customer insights.
