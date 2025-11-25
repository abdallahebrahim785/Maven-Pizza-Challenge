# 🍕 Maven Pizza Challenge - Business Intelligence Analysis

![Maven Pizza Challenge](https://img.shields.io/badge/Maven%20Analytics-Challenge-orange)
![Python](https://img.shields.io/badge/Python-3.8+-blue)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow)
![Status](https://img.shields.io/badge/Status-Complete-success)

## 📊 Project Overview

This project analyzes customer transaction data for **Plato's Pizza**, a Greek-inspired pizza restaurant in New Jersey, to identify opportunities for increasing sales and improving operational efficiency.

**Role:** BI Consultant  
**Client:** Plato's Pizza  
**Tools Used:** Python, Power BI, Pandas, YData Profiling  
**Duration:** November 2025  
**Challenge Source:** [Maven Pizza Challenge](https://mavenanalytics.io/challenges/maven-pizza-challenge)

---

## 🎯 Business Objectives

The analysis aims to answer five critical business questions:

1. ❓ **What days and times is the restaurant busiest?**
2. ❓ **How many pizzas are made during peak periods?**
3. ❓ **What are the best and worst selling pizzas?**
4. ❓ **What's the average order value?**
5. ❓ **How well is the restaurant utilizing seating capacity?** (15 tables, 60 seats)

---

## 📁 Project Structure

```
maven-pizza-challenge/
│
├── data/
│   ├── raw/                          # Original datasets
│   ├── cleaned/                      # Cleaned datasets
│   └── orders_summary.csv            # Aggregated order data
│
├── notebooks/
│   ├── 01_data_loading.ipynb        # Data loading & inspection
│   ├── 02_data_profiling.ipynb      # YData profiling analysis
│   ├── 03_data_preprocessing.ipynb  # Data cleaning & transformation
│   └── 04_exploratory_analysis.ipynb # EDA (Uni/Bi/Multi-variate)
│
├── powerbi/
│   └── Maven_Pizza_Dashboard.pbix    # Power BI dashboard file
│
├── requirements.txt                  # Python dependencies
├── README.md                         # Project documentation
└── LICENSE                           # MIT License

```

---

## 🔧 Technologies Used

### **Python Libraries:**
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **YData Profiling** - Automated exploratory data analysis
- **Matplotlib & Seaborn** - Data visualization

### **Business Intelligence:**
- **Power BI Desktop** - Interactive dashboard creation
- **DAX** - Data Analysis Expressions for measures

---

## 📝 Data Preprocessing Steps

### **1. Orders Table**
- ✅ Converted `order_date` and `order_time` to proper datetime format
- ✅ Extracted temporal features: `year`, `month_name`, `day_name`, `hour`, and `day_part`

### **2. Order Details Table**
- ✅ Removed outliers in `quantity` column using IQR method
- ✅ Created `order_summary` DataFrame (grouped by `order_id` and summed quantity)

### **3. Pizzas Table**
- ✅ Standardized `size` column: 'S' → 'Small', 'M' → 'Medium', 'L' → 'Large', 'XL' → 'Extra Large', 'XXL' → 'Double Extra Large'
- ✅ Removed outliers in `price` column

### **4. Pizza Types Table**
- ✅ Removed prefix “The” from pizza names
- ✅ Created `ingredients_count` column by counting ingredients

### **5. Data Quality Checks**
- ✅ Checked for missing values
- ✅ Removed duplicates
- ✅ Ensured data consistency and integrity

---

## 📊 Exploratory Data Analysis

Performed **Univariate**, **Bivariate**, and **Multivariate** analyses:
- Distribution of orders, prices, and categories
- Relationships between revenue, time, and pizza size
- Heatmaps and category performance matrices

---

## 📈 Key Insights

- **Busiest Hour:** 12:00 PM (Lunch time)  
- **Busiest Day:** Friday  
- **Peak Period Pizzas:** 6,322 pizzas made during peak  
- **Top Seller:** Thai Chicken Pizza  
- **Worst Seller:** Barbecue Chicken Pizza  
- **Most Popular Size:** Large (45.9%)  
- **Total Revenue:** $785.5K  
- **Average Order Value:** $36.90  
- **Seating Utilization:** 30.93% (underutilized)

---

## 🎨 Power BI Dashboard

You can explore the interactive dashboard here 👇  
🔗 **Power BI Report:** [View Dashboard](https://app.powerbi.com/view?r=eyJrIjoiNjA4ZTg0MzYtYTRhYS00MWQxLThmYzUtOTNiZDkyYjEwYmZmIiwidCI6ImVhZjYyNGM4LWEwYzQtNDE5NS04N2QyLTQ0M2U1ZDc1MTZjZCIsImMiOjh9)

🔗 **Challenge & Dataset:** [Maven Analytics - Maven Pizza Challenge](https://mavenanalytics.io/challenges/maven-pizza-challenge)

---

## 💡 Business Recommendations

1. **Increase Marketing Visibility** – Promote during lunch & dinner rush hours.  
2. **Focus on Best Sellers** – Emphasize Thai Chicken Pizza and large sizes.  
3. **Enhance Operations** – Staff training & online ordering for efficiency.  
4. **Optimize Menu** – Consider removing low-performing pizzas.  
5. **Target Growth** – Aim for 65-75% seat utilization.

---

## 🎓 Learning Outcomes

- ✅ Data Cleaning & Preprocessing  
- ✅ Exploratory Data Analysis  
- ✅ Power BI Dashboarding  
- ✅ DAX Calculations  
- ✅ Business Storytelling

---

## 📫 Connect With Me

- **LinkedIn:** [Abdallah Ibrahim](https://linkedin.com/in/abdallah-ibrahim-4556792a5)  
- **Email:** abdallahebrahim785@gmail.com  
- **GitHub:** [github.com/abdallahebrahim785](https://github.com/abdallahebrahim785)

---

## 🙏 Acknowledgments

- **Maven Analytics** – For the challenge and dataset inspiration.  
- **Power BI Community** – For design inspiration.

---

**Built with ❤️ by Abdallah Ibrahim**

