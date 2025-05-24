# Energy Consumption Forecasting & Anomaly Detection

![Energy Image](https://cdn-icons-png.flaticon.com/512/1642/1642708.png)

## 📌 Overview
Time series modeling project to forecast household electricity consumption and detect anomalous usage days. Developed multiple forecasting models, visualized patterns, and deployed an interactive Tableau dashboard for insights.

## 📂 Dataset Information

### Source
- **Dataset**: [UCI Machine Learning Repository - Household Power Consumption Dataset](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)

### Key Details
- **Granularity**: Minute-level readings aggregated to daily  
- **Instances**: 1,441 days (Dec 2006 – Nov 2010)
- **Attributes**:
  - `Date`
  - `Global_active_power` (kW, minute-averaged)
  - `Voltage`
  - `Sub-metering` values

## 📦 Project Structure

energy-forecasting/
├── data/                   # Raw & processed data  
├── img/                    # Visualizations and plots  
├── report/                 # Final reports (PDF, HTML, Markdown)  
├── notebooks/              # Jupyter notebooks  
├── models/                 # Serialized models (if any)  
├── requirements.txt        # Dependencies  
└── README.md               # Project overview  

## 📊 Performance Metrics

### Forecasting Goal
Predict daily household electricity consumption and identify days with abnormal consumption patterns.

### Model Comparison

| Model | MAE | MAPE | MSE | RMSE | Use Case |
|-------|-----|------|-----|------|----------|
| **SARIMAX** | 22.13 | 6.11e13 | 555.24 | 23.56 | Benchmark seasonal model |
| **Prophet** | 8.41 | 1.83e15 | 107.37 | 10.36 | Preferred for production |

#### SARIMAX Model
**Traditional Seasonal Model**  
- Captured strong seasonality patterns  
- Reliable baseline forecasting

#### Prophet Model  
**Auto-detects Trends & Seasonality**  
- Better accuracy, faster tuning  
- Ideal for operational energy forecasting

## 🚀 Installation & Usage

### Prerequisites
- Python 3.8+
- Jupyter Notebook/Lab
- Tableau Public (for dashboard)

### Quick Start
```bash
git clone https://github.com/yourusername/energy-forecasting-anomaly-detection.git
cd energy-forecasting-anomaly-detection
pip install -r requirements.txt
jupyter notebook
```

## 📜 License
MIT License https://choosealicense.com/licenses/mit/


## 🧚🏼‍♂️ Donation --> Way to heaven
If you appreciate this project and want to support future work, consider buying me [☕](https://buymeacoffee.com/prasadpandp)... (or better, donating a [GPU](https://www.amazon.in/gp/cart/view.html?ref_=nav_cart) 😆).
