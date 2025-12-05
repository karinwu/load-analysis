# ⚡ Representative Load Shape

This repository contains code and tools for analyzing electricity load curves and generating representative load shapes.

---

## 🧭 Overview

The **Load Shape Library** is designed to model and represent electricity consumption across an entire year (8,760 hours).  
It includes methods to compute centroids of time-series data using techniques such as:

- 📈 **Euclidean Barycentre**  
- 🔁 **Dynamic Time Warping (DTW)**  
- 🧮 **Soft Dynamic Time Warping (Soft-DTW)**  

These algorithms are applied to derive representative load centroids and create a comprehensive load shape library.

As suggested by [Luo et al. (2017)](https://www.sciencedirect.com/science/article/abs/pii/S0306261917309819), electricity load shapes are influenced by **seasonal** and **weekly usage patterns**.  

The dataset is divided into four seasons:

- ❄️ **Winter:** December, January, February  
- 🌸 **Spring:** March, April, May  
- ☀️ **Summer:** June, July, August  
- 🍂 **Fall:** September, October, November  

Each season is further separated into **weekdays** and **weekends** to capture distinct consumption behaviors.

The library also provides a **scaling feature** ⚙️ that allows users to normalize load profiles to a user-defined peak load.  
Users can apply either a *winter peak kW scaler* ❄️ or a *summer peak kW scaler* ☀️ for customized analysis.

---

## 📊 Data Sources

This project uses the **PJM Hourly Energy Consumption** dataset from *PJM Interconnection LLC (PJM)* — a regional transmission organization (RTO) operating in parts of:

> 🗺️ Delaware, Illinois, Indiana, Kentucky, Maryland, Michigan, New Jersey, North Carolina, Ohio, Pennsylvania, Tennessee, Virginia, West Virginia, and the District of Columbia.

The dataset can be downloaded from Kaggle:  
📥 [**PJM Hourly Energy Consumption Data**](https://www.kaggle.com/datasets/robikscube/hourly-energy-consumption?resource=download&select=COMED_hourly.csv)

---

## 📚 References

Luo, X., Hong, T., & Fang, S. (2017). *Benchmarking time series load forecasting models: Empirical evidence for diversity and accuracy.*  
[Applied Energy, 205, 118–133.](https://www.sciencedirect.com/science/article/abs/pii/S0306261917309819)


****
