# OTC Sales Forecasting with Random Forest

This repository contains a time series forecasting project using Random Forest Regressors to predict weekly over-the-counter (OTC) pharmaceutical shipments. The analysis focuses on modeling sales trends and generating short-term forecasts to support inventory planning and anomaly detection.

---

## Project Objectives

- Analyze weekly shipment trends in OTC product data  
- Build and compare a baseline and an enhanced forecasting model  
- Forecast future shipments based on historical patterns  
- Evaluate model performance using R² and mean squared error  

---

## Tools and Libraries Used

- `pandas` – data processing  
- `matplotlib`, `seaborn` – visualization  
- `scikit-learn` – model development  
- `scipy.stats` – statistical testing  

---

## Dataset

- **Filename**: `pharmacy_otc_sales_data.csv`  
- **Key Columns**:
  - `Date`
  - `Product`
  - `Sales Person`
  - `Boxes Shipped`
  - `Amount ($)`
  - `Country`

Data was aggregated weekly to simplify temporal analysis and forecasting.

---

## Modeling Overview

### Baseline Model
- Input: Time index  
- Method: Random Forest  
- Purpose: Establish a simple benchmark for performance comparison  

### Enhanced Model
- Inputs: Lag features, rolling averages, week-of-year, and month  
- Method: Random Forest  
- Outcome: Significantly improved R² and reduced prediction error  

---

## Forecasting

The enhanced model was used to predict box shipments for the next 10 weeks. Forecast results were visualized alongside historical data to evaluate model stability and potential anomalies.

---

## Key Findings

- The enhanced model outperformed the baseline model in both accuracy and stability  
- Incorporating lag and seasonal features improves short-term forecast reliability  
- Grouping products based on their public health relevance may enhance model sensitivity to seasonal and pandemic-driven changes  

---

## Future Improvements

- Integrate external features (e.g., flu season, holidays, weather conditions)  
- Segment product categories for targeted forecasting  
- Test other models discussed in the course for comparative analysis  
- Use model residuals to detect outlier weeks for anomaly tracking  

---

## Conclusion

The project demonstrates that Random Forest regression, enhanced with lag and calendar features, provides a strong foundation for demand forecasting in OTC sales. It can be extended further with domain-specific variables and time-aware modeling practices to support real-world decision-making.

---

## Repository Contents

