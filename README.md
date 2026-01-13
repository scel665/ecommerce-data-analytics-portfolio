# ecommerce-data-analytics-portfolio
End-to-end data analytics project analysing transactional e-commerce data to uncover user behaviour, revenue trends, and channel performance using Python.

## Background
This project analyses historical transactional and user-level data from a mid-sized Australia-based e-commerce platform operating across multiple product categories, including Electronics, Home, Fashion, Beauty, and Sports.

The platform serves customers across AU, US, UK, and CA, and acquires traffic through a mix of organic, paid search, social media, and email channels.

## Data Overview
The dataset contains four core tables commonly used in e-commerce analytics:

- **users**: Customer profile and signup information  
  **Primary key:** `user_id`

- **products**: Product catalogue and pricing data  
  **Primary key:** `product_id`

- **orders**: Order-level transaction data including channel and payment information  
  **Primary key:** `order_id`  
  **Foreign key:** `user_id` → `users.user_id`

- **order_items**: Line-item level purchase details (product-level granularity)  
  **Foreign key:** `order_id` → `orders.order_id`  
  **Foreign key:** `product_id` → `products.product_id`

## Data Quality Notes
As with most production datasets, data quality issues were observed during exploration. Key challenges include:
- Missing customer and payment attributes
- Inconsistent categorical labels (channels, devices, categories)
- Invalid and extreme numeric values (e.g., zero values and outliers)
- Duplicate transactional records
- Referential and temporal inconsistencies across tables

A structured data validation and cleaning workflow is applied before analysis to ensure reliable insights.

## Project Objectives
- Conduct a data quality audit and define business rules for cleaning
- Build a clean analytical dataset via joins and validation checks
- Analyse revenue drivers, user behaviour, and channel performance
- Deliver actionable insights and recommendations for growth and operational decisions

## Tools
- Python (Pandas, NumPy)
- SQL concepts (joins, CTEs, window functions)
- Data visualisation and exploratory analysis

## Project Structure (recommended)

