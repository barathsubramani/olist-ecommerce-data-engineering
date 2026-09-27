# Data Dictionary

## Overview

This document describes the analytical datasets created as part of the Olist E-Commerce Data Engineering project.

The project follows a Medallion Architecture consisting of Bronze, Silver, and Gold layers.

---

## Gold Layer

### gold_sales_performance

Contains order-level sales and revenue metrics.

Purpose:

- Analyze order performance
- Track revenue
- Analyze order status
- Study customer purchasing behavior
- Support executive-level KPIs

Business use:

Used by the Executive Overview dashboard.

---

### gold_customer_360

Contains customer-level analytical information.

Purpose:

- Analyze customer purchasing behavior
- Measure customer spending
- Analyze order frequency
- Support customer segmentation
- Identify high-value customers

Business use:

Used for customer analytics and customer value analysis.

---

### gold_product_performance

Contains product and category-level performance metrics.

Purpose:

- Analyze product revenue
- Analyze units sold
- Compare product prices
- Analyze freight costs
- Evaluate product categories

Business use:

Used by the Sales & Product Analysis dashboard.

---

### gold_seller_performance

Contains seller-level performance metrics.

Purpose:

- Analyze seller revenue
- Analyze seller sales volume
- Compare seller performance
- Analyze seller locations

Business use:

Used for seller performance analysis.

---

### gold_delivery_performance

Contains delivery and logistics performance metrics.

Purpose:

- Analyze delivery duration
- Measure on-time delivery
- Identify late deliveries
- Analyze delivery performance over time

Business use:

Used for operational and logistics analysis.

---

### gold_payment_analysis

Contains payment-level analytical metrics.

Purpose:

- Analyze payment methods
- Analyze payment values
- Analyze installment behavior
- Understand customer payment patterns

Business use:

Used for payment analysis.

---

### gold_review_analysis

Contains customer review and satisfaction metrics.

Purpose:

- Analyze review scores
- Measure positive and negative reviews
- Analyze customer satisfaction
- Evaluate review trends

Business use:

Used for customer satisfaction and review analysis.

---

## Data Layers

| Layer | Description |
|---|---|
| Bronze | Raw source data converted into Delta tables |
| Silver | Cleaned and transformed data |
| Gold | Business-ready analytical datasets |

---

## Data Quality

The Gold layer is validated using automated data quality checks covering:

- Completeness
- Uniqueness
- Business rules
- Negative values
- Invalid review scores
- Delivery metrics
- Payment values

---

## Analytical Consumption

The Gold datasets are consumed by Power BI to create interactive dashboards for:

- Executive reporting
- Sales analysis
- Product analysis
- Customer analysis
- Seller analysis
- Delivery analysis
- Payment analysis
- Review analysis
