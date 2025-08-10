# 🌡️ NOAA Temperature Analysis – Machine Test Submission

## 📌 Overview
This notebook presents an analysis of temperature data near **Ann Arbor, Michigan, United States**, using NOAA's GHCN-Daily dataset. The goal is to visualize record high and low temperatures from 2005–2014, highlight anomalies in 2015, and map station locations.

This submission is part of the **Data Science Intern Machine Test** for **Tranzmeo IT Solutions Pvt. Ltd.**

---

## 📁 Dataset Description

- **temperature.csv**: Contains daily temperature records from NOAA stations.
- **BinSize.csv**: Supplementary file for binning or mapping purposes.

### Columns in `temperature.csv`:
- `id`: Station identification code  
- `date`: Date in `YYYY-MM-DD` format  
- `element`: Type of temperature measurement (`TMAX`, `TMIN`)  
- `value`: Temperature value in tenths of degrees Celsius  

---

## 🧪 Tasks Completed

1. **Visualized record high and low temperatures (2005–2014)**  
   - Line graph with shaded area between TMAX and TMIN  
2. **Overlayed 2015 anomalies**  
   - Scatter plot for days where 2015 broke previous records  
3. **Leap day handling**  
   - Removed February 29th to ensure consistent comparison  
4. **Enhanced plot readability**  
   - Added legends, labels, and removed chart junk  
5. **Mapped station locations near Ann Arbor**  
   - Used latitude/longitude data for visualization  
6. **Plotted 2015 temperature summary**  
   - Focused analysis on recent year trends  

---

## 🛠️ Implementation Notes

- Used **pandas** for data manipulation  
- Used **matplotlib** and **seaborn** for visualization  
- Removed leap day using logical filtering  
- Applied `.copy()` to avoid `SettingWithCopyWarning`  
- Used `groupby` and `strftime('%m-%d')` for day-wise aggregation  
- Optional: Used `folium` or `plotly` for interactive maps (if applicable)

---

## 📓 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/manutomy14/notebook_share.git
   cd notebook_share
