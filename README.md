# Data Leverager – Power Query ETL Project

## 📌 Project Title  
**Data Leverager – Sales & Employee Data Transformation using Power Query**

## 📌 Objective  
The objective of this project is to perform end-to-end data preparation (ETL) using Power BI Power Query, including:  

- Loading data from multiple Excel files  
- Cleaning and transforming raw data  
- Applying date, numeric, and text transformations  
- Merging datasets  
- Creating dynamic refresh using parameters  

> **Note:** No DAX or visualizations are used. This project strictly focuses on Power Query ETL operations.

## 📌 Data Sources  
### 1️⃣ Sales Data (Folder Source)  
- `Sales_Jan.xlsx`  
- `Sales_Feb.xlsx`  
- `Sales_Mar.xlsx`  
- Loaded using **Folder → Combine & Transform**

### 2️⃣ Employee Data  
- `Employee.xlsx`  
- Contains employee details such as Department, Region, Join Date, Birth Date.

## 📌 Key Transformations Performed  

### 🔹 Data Cleaning  
- Removed blank rows and columns  
- Promoted first row as headers  
- Renamed columns for standardization  
- Removed duplicates  
- Filtered null values  

### 🔹 Text Transformations  
- UPPER  
- TRIM  
- CLEAN  
- Replace special characters  
- Split columns (where applicable)  

### 🔹 Numeric Transformations  
- Renamed `TotalSale` → `Revenue`  
- Rounded Revenue to 2 decimals  
- Created **Profit** column:  
Profit = Revenue – Cost

text

### 🔹 Date & Time Transformations  
- From **Order Date**:  
- Year  
- Month Name  
- Quarter  
- Day  
- From **Birth Date**:  
- Calculated **Age** using error-safe formula  

### 🔹 Conditional Logic  
- Created **Sales Category** column:  
- Revenue ≥ 10000 → **High**  
- Revenue ≥ 5000 → **Medium**  
- Else → **Low**  

### 🔹 Indexing  
- Index column starting from 0  
- Index column starting from 1  

### 🔹 Pivot & Unpivot  
- Pivoted **Month** column using **Revenue**  
- Unpivoted to normalize data back  

### 🔹 Merge Operation  
- Merged **Sales** and **Employee** tables  
- Join Column: **Region**  
- Join Type: **Left Outer Join**  

### 🔹 Grouping & Aggregation  
- Grouped by **Region**:  
- Total Sales (Sum of Revenue)  
- Average Order Value (Average of Revenue)  
- Transaction Count (Count of Order ID)  

### 🔹 Data Profiling  
- Enabled:  
- Column Quality  
- Column Distribution  
- Column Profile  
- Used to identify missing values and errors  

### 🔹 Parameters & Dynamic Refresh  
- Created parameter: **SalesFolderPath**  
- Used parameter in folder source  
- Enabled automatic refresh when new files are added  

### 🔹 Refresh Simulation  
- Added `Sales_Apr.xlsx`  
- Clicked **Refresh**  
- Data loaded automatically  

## 📌 Tools & Technologies Used  
- Power BI Desktop  
- Power Query (M Language)  
- Microsoft Excel  

## 📌 Final Output  
- Cleaned and transformed dataset  
- Dynamic ETL pipeline  
- Saved as:  
- `DataLeverager.pbix`  

## 📌 Conclusion  
This project demonstrates practical data engineering and ETL skills using Power Query, including automation, transformation, and data quality analysis, aligned with real-world business requirements.
