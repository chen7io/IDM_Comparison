# IDM_Comparison
Power BI Dashboard: Semiconductor IDM Comparison (TI / ADI / NXP) An interactive Power BI dashboard built with official SEC 10-K filings (2020–2024) to compare Texas Instruments, Analog Devices, and NXP.
利用官方 SEC 10-K 財報 (2020–2024) 建立的 Power BI 互動式儀表板，對比 Texas Instruments、Analog Devices、NXP 三大半導體廠商的營收、每股盈餘（EPS）、研發費用及區域/產品線分布。

專案特色：

自動化清理與整合 SEC 原始財報資料，確保數據一致性與準確性。

建立多維度視覺化（年度成長率、區域營收占比、產品組合分析），協助快速洞察各公司策略差異。

儀表板具備互動功能，可依年份、公司、業務區域篩選，提升決策支援效率。

目的：展現以資料分析工具（Power BI、DAX、Power Query）處理大型財報數據的能力，並以視覺化方式呈現產業競爭力比較，支持商業決策。

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
![Dashboard Screenshot](https://github.com/chen7io/IDM_Comparison/blob/main/IDM_Comparison_Image.png)

## 📥 How to View This Project  

There are two ways to explore the dashboard:  

1. **Download the file**  
   - The Power BI file (`IDM Comparison.pbix`) is available in this repository.  
   - You can download it and open it with **Power BI Desktop** for full interactivity.  

2. **Preview the visuals**  
   - If you don’t have Power BI installed, you can still check the **preview images** included in the repo (e.g., `IDM_Image.png`).  
   - These screenshots provide a quick overview of the dashboard design and insights.  

## 📑 Data Source
- [TI 10-K](https://investor.ti.com/financial-information/sec-filings)
- [ADI 10-K](https://investor.analog.com/financial-information/sec-filings)
- [NXP 10-K](https://investors.nxp.com/financials/sec-filings)

## 🛠 Tools
- Power BI
- Python
- DAX (calculated measures)
- Data modeling & visualization
