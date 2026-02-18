# 🏏 Cricket Analytics Dashboard: India vs South Africa 

## 📌 Project Overview
This project demonstrates an end-to-end data visualization workflow, transforming raw web data into an interactive performance dashboard. I focused on the historical batting data of the India vs. South Africa series, extracted directly from **ESPN Statsguru**.

The dashboard is designed to be a "beginner-friendly" template, showing how to achieve complex data scraping and professional UI design using only Power BI's native features.

## 🚀 Key Features
* **No-Code Web Scraping:** Leveraged the Power BI Web Connector to pull live HTML tables from ESPN.
* **Dynamic Player KPI Cards:** Interactive visuals that update based on player selection (Runs, Average, Strike Rate, etc.).
* **Boundary Analysis:** Detailed tracking of 4s, 6s, and milestone scores (Centuries/Half-Centuries).
* **Clean UI/UX:** A structured layout with a custom color palette and visual hierarchy for easy data consumption.

## 🛠️ Data Lifecycle (ETL Process)

### 1. Data Extraction
Instead of using Python, I utilized the **"Get Data > Web"** feature in Power BI. This involved:
* Connecting to ESPN Statsguru URL.
* Using "Add Table Using Examples" to identify the correct batting/bowling structures.

### 2. Transformation (Power Query)
Data cleaning was performed to ensure accuracy:
* **Data Type Correction:** Converted text-based stats into numeric values for calculations.
* **Cleaning Special Characters:** Handled the `*` symbol in the "Highest Score" and "Not Out" columns.
* **Span Splitting:** Separated career start and end years to enable timeline analysis.

### 3. Visualization
* **Slicers:** Added for player-specific deep dives.
* **Measures:** Created DAX measures for core metrics like Batting Average and Strike Rate to ensure dynamic updates.

## 📂 Repository Structure
* `Cricket_Analysis.pbix`: The main Power BI file.
* `Screenshots/`: Images of the Batting, Bowling, and Fielding sheets.
  
## 📈 Future Roadmap
* [ ] Complete the **Bowling Analysis** sheet.
* [ ] Complete the **Fielding Analysis** sheet.
* [ ] Add a "Player Comparison" view to compare stats side-by-side.

---
