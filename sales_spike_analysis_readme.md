# 📊 Sales Spike Analysis During Events

This project explores how major events and holidays impact weekly sales across U.S. states and product categories using a cleaned and balanced sales dataset.

## 🔍 Objectives

- Measure changes in sales around holidays and other events
- Compare sales trends across product categories and states
- Identify patterns that could inform promotional strategies

## 📁 Project Structure

```
├── data/                  # Not included - proprietary
├── notebooks/             # Jupyter notebooks with analysis
├── visuals/               # Plots and charts
├── scripts/               # Python scripts for data prep and analysis
├── README.md              # This file
└── requirements.txt       # Python dependencies
```

## 🧮 Data Summary

> **Note:** Raw data is proprietary (e.g., Circana/IRI via USDA ERS) and **not included** in this repository. For access, visit: [USDA ERS - Using Proprietary Data](https://www.ers.usda.gov/topics/food-markets-prices/food-prices-expenditures-and-establishments/using-proprietary-data)

- **Fields used**: `Date`, `State`, `Category`, `Variable`, `Value`
- **Event Windows**: Pre-Holiday, Holiday, Post-Holiday, Other
- **COVID Period Exclusion**: March–July 2020 is excluded from trend analysis

## 📈 Key Outputs

1. **Event Impact Table**: Percent change in average weekly sales per category by event window
2. **Line Graphs**: Weekly sales trends across categories and states (log scale)
3. **Z-Score & Percent Change Visualization**: Heatmaps and barplots showing relative change

## 🛠️ How to Run

```bash
pip install -r requirements.txt
jupyter notebook notebooks/sales_analysis.ipynb
```

## 🧠 Insights & Suggestions

- Some categories (e.g., Alcohol, Prepared Items) spike during holiday periods
- Commercially prepared items showed less variation than expected
- Different states exhibit varied holiday patterns

## 🚀 Future Steps

- **Product-level insights**: If available, analyze UPC-level data to spot specific product drivers
- **Promotion modeling**: Link price drops or ad campaigns to volume spikes
- **Demographic segmentation**: If household panel data is accessible, explore trends by age, income
- **Nutritional profiling**: Assess whether spikes align with healthy or unhealthy food choices

## 📜 Disclaimer

This repository includes only **aggregated and anonymized results**. The raw data used is proprietary and protected under license agreements. Please contact USDA ERS or Circana/IRI for access.

---

For any questions or suggestions, feel free to open an issue or submit a pull request.

