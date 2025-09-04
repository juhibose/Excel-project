# Excel Project: Sales Analysis

## Description
This project demonstrates data cleaning, analysis, and visualization in Excel. It includes raw datasets, processed outputs, and dashboards to provide actionable insights.

---

## Folder Structure
- `data/` : Raw input files (Excel or CSV)
- `outputs/` : Cleaned datasets, pivot tables, charts, and dashboards
- `README.md` : Project description and usage instructions

---

## Excel Data Cleaning Checklist 🧹

1. **Handle Duplicates** ✅  
   * Go to Data → Remove Duplicates → Select all columns.  
   * Keep the first occurrence and delete the rest.

2. **Fix Date Formats** ✅  
   * Some dates are in `DD-MM-YYYY`, others in `YYYY/MM/DD`.  
   * Select the Order Date column → Use Text-to-Columns or `DATEVALUE()`.  
   * Convert all dates to `DD-MMM-YYYY` format for consistency.

3. **Standardize Text Columns** ✅  
   **Affected Columns:** Region, Product Category, Payment Method, Customer Name  
   **Steps:**  
   * `TRIM()` → Remove extra spaces  
   * `PROPER()` → Proper capitalization  
   * Correct typos manually:  
     - “Noth” → “North”  
     - “Soth” → “South”  
     - “Electrnics” → “Electronics”  
     - “Furnitur” → “Furniture”  
   * Standardize Payment Methods: “Credit Card”, “Cash”, “Online”

4. **Handle Missing & Incorrect Values** ✅  
   * Total Sales → Where empty, recalculate: `=Units Sold * Unit Price`  
   * Highlight rows with negative or zero values.

5. **Apply Data Validation (Optional)**  
   * Create dropdown lists for: Region, Product Category, Payment Method  
   * Helps prevent future inconsistencies.

6. **Final Check**  
   * Freeze top row for usability  
   * Apply a clean table format → Home → Format as Table  
   * Save as `Cleaned_Sales_Dataset.xlsx`

---

## Dashboard & Analysis Summary 📊

- Created pivot tables for:
  * Total Sales by Region, Product Category, and Sales Trend by Month and Year
  * Units Sold by Payment Method
- Added KPIs:
  * Total Sales  
  * Total Units Sold  
- Slicers added for interactive filtering  
- Dashboard configured to **Refresh All** to update with new data

---

## Usage
1. Open files in the `data/` folder to explore raw datasets.  
2. Open files in the `outputs/` folder to see cleaned data, pivot tables, and dashboards.  
3. Modify or add new data in the `data/` folder → Refresh dashboard in Excel to update results.  

---

## Project Status
✅ Completed – ready for exploration and further enhancements.
