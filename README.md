# 📊 Power BI Project — E - Commerce  Sales Data Analysis  

✨ My very first Power BI data analysis project — exploring sales data, building visuals, and sharing insights! 🚀  

---

## 📌 Project Overview  
This project was created as part of my **data analytics learning journey**.  
I worked with **Orders** and **Order Details** data to practice:  

- Cleaning & transforming raw data 🧹  
- Building data models 🔗  
- Writing DAX measures 🧮  
- Designing dashboards with interactive visuals 🎨  
- Extracting business insights 💡  

---

## 🔍 Business Questions I Tried to Answer  
1️⃣ What are the **total sales, orders, and quantities**?  
2️⃣ Which **products/customers** bring the highest revenue?  
3️⃣ What is the **monthly sales trend**?  
4️⃣ Are there **seasonal patterns** in sales?  
5️⃣ What **recommendations** can we give to improve performance?  

---

## 🚀 Tools & Technologies Used
- Power BI Desktop  
- DAX (Data Analysis Expressions)  
- CSV (raw data format)  
- Git & GitHub (for version control)
  
---

## 🔧 Data Cleaning & Modeling  
- Imported **Orders.csv** & **Details.csv** into Power BI  
- Fixed data types (dates, numbers, text)  
- Built relationships: `Orders[OrderID]` → `Details[OrderID]`  
- Created a **Date Table** for time-based analysis  
- Defined **DAX measures** for KPIs  

📝 **Example DAX Measures**:  
```DAX
Total Sales = SUMX(Details, Details[UnitPrice] * Details[Quantity] * (1 - Details[Discount]))
Total Orders = DISTINCTCOUNT(Orders[OrderID])
Average Order Value (AOV) = DIVIDE([Total Sales], [Total Orders])
```

## 📊 Visuals & Dashboards  

The report includes:  

- 📌 **KPI Cards**: Total Sales, Orders, Quantity, AOV  
- 📈 **Monthly Sales Trend Line**  
- 🏆 **Top N Customers / Products** (bar charts)  
- 🌍 **Regional or Category analysis** (if applicable)  
- 📑 **Summary page** with insights & recommendations  

📸 **Sample Screenshot:**  
--->  ![Dashboard Screenshot](Screenshot%202025-08-27%20144844.png)

---

## 🧠 Insights & Recommendations  

- Sales are **growing steadily** month over month 📈  
- A few products/customers generate the **majority of revenue** (Pareto principle) 💰  
- **Seasonal spikes** show demand peaks in certain months 🎯  
- ✅ **Recommendation**: Focus on top customers/products and prepare inventory for peak seasons  

---

## 📈 Key Learnings
- Learned how to clean and model data in Power BI  
- Built KPI cards and visuals with DAX measures  
- Practiced storytelling with dashboards  
- First experience publishing a project on GitHub 🚀  

---

## 🌟 Future Improvements
- Add more datasets (customer demographics, shipping, etc.)  
- Try advanced DAX calculations  
- Publish the report to Power BI Service and share link  
- Automate data refresh with Power BI Gateway  

---

## ▶️ How to Open This Project  

1. ⬇️ Download this repo (or clone it using Git)  
2. 🖥 Open the `.pbix` file inside the `/powerbi/` folder with **Power BI Desktop**  
3. 📂 Ensure raw data (`Orders.csv`, `Details.csv`) exists in `/data/raw/`  
4. 🔄 Click **Refresh** to load the latest data  

---

## 📄 License  

📌 This project is for **learning purposes only**.  
📊 Data is **sample data (non-confidential)**.  
🙌 Feel free to explore, learn, and get inspired 🚀  



