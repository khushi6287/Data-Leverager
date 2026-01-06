
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
