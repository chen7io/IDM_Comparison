# IDM_Comparison
Power BI Dashboard: Semiconductor IDM Comparison (TI / ADI / NXP) An interactive Power BI dashboard built with official SEC 10-K filings (2020–2024) to compare Texas Instruments, Analog Devices, and NXP.

# 📊 Semiconductor IDM Comparison Dashboard

Interactive Power BI Dashboard comparing **Texas Instruments (TI)**, **Analog Devices (ADI)**, and **NXP**  
using official **SEC 10-K filings (2020–2024)**.

## 🐍 Data Collection  
All financial data was programmatically collected using **Python** from the official **SEC EDGAR database**.  

- The SEC EDGAR filings are stored in **XBRL (eXtensible Business Reporting Language)** format, which is deeply nested and challenging to parse.  
- Built a custom ETL pipeline in Python to automatically fetch and extract data points (Revenue, EPS, and R&D) from **10-K filings (2020–2024)**.  
- Key libraries used:  
  - `sec-api` → query SEC filings  
  - `lxml` → parse nested XBRL structures  
  - `pandas` → clean and transform extracted data  
- This process ensures **accuracy, reproducibility, and scalability**, while demonstrating the ability to work with **complex, unstructured financial datasets**.
  
## 🔎 Features
- Revenue, EPS, and R&D trend analysis
- Segmentation by region and industry
- Harmonize color palette to improve cross-company comparisons
- Note: NXP changed regional segmentation in 2020, hence excluded from region chart

## 📂 Preview
![Dashboard Screenshot](https://github.com/chen7io/IDM_Comparison/blob/main/IDM_Image.png)

## 📑 Data Source
- [TI 10-K](https://investor.ti.com/financial-information/sec-filings)
- [ADI 10-K](https://investor.analog.com/financial-information/sec-filings)
- [NXP 10-K](https://investors.nxp.com/financials/sec-filings)

## 🛠 Tools
- Power BI
- DAX (calculated measures)
- Data modeling & visualization
