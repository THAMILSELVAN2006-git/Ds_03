# Food Delivery Delay Analysis (DS_03)

Empirical data science and operations analysis investigating the operational and environmental drivers of delivery lateness in on-demand food fulfillment platforms.

---

## 📌 Project Overview

Customer retention and platform profitability in on-demand delivery depend heavily on reliable, predictable fulfillment times. This study conducts a rigorous statistical and machine learning investigation using empirical data from `Food_Delivery_Times.csv` (1,000 completed orders). 

Key areas of investigation:
- **Physical Logistics vs. Friction**: Decomposing delivery time variance across transit distance, preparation time, traffic congestion, and adverse weather.
- **Statistical Delay Profiling**: Modeling operational delay thresholds and identifying delay factors.
- **Predictive Modeling**: Evaluating Linear Regression and Random Forest ensembles with cross-validation to estimate fulfillment times and guide SLA management.

---

## 📁 Repository Structure

```text
├── DS_Day01_03_Food_Delivery_Delays.ipynb   # Main interactive notebook with end-to-end analysis & visualizations
├── Food_Delivery_Times.csv                 # Dataset containing 1,000 delivery records
├── .gitignore                              # Git ignore rules for Python/Jupyter cache
└── README.md                               # Project documentation
```

---

## 📊 Dataset Schema

| Field | Description | Type |
| :--- | :--- | :--- |
| `Order_ID` | Tracking identifier (1 to 1000) | Integer |
| `Distance_km` | Travel distance between merchant and customer | Float |
| `Preparation_Time_min` | Kitchen order prep time | Float |
| `Courier_Experience_yrs` | Courier tenure / experience | Float |
| `Weather` | Weather condition (`Clear`, `Rainy`, `Foggy`, `Snowy`, `Windy`) | Categorical |
| `Traffic_Level` | Congestion level (`Low`, `Medium`, `High`) | Categorical |
| `Time_of_Day` | Order period (`Morning`, `Afternoon`, `Evening`, `Night`) | Categorical |
| `Vehicle_Type` | Courier transport (`Bike`, `Scooter`, `Car`) | Categorical |
| `Delivery_Time_min` | Total elapsed delivery time (target) | Float |

---

## 🚀 Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook / JupyterLab / Google Colab

### Installation
Clone the repository:
```bash
git clone https://github.com/THAMILSELVAN2006-git/Ds_03.git
cd Ds_03
```

Install dependencies:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

Run the notebook:
```bash
jupyter notebook DS_Day01_03_Food_Delivery_Delays.ipynb
```
