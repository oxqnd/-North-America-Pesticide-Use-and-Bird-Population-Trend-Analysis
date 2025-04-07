# -North-America-Pesticide-Use-and-Bird-Population-Trend-Analysis
This repository contains data and preprocessing scripts for analyzing the relationship between pesticide usage and bird population changes in North America.

---

## 📊 Project Overview

The goal of this project is to examine how pesticide usage in North America (United States, Canada, and Mexico) correlates with changes in bird population indices between 1990 and 2020.



---

## 📂 Data Description

### Raw Data

- **`Inputs_Pesticides_Use_E_All_Data.csv`**
  - Source: FAOSTAT (https://www.fao.org/faostat)
  - Contains global pesticide usage by type, country, and year.

- **`LPD_2024_public.csv`**
  - Source: Living Planet Index Database (https://livingplanetindex.org)
  - Includes abundance trends of vertebrate species worldwide.

### Processed Data

- **`north_america_pesticide_use.csv`**
  - Annual pesticide usage in North America (sum of USA, Canada, and Mexico) from 1990 to 2020, by pesticide category.

- **`bird_population_by_year.csv`**
  - Average annual bird population index across species native to North America, extracted from LPD data.

---

## 🛠 Preprocessing Steps

1. **Filter**: Selected North American countries (USA, Canada, Mexico)
2. **Pivot**: Transformed pesticide data into year-wise, category-specific format
3. **Bird Index Extraction**: Averaged per-year bird indices from native species
4. **Merge**: Aligned pesticide use and bird index by year

All steps are documented in the notebook [`01_data_preprocessing.ipynb`](notebooks/01_data_preprocessing.ipynb).

---

## 📜 License

This project uses datasets from open sources. Please cite original data providers if you reuse the data.

---
