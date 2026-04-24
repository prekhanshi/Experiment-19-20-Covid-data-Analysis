# Experiment-19-20-Covid-data-Analysis
# Name : Prekhanshi Kumbhakar
# PRN: 25070123151
# Branch: F.Y. E&TC (2025–29)
# Batch: A1
# Subject: Exploratory Data Analysis with Python


## 📌 Overview  
This experiment focuses on analyzing global COVID-19 data using Python and the Pandas library in Google Colab. The dataset contains records of confirmed, recovered, and death cases across different countries and states over time.

---

## 🎯 Objectives  
- Perform data cleaning and preprocessing  
- Analyze COVID-19 trends globally and for India  
- Calculate active cases  
- Identify most affected countries and states  
- Visualize data using maps  

---

## 🗂️ Dataset Description  

The dataset includes the following columns:

- SNo – Serial number  
- ObservationDate – Date of record  
- Province/State – State or region  
- Country/Region – Country name  
- Last Update – Last updated timestamp  
- Confirmed – Total confirmed cases  
- Deaths – Total deaths  
-# 🦠 Experiment 19 & 20: COVID-19 Data Analysis Using Pandas

## 📌 Overview  
This experiment focuses on analyzing global COVID-19 data using Python and the Pandas library in Google Colab. The dataset contains records of confirmed, recovered, and death cases across different countries and states over time.

---

## 🎯 Objectives  
- Perform data cleaning and preprocessing  
- Analyze COVID-19 trends globally and for India  
- Calculate active cases  
- Identify most affected countries and states  
- Visualize data using maps  

---

## 🗂️ Dataset Description  

The dataset includes the following columns:

- SNo – Serial number  
- ObservationDate – Date of record  
- Province/State – State or region  
- Country/Region – Country name  
- Last Update – Last updated timestamp  
- Confirmed – Total confirmed cases  
- Deaths – Total deaths  
- Recovered – Total recovered cases  

---

## 🛠️ Tools & Technologies  

- Python  
- Google Colab  
- Pandas  
- NumPy  
- Plotly  

---

## 🚀 Steps Performed  

### 1. Data Loading  
- Imported dataset using `pd.read_csv()`  
- Displayed initial records using `.head()`

### 2. Data Cleaning  
- Dropped unnecessary columns (`SNo`, `Last Update`)  
- Converted data types:
  - `ObservationDate` → datetime  
  - `Confirmed`, `Deaths`, `Recovered` → integer  

### 3. Feature Engineering  
- Created a new column for Active Cases:

```python
data['Active'] = data['Confirmed'] - data['Deaths'] - data['Recovered']
### 4. Data Exploration
Checked dataset structure using .info()
Identified the latest date in the dataset
Filtered data for the most recent records
### 5. Global Analysis
Grouped data by country
Calculated total confirmed, deaths, recovered, and active cases
Identified top affected countries:
US
India
Brazil
France
Turkey
### 6. Visualization
Created a world choropleth map using Plotly
### 7. India-Specific Analysis
Filtered dataset for India
Found total number of states/UTs
Listed all states
### 8. Data Cleaning (India States)
Replaced 'Unknown' values with NaN
Filled missing values using mode
### 9. Latest India Data Analysis
Extracted latest COVID data for India
Compared cases across states
### 10. Top Affected States in India
Maharashtra (highest cases)
Karnataka
Kerala
Tamil Nadu
Uttar Pradesh
### 📊 Key Results
Total Countries Analyzed: 195
Most Affected Country: US
Second Most Affected: India
Most Affected State in India: Maharashtra
Total Indian States/UTs: 38
### 📚 Conclusion

This experiment demonstrates how pandemic data can be analyzed using Pandas. It helps in understanding global and national trends of COVID-19 and builds foundational data analysis skills.
