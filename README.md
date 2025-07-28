# E-commerce Analysis 
## 📂 About Data 
The dataset used in this project contains records of all transactions made between December 1, 2010 and December 9, 2011 by a UK-based online retail company. The company specializes in selling gift items for various occasions, with a customer base that includes both individual consumers and wholesale distributors. 

You can find the dataset on the UCI Machine Learning Repository: [Link](https://archive.ics.uci.edu/dataset/352/online+retail)

## ✏️ Data Preprocessing
Conducted simple data cleaning:

- Converted `InvoiceDate` to datetime format and created a new column InvoiceDateOnly containing only the date part.
- Removed missing values in `CustomerID` and `Description`.
- Dropped duplicated rows.
- Removed invalid transactions with `UnitPrice` < 0. Negative `Quantity` values were kept as they represent cancellations or returns (`InvoiceNo` starting with "C").
- Removed abnormal `StockCode` values and irrelevant `Description` entries. Standardize `Description` text to uppercase.
- Added a new column `TotalPrice` calculated as `Quantity` x `UnitPrice`.

## 📊 Visualization
Created 3 interactive dashboards using Tableau to analyze different aspects of the dataset: 

- **Sales Performance:** Shows total revenue, order volume, return rates and sales trends over time.
<img width="1200" height="700" alt="Screenshot 2025-07-18 013259" src="https://github.com/user-attachments/assets/ed2b9a6b-a0b8-4518-816c-8fa72933553c" />

- **Customer Insights:** Highlights customer distribution, purchase behavior, top customers and segmentation.
<img width="1200" height="700" alt="Screenshot 2025-07-18 015017" src="https://github.com/user-attachments/assets/8ea055c5-61e3-4977-87c1-98fba28babbe" />

- **Product Analysis:** Reveals top-selling products, most returned items and sales trends by product categories.
<img width="1200" height="700" alt="Screenshot 2025-07-18 020932" src="https://github.com/user-attachments/assets/64e6b00f-08f5-41f6-9d27-0068dea948a0" />


📎 Dashboards on Tableau Public: [Link](https://public.tableau.com/app/profile/y.ho.thi.ngoc/viz/Nhom11_ProjectCK/SalesPerformance)

## 🧠 Insights Summary
- **High return rate** of 18.4% indicates a need to improve logistics, product descriptions or customer support.
- **Customer loyalty is strong**, with ~70% returning customers and high revenue per customer.  
- **Pareto principle applies** – a small number of products contribute most of the revenue.  
- **Seasonal sales trends** peak in Q4/2011 especially during November.
- **Product categories** like *Garden* and *Fashion Accessories* show strong growth potential.

## 👨‍💻 Contributors
- **Vũ Gia Huy** – Data preprocessing, presentation, report writing  
- **Đỗ Đức Phát** – Data analysis, report writing, slide design  
- **Lư Thị Ánh Tuyết** – Data visualization, report writing  
- **Hồ Thị Ngọc Ý** – Team leader, data visualization, report writing, content consolidation
