# 🌌 AeroSense – Smart AQI Analytics with Python

📍 *Real-Time Air Quality Monitoring & Environmental Data Analytics*

<div align="center">


 ![AeroSense Banner](banner.png)
  
[![Python](https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python)]()
[![API](https://img.shields.io/badge/Data%20API-CPCB%20%7C%20WAQI-teal?style=for-the-badge&logo=apachespark)]()
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)]()
[![Data Science](https://img.shields.io/badge/Data-Science-blue?style=for-the-badge&logo=datascience)]()

</div>

---

## 🌟 Overview
AeroSense is a real-time environmental analytics system that:
- Fetches live AQI (Chandigarh)
- Visualizes pollutant breakdown (PM2.5/PM10/O3/NO2/SO2)
- Maps AQI station using GeoMapping
- COVID Lockdown trend analysis
- Automated pollutant insight extraction

🔗 Project Notebook:  
https://colab.research.google.com/github/RahulRaj2503/AIR-QUALITY-MONITORING/blob/main/AIR_POLLUTION_MONITORING_USING_PYTHON_.ipynb

---

## 🔥 Features
| Feature | Description |
|--------|-------------|
| 🌐 Real-Time AQI | Live API fetch |
| 📊 Pollutant Analytics | Pie chart & values |
| 🗺 City Mapping | Cartopy plots |
| 📈 Trend Visualization | PM2.5 during lockdown |
| 🧠 Insights | Min/Max/Average pollutant |

---

## 🛠 Tech Stack
- Python
- Pandas
- Matplotlib
- Cartopy
- WAQI API (CPCB Verified Data Source)

---

## 🚀 Installation & Setup

Run these commands in terminal:

git clone https://github.com/<username>/AeroSense.git  
cd AeroSense  
pip install -r requirements.txt  
jupyter notebook  

---

## 🔑 API Setup

Replace token value inside project:

api_key = "YOUR_WAQI_TOKEN"  
city = "Chandigarh"  
url = f"http://api.waqi.info/feed/{city}/?token={api_key}"

➡️ Get Token: https://aqicn.org/data-platform/token/#/

---

## 📌 Code Used (Plain Text Format)

1️⃣ Request AQI data  
response = requests.get(url).json()  
data = response["data"]  
aqi = data["aqi"]

2️⃣ Extract Pollutants  
pollutants = {k:v["v"] for k,v in data["iaqi"].items()}

3️⃣ Pie Chart  
Plot PM2.5, PM10, NO2, SO2, O3 % values

---

## 📸 Output Visualizations

📌 Add images when generated:

- Pie Chart → ./assets/pie_chart.png  
- Map → ./assets/map_plot.png  
- Trend Graph → ./assets/trend_plot.png  

Reference Output:  
https://colab.research.google.com/github/RahulRaj2503/AIR-QUALITY-MONITORING/blob/main/AIR_POLLUTION_MONITORING_USING_PYTHON_.ipynb

---

## 📊 Insights Summary (Fill later)

✔ Lowest PM2.5 day → PLACEHOLDER  
✔ Highest O₃ level → PLACEHOLDER  
✔ Avg SO₂ during lockdown → PLACEHOLDER  

---

## 📁 Folder Structure

AeroSense/  
 ├─ notebooks/  
 │   └─ AeroSense.ipynb  
 ├─ assets/ (place chart outputs here)  
 │   ├─ AeroSense_Banner.png  
 │   ├─ pie_chart.png  
 │   ├─ map_plot.png  
 │   └─ trend_plot.png  
 ├─ data/  
 │   └─ dataset.csv  
 ├─ README.md  
 └─ requirements.txt  

---

## 🔮 Future Enhancements
- ML-based AQI prediction
- Health risk severity labels
- Multi-city support
- Web dashboard

---

## ✍️ Author
👨‍💻 **Rahul Raj Singh | Python Developer**  
📍 Chandigarh, India  

Let’s collaborate on Data/AI & Sustainability 🌱

---

## ⭐ Support
If you like this project → Please ⭐ the repository!

<div align="center">

**AeroSense — Where Data Meets Clean Air 🌬️✨**

</div>
