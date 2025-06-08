# A/B Testing

This project involves hypothesis prioritization and A/B testing analysis for an online store. The goal was to identify which change would most effectively increase revenue, and to analyze user behavior based on experimental results.

## 📁 Project Structure
- `AB_testing.ipynb` — main analysis notebook
- `datasets/hypotheses_us.csv` — marketing hypotheses with impact estimates
- `datasets/orders_us.csv` — customer orders data
- `datasets/visits_us.csv` — daily website visit logs

## 🧠 Project Tasks

### Part 1: Hypothesis Prioritization

- Prioritized marketing hypotheses using **ICE** and **RICE** scoring frameworks
- Compared the rankings and explained the differences between the two approaches
- Selected **Hypothesis #7** ("Add a subscription form to all main pages") based on RICE as the most impactful for analysis

### Part 2: A/B Test Analysis

- Visualized:
  - Cumulative revenue by group
  - Cumulative average order value
  - Relative differences between groups
  - Daily conversion rates
- Identified outliers using the 95th and 99th percentiles for:
  - Orders per user
  - Order prices
- Filtered data to remove anomalies
- Calculated statistical significance for:
  - Conversion rate differences
  - Average order size differences
- Performed significance tests on both raw and filtered datasets

## 🛠️ Tools and Libraries

- Python
- pandas
- numpy
- matplotlib.pyplot
- seaborn
- scipy.stats

## ✅ Key Results

- **Group B** outperformed Group A in all major metrics: conversion rate, average order value, and total revenue.
- **Conversion rate in Group B was significantly higher**, even after removing anomalies.
- **Average order size difference** was not statistically significant after filtering out outliers.
- The test confirmed that **Hypothesis #7 was successful** — adding an email subscription form increased user conversion.

## 🧾 Final Decision

The test should be **stopped**, and **Group B** should be declared the winner. The new feature positively impacted conversion and should be implemented.
