# EDA-Rollercoaster

An exploratory data analysis (EDA) of a rollercoaster dataset, looking at what
characterises the fastest and most consistent coasters.

## Project Question
**What characterises the fastest rollercoasters?**

## Key Findings
- After cleaning, the dataset covers 990 unique rollercoasters. Duplicates were
  removed using coaster name, location, and opening date as the key.
- Most coasters were introduced around **1999–2000**, a building boom at the turn
  of the millennium.
- **Speed and height are strongly correlated (r = 0.71)** — taller coasters tend
  to be faster, which makes physical sense, since height provides the potential
  energy to reach high speeds.
- **Busch Gardens Williamsburg** has both the highest average speed (58.3 mph)
  and the most consistent speeds (coefficient of variation 0.24).
- **Cedar Point** is second on average speed (57.8 mph) but has a high spread,
  dropping it to 7th on consistency — a fast park with a wide mix of coasters.

**Conclusion:** A fast rollercoaster is, above all, a tall one. Most coasters in
the data were built around 1999–2000, and the fastest parks cluster tightly at
the top, with Busch Gardens Williamsburg standing out as both fastest and most
consistent.

*Note: all relationships are correlational and describe patterns in the dataset,
not guaranteed causes.*

## Tools
Python, pandas, NumPy, Matplotlib, Seaborn (in Google Colab). Data loaded via the
Kaggle API (`kagglehub`).

## Dataset
Rollercoaster database with coaster specifications (speed, height, type, location,
opening date, and more).
Source: [Rollercoaster Database on Kaggle](https://www.kaggle.com/datasets/robikscube/rollercoaster-database)

## Running the notebook
This notebook loads data through the Kaggle API. To run it yourself, add your own
Kaggle token in Colab (Secrets → `KAGGLE_API_TOKEN`), or download the dataset from
the Kaggle link above.

## Credit
Dataset by Robik Shrestha (robikscube), via Kaggle.
