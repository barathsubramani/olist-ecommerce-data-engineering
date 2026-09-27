# Project Workflow

## 1. Project Overview

This project implements an end-to-end data engineering and analytics platform for the Olist Brazilian E-Commerce dataset.

The solution uses Databricks, PySpark, SQL, Delta Lake, Unity Catalog, and Power BI to transform raw e-commerce data into analytics-ready datasets.

---

## 2. Data Flow

```text
Olist Brazilian E-Commerce Dataset
              |
              v
      Raw CSV Files - 9 Tables
              |
              v
   Unity Catalog Managed Volume
              |
              v
        Bronze Layer
        Raw Delta Tables
              |
              v
        Silver Layer
   Cleaned & Transformed Data
              |
              v
          Gold Layer
     Business-Ready Tables
              |
              +--------------------+
              |                    |
              v                    v
      Data Quality Checks    Delta Optimization
              |                    |
              +---------+----------+
                        |
                        v
                  Power BI
                  Dashboards
