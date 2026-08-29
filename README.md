# 🚗 Car Market Trends Analysis

A data analytics project exploring vehicle pricing, depreciation, and market trends using CarDekho marketplace data.

## What's This About?

This project analyzes **300+ vehicles** from the CarDekho marketplace to uncover insights about:
- How vehicle prices vary over time
- How much cars depreciate
- The differences between cars and two-wheelers (bikes/scooters)
- Which vehicles are most popular and expensive

## 📊 The Data

We're working with a dataset of **301 vehicles** that contains:
- Vehicle names and manufacturing years
- Original price (when new)
- Current selling price on the marketplace
- Owner count, fuel type, transmission type, and more

**Fun discovery:** The dataset actually contains TWO types of vehicles hidden in the `Car_Name` column:
- 🚗 **Cars** (written as lowercase, like `ritz`, `city`, `fortuner`)
- 🏍️ **Two-wheelers** (bikes and scooters, written in Title Case like `Honda Activa 4G`, `Royal Enfield Classic 350`)

We engineered a special `Vehicle_Type` column to separate them so we can analyze each group!

## 🔍 What We Found

The analysis answers **25 key questions**, including:

**Basic Stats (Q1-Q14):**
- Year range of vehicles in the dataset
- Lowest and highest selling prices
- Missing data checks
- Top brands and models

**Car vs Two-Wheeler Analysis (Q15-Q25):**
- Price differences between cars and bikes
- Depreciation patterns for each vehicle type
- Most expensive and cheapest vehicles by category
- And more!

## 🚀 How to Use

1. **Open the notebook:** `Car_Market_Trends_Analysis.ipynb`
2. **Run all cells** to see the analysis and visualizations
3. **The data file** (`Car_Market_Trends_Analysis_with_Car_Dekho_Data.csv`) is automatically loaded in the notebook

### Requirements

You'll need Python 3.x with these libraries:
- `pandas` - for data analysis
- `numpy` - for numerical operations
- `matplotlib` - for charts and visualizations

## 📝 Project Structure

```
├── README.md                                          # This file
├── Car_Market_Trends_Analysis.ipynb                   # Main analysis notebook
└── Car_Market_Trends_Analysis_with_Car_Dekho_Data.csv # Dataset (301 records)
```

## 💡 Key Insights

- The dataset spans multiple manufacturing years with a wide range of prices
- Depreciation varies significantly between vehicle types
- Two-wheelers and cars show very different pricing patterns
- The naming pattern of vehicles reveals which category they belong to

## 🔧 How It Works

The notebook:
1. **Cleans the data** - removes duplicates and handles missing values
2. **Engineers new features** - creates Vehicle_Type, Age, and Depreciation columns
3. **Analyzes** - answers each of the 25 questions with code and insights
4. **Visualizes** - shows trends with charts and summaries

## 📌 Notes

- All prices are in **lakhs** (Indian currency, 1 lakh = 100,000 rupees)
- The dataset appears to have been collected around 2018-2020 based on the newest vehicles
- Some questions specifically compare cars vs two-wheelers, so that feature engineering step is crucial

---

**Happy analyzing!** 🎯
