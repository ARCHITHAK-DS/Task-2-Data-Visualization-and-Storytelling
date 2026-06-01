# 📊 Amazon Sales Data Analysis — Data Visualization & Storytelling

## 📌 Project Overview

This project focuses on **Data Visualization and Storytelling** using the **Amazon Sales Dataset** from Kaggle.  
The objective was to transform raw sales and customer review data into meaningful visual insights using **Power BI**.

The dashboard is structured as a **4-page storytelling report**, each page uncovering a different dimension of Amazon's product and customer data — from pricing strategies to customer satisfaction.

## 🎯 Objective

> To create meaningful and interactive visualizations that communicate a compelling business story from Amazon sales data — focusing on **business insights**, not just visuals.

## 🛠 Tools & Technologies Used

| Tool | Purpose |
|------|---------|
| **Power BI Desktop** | Dashboard creation & visualization |
| **Power Query Editor** | Data cleaning & transformation |
| **Microsoft Excel / CSV** | Raw data handling |
| **Kaggle** | Dataset source |

## 📂 Dataset Information

**Dataset Name:** Amazon Sales Dataset  
**Source:** [Kaggle — Amazon Sales Dataset](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset)

### Features Used

| Column | Description |
|--------|-------------|
| `product_id` | Unique Product Identifier |
| `product_name` | Name of the Product |
| `category` | Product Category (pipe-separated hierarchy) |
| `discounted_price` | Price after discount (₹) |
| `actual_price` | Original MRP (₹) |
| `discount_percentage` | Discount offered (%) |
| `rating` | Average customer rating (out of 5) |
| `rating_count` | Number of customer reviews |
| `review_title` | Short review headline |
| `review_content` | Full customer review text |

## 🧹 Data Preparation & Cleaning

All cleaning was performed inside **Power Query Editor** in Power BI before building visualizations.

### Steps Performed

- ✅ Removed irrelevant columns: `img_link`, `product_link`, `user_id`, `review_id`
- ✅ Removed `₹` symbols and commas from `discounted_price` and `actual_price`
- ✅ Removed `%` symbol from `discount_percentage` and converted to numeric
- ✅ Fixed data types for prices, ratings, rating counts, and discount percentage
- ✅ Handled null values and inconsistent formatting
- ✅ Extracted `main_category` from the pipe-separated category column
- ✅ Created calculated measures for KPI cards (Avg Rating, Avg Discount %, Total Reviews)


## 📈 Dashboard Pages & Data Story

### Page 1 — 🏠 Overview Dashboard
**Story: "What does Amazon's product landscape look like?"**

| Visual | Fields Used |
|--------|-------------|
| Bar Chart — Product Count by Category | `category`, `product_name` (count) |
| Bar Chart — Sum of Ratings by Category | `category`, `rating` |

**💡 Key Insight:**  
Computers & Accessories and Electronics dominate Amazon's catalog, indicating stronger market presence and higher customer demand in these segments.


### Page 2 — 💰 Pricing Story
**Story: "How is Amazon playing the discount game?"**

| Visual | Fields Used |
|--------|-------------|
| Bar Chart — Top Discounted Products | `product_name`, `discount_percentage` |
| Clustered Bar Chart — Actual vs Discounted Price by Category | `category`, `actual_price`, `discounted_price` |
| Slicers (Filters) | `category`, `rating`, `discount_percentage`, `product_name` |

**💡 Key Insight:**  
Brands like Fire-Boltt and boAt receive exceptionally high discounts — this is a deliberate strategy to boost visibility and sales volume. The large gap between actual and discounted prices across Electronics reflects aggressive competitive pricing.

### Page 3 — ⭐ Customer Satisfaction Story
**Story: "Are customers happy, and who is engaging the most?"**

| Visual | Fields Used |
|--------|-------------|
| Histogram — Rating Distribution | `rating`, `product_name` (count) |
| Treemap — Review Count by Category | `category`, `rating_count` |

**💡 Key Insight:**  
Most products receive ratings between **4.0 and 4.5**, showing overall positive customer satisfaction. Electronics (Headphones, Mobiles) and Computers & Accessories generate the highest review counts — indicating high buyer engagement in these categories.

### Page 4 — 📋 Summary & Business Insights
**Story: "The four numbers every decision-maker needs."**

| KPI Card | Value | Interpretation |
|----------|-------|----------------|
| **Total Products** | 1K | Broad catalog analyzed |
| **Average Rating** | 4.10 | Customers are broadly satisfied |
| **Average Discount %** | 0.48 (48%) | Aggressive pricing strategy platform-wide |
| **Total Review Count** | 27M | Massive customer engagement & social proof |

## 🔍 Final Business Insights

1. **Electronics dominates** Amazon's catalog by product count and customer reviews.
2. **48% average discount** reflects a platform-wide aggressive pricing strategy.
3. **Most products rated 4.0–4.5** — customers are broadly satisfied with purchases.
4. **High review counts** in Electronics and Computer Accessories signal strong buyer engagement.
5. **Brands with heavy discounts** (Fire-Boltt, boAt) tend to dominate category visibility.

## 📁 Repository Structure

```
amazon-sales-data-visualization/
│
├── Amazon Sales Dashboard.pbix      ← Power BI source file
├── Amazon Sales Dashboard.pdf       ← Exported dashboard (deliverable)
├── amazon.csv                       ← Raw dataset from Kaggle
└── README.md                        ← Project documentation (this file)
```
