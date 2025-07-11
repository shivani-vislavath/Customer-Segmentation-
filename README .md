# Customer Demographics & Behavioral Insights

It explores customer demographics and behavioral patterns through powerful data visualization using **Power BI**.

---

## 📍 Project Objective

This project addresses the task of creating a bar chart or histogram to visualize the distribution of a categorical or continuous variable. Specifically, it uses Power BI to analyze a population dataset and highlight patterns such as:

Distribution of gender (categorical)

Distribution of age and income (continuous)

Segment-level insights using interactive filters (slicers)

---

## 🛠 Tools & Technologies

* **Power BI Desktop**
* Sample customer demographic dataset (CSV)

---

## 📈 Key KPIs

| KPI                    | Value | Description                                      |
| ---------------------- | ----- | ------------------------------------------------ |
| **Customers**          | 200   | Total customer count in dataset                  |
| **Avg Income (k\$)**   | 60.56 | Average annual income                            |
| **Avg Spending Score** | 50.20 | Overall customer spending tendency (1–100 scale) |

---

## 📊 Visualizations Included

### 1. 💰 **Income vs Spending Score**

* **Chart Type**: Scatter plot
* **Insight**: No direct correlation; both low and high earners exhibit varied spending behaviors.

### 2. 🔍 **Customer Segmentation Heatmap**

* **Chart Type**: Matrix
* **Insight**: Highest average spending observed in the 26–35 female segment (64.65).

### 3. 📈 **Spending Score by Age Group**

* **Chart Type**: Bar chart
* **Insight**: Customers aged 26–35 are the most engaged spenders.

### 4. 👤 **Gender Distribution of Customers**

* **Chart Type**: Bar chart
* **Insight**: Female customers (112) slightly outnumber male customers (88).

### 5. 📅 **Average Income by Gender**

* **Chart Type**: Column chart
* **Insight**: Males have a slightly higher average income (62.23k) compared to females (59.25k).

### 6. 🌐 **Income Distribution of Customers**

* **Chart Type**: Histogram-style column chart
* **Insight**: Majority of customers fall within the 41k–70k income range.

### 7. 📅 **Customer Count by Age Group**

* **Chart Type**: Column chart
* **Insight**: Highest number of customers in the 26–35 age group (60).

### 8. 🎛️ **Slicers for Age and Gender**

* **Visual Type**: Slicers (interactive filters)
* **Insight**: Enables users to filter all visualizations dynamically by specific age groups or gender to explore behavior within segments.

---

## 💡 Key Insights Summary

* 👧 **Top Segment**: Females aged 26–35 with highest average spending score (64.65)
* 🧮 **Spending vs Income**: No linear trend, indicating diverse customer behavior
* 👥 **Demographic Reach**: Balanced gender distribution with concentration in young adults

---

## 📘 DAX Calculations Used

### 🎂 AgeGroup Binning:

```DAX
AgeGroup = 
SWITCH(TRUE(),
    Customers[Age] <= 25, "18–25",
    Customers[Age] <= 35, "26–35",
    Customers[Age] <= 45, "36–45",
    Customers[Age] <= 55, "46–55",
    "56+"
)
```

### 💵 IncomeGroup Binning:

```DAX
IncomeGroup = 
SWITCH(TRUE(),
    Customers[Annual Income (k$)] <= 40, "0–40",
    Customers[Annual Income (k$)] <= 70, "41–70",
    Customers[Annual Income (k$)] <= 100, "71–100",
    "101+"
)
```

---

## 📁 Files Included

*https://github.com/shivani-vislavath/-PRODIGY_DS_01-/blob/main/customer_demographics_Dashboard.pbix - Power BI dashboard
* https://github.com/shivani-vislavath/-PRODIGY_DS_01-/blob/main/Dashboard_preview.png.png - Dashboard screenshot

---

## 👨‍💻 Author

**Shivani Vislavath**
📧 [shivanivislavath02@gmail.com](mailto:shivanivislavath02@gmail.com)
🔗 [LinkedIn](https://www.linkedin.com/in/shivani-vislavath-680102286)
🔗 [GitHub](https://github.com/shivani-vislavath)

---

If you found this useful, feel free to ⭐ star this project or connect with me!
