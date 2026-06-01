# 📊 Amazon Sales Data Analysis — Data Visualization & Storytelling

## 📌 Project Overview

This project focuses on **Data Visualization and Storytelling** using the **Amazon Sales Dataset**. The objective was to transform raw sales and customer review data into meaningful visual insights using **Power BI**.

The dashboard was designed to highlight important **business insights** related to product categories, customer satisfaction, discounts, pricing strategy, and customer engagement.

The project emphasizes **storytelling through visualizations**, helping understand how product pricing, ratings, and discounts influence customer behavior on Amazon.

## 🎯 Objective

To create meaningful and interactive visualizations that communicate a compelling business story from Amazon sales data.

## 🛠 Tools & Technologies Used

- **Power BI Desktop**
- **Microsoft Excel**
- **Kaggle Dataset**
- **Data Cleaning & Transformation**
- **Data Visualization & Storytelling**

## 📂 Dataset Information

**Dataset Name:** Amazon Sales Dataset

**Source:** Kaggle

Dataset Link: https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset

### Features Used

- `product_id` → Product ID
- `product_name` → Product Name
- `category` → Product Category
- `discounted_price` → Discounted Product Price
- `actual_price` → Original Product Price
- `discount_percentage` → Discount Percentage
- `rating` → Customer Rating
- `rating_count` → Number of Customer Reviews
- `review_title` → Review Title
- `review_content` → Product Review


# 🧹 Data Preparation & Cleaning

The dataset was cleaned and transformed in **Power Query Editor** before creating visualizations.

### Cleaning Steps Performed

✔ Removed unnecessary columns:
- `img_link`
- `product_link`
- `user_id`
- `review_id`

✔ Fixed data types for:
- Prices
- Ratings
- Rating counts
- Discount percentage

✔ Removed currency symbols (`₹`) and commas from price columns.

✔ Converted numerical columns into proper numeric format.

✔ Handled null values and formatting issues.

✔ Created calculated measures for analysis.

# 📈 Dashboard Pages & Storytelling

## 1️⃣ Overview Dashboard

### Visualizations
- Product Count by Category
- Customer Ratings by Category

### Key Insight
Electronics and computer-related categories dominate Amazon’s marketplace, indicating higher customer demand and stronger market presence.

## 2️⃣ Pricing Story

### Visualizations
- Top Discounted Products
- Actual Price vs Discounted Price

### Key Insight
Amazon uses discount strategies to improve customer engagement and increase product sales. Electronics products receive higher discounts compared to other categories.

## 3️⃣ Customer Satisfaction Story

### Visualizations
- Product Rating Distribution
- Customer Review Count by Category

### Key Insight
Most products maintain ratings above **4.0**, indicating strong customer satisfaction and trust in product quality.

## 4️⃣ Summary & Business Insights

### KPI Metrics Used
- Total Products
- Average Rating
- Average Discount Percentage
- Total Review Count

### Final Business Insights
- Electronics dominate Amazon sales categories.
- Most products receive positive customer ratings.
- Discounts significantly influence product visibility.
- Customer engagement is higher for top-rated products.
- Review activity helps identify high-performing categories.

## 📁 Repository Structure

```text
amazon-sales-data-visualization/
│── Amazon Sales Dashboard.pbix
│── Amazon Sales Dashboard.pdf
│── README.md
│── amazon.csv
