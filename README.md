# 🛡 Insurance Claims & Policyholder Risk Analysis Dashboard  

![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)  
End-to-end **data analytics solution** designed to identify high-risk policyholders, track claims trends, and analyze policy adjustments using **synthetic insurance data**.  
Highlights the power of **Python for data generation** and **Power BI for interactive dashboards**.

### Dashboard Preview  
![Insurance Dashboard](https://github.com/srishtisharma44/Insurance-Claims-Risk-Analysis/blob/main/Dashboard.png)  

---

## Project Overview  
This project provides an end-to-end data analysis solution simulating insurance claims and policyholder behavior.  
It demonstrates a data-driven approach to understanding **risk patterns, claim severity, and policy adjustments** for better decision-making in the insurance sector.

By building a synthetic dataset from scratch, the project models and visualizes key insights on an interactive Power BI dashboard.  
Emphasizes skills in Python-based data generation, data cleaning, DAX calculations, and professional dashboard design in Power BI.

---

## Project Pipeline  
A structured progression from synthetic dataset creation to an interactive, decision-ready Power BI dashboard.

---

## Step-by-Step Process  

### 1. Data Generation  
- **Data Source**: Synthetic dataset created using Python and Pandas.  
- **Details**: ~10,000 policyholders with attributes including Age, Region, Policy Type, Claims Severity, Premium Amount, and Marital Status.  
- **Modeling**: Data simulated to reflect realistic policyholder behavior, claim severity distribution, and adjustment trends.  
- **Storage**: CSV file (`insurance_claims_synthetic_data.csv`).

### 2. Data Cleaning & Preparation  
- Ensured consistency across all fields.  
- Standardized categorical fields (Policy Type, Region, Marital Status).  
- Verified numerical fields (Claims Frequency, Premium Amount, Claims Adjustment).  
- Assigned severity levels: Low, Medium, High.

### 3. Power BI Modeling  
- Created relationships between demographics and claims behavior.  
- Designed DAX measures for **Total Claims**, **Average Claims**, **Claims Adjustment Impact**, and **Average Claim Amount**.  

### 4. Dashboard Design  
- Clean layout integrating KPI cards, charts, and slicers.  
- Used pie charts, bar charts, and tables for visual insights.  
- Applied consistent formatting, data labels, and conditional formatting.  

### 5. Interactive Elements (Slicers)  
- Added slicers for Age, Region, Policy Type, and Marital Status.  
- Enabled dynamic filtering and drill-down analysis by users.  

### 6. Final Dashboard  
- Delivered an interactive, professional-quality Power BI dashboard presenting high-level KPIs and detailed insights.

---

## Interactive Preview & Dataset  

### Project Demo Video  
[Click here to watch the Dashboard Demo](https://github.com/srishtisharma44/Insurance-Claims-Risk-Analysis/blob/main/Demo.gif)  

### Dataset Used  
- [Synthetic Insurance Dataset](https://github.com/srishtisharma44/Insurance-Claims-Risk-Analysis/blob/main/insurance_claims_synthetic_data.csv)  
- Dataset also available on Kaggle: [Insurance Data – Personal Auto Line of Business](https://www.kaggle.com/datasets/samialyasin/insurance-data-personal-auto-line-of-business/data)

---

## Tools Used  
- ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white) Python – Data generation and simulation.  
- ![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white) Pandas – Data manipulation and structuring.  
- ![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black) Power BI – Data modeling, DAX, and interactive dashboards.

---

## Results and Insights  
- **Risk Segmentation**: Identified groups with high claim frequency and severity.  
- **Policy Insights**: Premium policies had higher adjustment impact compared to regular ones.  
- **Demographic Trends**: Younger policyholders showed lower severity, while middle-aged groups had higher frequency.  
- **Actionable Insights**: Helped insurance firms adjust pricing models and policy structures.

---

## Future Enhancements  
- Automate Power BI refresh with live insurance data.  
- Add predictive modeling for fraud detection and risk scoring.  
- Extend KPIs to include Customer Lifetime Value (CLV) and Loss Ratio.  
- Migrate dataset storage to SQL database for scalability.  

---

## License  
This project is licensed under the MIT License.

---

## Acknowledgments  
- Python & Power BI Community – For tutorials and support.  
- [Kaggle Insurance Dataset](https://www.kaggle.com/datasets/samialyasin/insurance-data-personal-auto-line-of-business/data) – Inspiration for data modeling.

---

## Key Performance Indicators (KPIs)  
- **Total Claims** – Total number of claims made.  
- **Average Claims per Policyholder** – Trends across different policyholders.  
- **Claim Severity Distribution** – Low / Medium / High.  
- **Claims Adjustment Impact** – Effect of adjustments on claims.  
- **Average Claim Amount (DAX):**  

```DAX
Average Claim Amount =
DIVIDE(
    SUM('synthetic_insurance_data'[Claims_Adjustment]),
    SUM('synthetic_insurance_data'[Claims_Frequency]),


    0
)
