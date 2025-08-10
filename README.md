# 🌡️ NOAA Temperature Analysis – Climate Data Visualization Project

## 📌 Overview
This notebook explores temperature trends near **Ann Arbor, Michigan, United States**, using historical climate data from NOAA's GHCN-Daily dataset. The analysis focuses on identifying record high and low temperatures from 2005–2014, detecting anomalies in 2015, and visualizing station locations.

The project demonstrates data preprocessing, visualization, and geospatial mapping techniques using Python.

---

## 📁 Dataset Description

- **temperature.csv**: Daily temperature records from NOAA stations.
- **BinSize.csv**: Supplementary file for binning or mapping purposes.

### Key Columns:
- `id`: Station identification code  
- `date`: Date in `YYYY-MM-DD` format  
- `element`: Temperature type (`TMAX`, `TMIN`)  
- `value`: Temperature value in tenths of degrees Celsius  

---

## 📊 Analysis Highlights

1. **Temperature Trends (2005–2014)**  
   - Line graph of record highs and lows  
   - Shaded area between TMAX and TMIN  

2. **Anomaly Detection (2015)**  
   - Scatter plot of days breaking historical records  

3. **Leap Day Handling**  
   - Removed February 29th for consistency  

4. **Visualization Enhancements**  
   - Clear legends, labels, and minimal chart clutter  

5. **Geospatial Mapping**  
   - Plotted station locations near Ann Arbor  

6. **Yearly Summary (2015)**  
   - Focused temperature overview for recent trends  

---

## 🛠️ Tools & Techniques

- **pandas**: Data manipulation  
- **matplotlib & seaborn**: Plotting  
- **folium / plotly** (optional): Interactive maps  
- `.copy()` used to avoid `SettingWithCopyWarning`  
- Aggregation via `groupby` and `strftime('%m-%d')`  

---

## 📓 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/manutomy14/notebook_share.git
   cd notebook_share
