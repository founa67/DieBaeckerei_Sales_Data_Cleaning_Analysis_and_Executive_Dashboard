# Starke Bäcker Data Wrangling & Cleaning

## 📌 Project Overview
This project demonstrates a **systematic data cleaning and transformation workflow** using Microsoft Excel and Power Query.  
The dataset represents annual sales records for *Starke Bäcker*, a bakery chain.  
The primary goal was to create a curated, high-quality **FactSales table** that is analytics-ready, consistent, and validated for business reporting.

---

## 🔧 Tools & Techniques
- Microsoft Excel  
- Power Query (ETL / Data Wrangling)  
- Data Quality Validation  

---

## 🧹 Data Cleaning & Transformation  
Key steps applied to the raw dataset:
- Fixed encoding issues (e.g., `Knusperbrötchen` characters).  
- Standardized text fields (Branches, Products).  
- Assigned correct **data types**.  
- Removed **duplicates** based on (Branch, Product, Date).  
- Validated **Profit = Revenue – Cost**.  
- Ensured no negative values for Units Sold, Revenue, and Cost.  
- Derived new attributes: Unit Price, Unit Cost, Margin %, Year, Month, Quarter.  
- Filtered records outside the reporting window.  

---

## 📊 Data Schema  
The curated dataset includes:  
- **Branch** – Store location  
- **Product** – Product/SKU name  
- **Units Sold** – Quantity sold  
- **Revenue** – Gross sales revenue  
- **Cost** – Cost of goods sold  
- **Profit** – Revenue – Cost  
- **Date** – Transaction date  
- **Derived Fields** – Unit Price, Unit Cost, Margin %, Year, Month, Quarter  

---

## 📝 Transformation Log  
Each step was logged in Power Query to ensure transparency and reproducibility.  
Examples:  
- `Table.PromoteHeaders` → Make column names explicit  
- `Text.Trim`, `Text.Clean` → Clean text fields  
- `Table.Distinct` → Remove duplicates  
- `Table.AddColumn` → Add ProfitCheck, Unit Price, Margin %  
- `Date.*` → Extract calendar attributes  

---

## 💡 Business Impact  
- Improved **data governance** and data quality.  
- Delivered a **curated FactSales table** ready for pivot-based reporting.  
- Enabled accurate calculation of KPIs such as Profit Margin and Cost Margin.  
- Provided a repeatable, transparent **ETL process** suitable for analytics portfolios.  

---

## 📂 Files in Repository  
- `Starke_Bäcker_Documentation.docx` → Full technical documentation  
- `FactSales_Cleaned.xlsx` → Final curated dataset (for reporting)  

---

## 🚀 Conclusion  
This project showcases strong **data wrangling and cleaning skills** in Excel and Power Query.  
The structured FactSales dataset supports accurate analytics, governance, and performance monitoring.
