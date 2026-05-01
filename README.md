# Carbon-Emissions-calculator
Interactive Python tool for corporate carbon accounting following GHG Protocol standards.
# 🌍 Corporate Carbon Footprint Tool (Scope 1 & 2)


## Project Overview
As an entry-level Sustainability Analyst, I developed this interactive Python tool to help small-to-medium enterprises (SMEs) begin their carbon accounting journey. The tool calculates direct and indirect emissions in alignment with the **GHG Protocol Corporate Standard**.

## 🛠️ Methodology & Logic
The tool utilizes the fundamental carbon accounting equation:
**Activity Data × Emission Factor = CO2e Emissions**

### 1. Scope 1: Direct Emissions
* **Stationary Combustion:** Calculates emissions from natural gas usage. 
* **Mobile Combustion:** Analyzes fleet fuel consumption (Diesel).
* **Fugitive Emissions:** Calculates the impact of refrigerant leaks. 
    * *Logic:* I applied **Global Warming Potential (GWP)** values for R410A. This ensures the tool accounts for the fact that refrigerants are significantly more potent than CO2.

### 2. Scope 2: Indirect Energy (Dual Reporting)
Following the GHG Protocol Scope 2 Guidance, this tool provides **Dual Reporting**:
* **Location-based:** Uses the regional grid average emission factor (Defaulted to India/CEA factors).
* **Market-based:** Accounts for contractual instruments (Renewable Energy Certificates). If a company uses 100% renewable energy, the market-based total will reflect 0 tCO2e, demonstrating the impact of procurement choices.

## 📊 Technical Stack
* **Python:** Core calculation logic.
* **Pandas:** Data structuring and table generation.
* **Matplotlib/Seaborn:** Data visualization for stakeholder reporting.
* **Google Colab:** Deployment environment.

## 📈 Sample Output
The tool generates a breakdown by category and a visualization of the emission "hotspots," allowing analysts to prioritize decarbonization strategies (e.g., transitioning to EVs if Mobile emissions are >40%).

---
*Disclaimer: This tool is for educational and screening purposes. Official reporting should use verified, year-specific emission factor databases.*
