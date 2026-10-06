# 🛒 Vrinda Store – Annual Sales Analysis 2022 (Excel)

An Excel-based data analysis project that turns **31,047 online order records** from a fashion retailer into an interactive annual sales dashboard. The analysis covers monthly sales trends, customer demographics, sales channels, order status, and top-performing states.

---

## 📂 Repository Structure

```
├── Vrinda_Store_Data_Analysis.xlsx   # Raw data, pivot tables, and final dashboard
└── README.md
```

### Workbook Sheets

| Sheet | Purpose |
|---|---|
| `Vrinda Store` | Cleaned raw dataset (31,047 rows, 21 columns) |
| `Order Vs sales` | Pivot: monthly sales amount vs. order count |
| `Men Vs Women` | Pivot: sales split by gender |
| `Order Status` | Pivot: Delivered / Returned / Cancelled / Refunded |
| `States` | Pivot: top 5 states by sales |
| `Age and Gender` | Pivot: order share by age group and gender |
| `Channels` | Pivot: order share by sales channel |
| `Vrinda Report 2022` | **Final dashboard** combining all charts |

---

## 📊 Dataset

Each row is an order line with these fields:

`Order ID`, `Cust ID`, `Gender`, `Age`, `Age Group`, `Date`, `Month`, `Status`, `Channel`, `SKU`, `Category`, `Size`, `Qty`, `currency`, `Amount`, `ship-city`, `ship-state`, `ship-postal-code`, `ship-country`, `B2B`

- **Period:** 2022
- **Currency:** INR (₹)
- **Categories:** Set, Kurta, Western Dress, Top, Saree, Ethnic Dress, Blouse, Bottom
- **Channels:** Amazon, Myntra, Flipkart, Ajio, Meesho, Nalli, Others

---

## 🛠️ Tools & Techniques

- **Microsoft Excel**
- **Data cleaning:** removing duplicates/blank values, standardising fields
- **Formulas:** `IF` to create age groups, `TEXT` to extract the month from the order date
- **Pivot Tables & Pivot Charts**
- **Slicers** for interactive filtering
- **Dashboard design** with bar and pie charts

### Derived columns

```excel
Age Group:  =IF(Age>=50,"Senior",IF(Age>=30,"Adult","Teenager"))
Month:      =TEXT(Date,"mmm")
```

---

## 🎯 Business Questions Answered

1. How do sales and order volume change month by month?
2. Who buys more: men or women?
3. Which age group buys the most?
4. Which states generate the most revenue?
5. Which sales channels drive the most orders?
6. What share of orders are delivered, returned, cancelled, or refunded?

---

## 🔍 Key Insights

- **Total sales: ≈ ₹2.12 crore (₹21.18M)** across the year.
- **Women drive the majority of revenue:** about **64%** of sales (₹13.56M) vs. **36%** for men (₹7.61M).
- **Adult women (30–49)** are the largest customer segment, at roughly **35%** of orders.
- **Peak month is March** (₹1.93M, 2,819 orders); sales **decline steadily through the second half** of the year, with November at the lowest points (₹1.62M).
- **Top 5 states:** Maharashtra (₹2.99M), Karnataka (₹2.65M), Uttar Pradesh (₹2.10M), Telangana (₹1.71M), Tamil Nadu (₹1.68M), which together account for a large share of revenue.
- **Amazon is the leading channel at ~35% of orders**, followed by Myntra (~23%) and Flipkart (~22%).
- **Order fulfilment:** 28,641 orders were delivered, while **1,045 were returned, 844 cancelled, and 517 refunded** (≈ 8% not completed successfully).
- **Product mix:** *Set* and *Kurta* are the most ordered categories, with Sets generating the highest revenue (≈ ₹10.5M).

---

## 💡 Recommendations

- Focus marketing on **women aged 30–49**, the highest-value segment.
- Strengthen presence on **Amazon, Myntra, and Flipkart**, and test growth on under-used channels such as Meesho and Ajio.
- Investigate the **second-half sales decline** and plan promotions or new launches for Q3–Q4.
- Prioritise inventory and logistics in the **top 5 states**.
- Look into reasons for **returns and cancellations** to reduce lost revenue.

---

## 🚀 How to Use

1. Download `Vrinda_Store_Data_Analysis.xlsx`.
2. Open it in **Microsoft Excel** (2016 or later recommended for slicer support).
3. Go to the **`Vrinda Report 2022`** sheet to view the dashboard.
4. Use the slicers to filter the charts. The pivot sheets show the underlying numbers.

> 📸 *Add a screenshot of the dashboard here:* `![Dashboard](images/dashboard.png)`

---

## 💡 Skills Demonstrated

- Data cleaning and preparation in Excel
- Pivot tables and pivot charts
- Dashboard design and data storytelling
- Translating data into business insights and recommendations

---
