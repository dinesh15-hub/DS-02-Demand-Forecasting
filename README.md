# Nationwide Demand Forecasting and Inventory Optimization

**Nexvia Technologies | DS-02 Project**

An end-to-end demand forecasting and inventory optimization system built using the M5 Forecasting dataset, combining statistical forecasting, machine learning, hierarchical reconciliation, uncertainty estimation, and operations research.

## Project Overview

This project develops a nationwide retail demand forecasting and inventory optimization system using historical Walmart sales data from the M5 Forecasting dataset.

It integrates statistical and machine learning forecasting models with hierarchical reconciliation, prediction intervals, and inventory optimization to generate actionable demand forecasts and replenishment recommendations.

The system provides an integrated workflow for analyzing historical sales, predicting future demand, evaluating forecasting performance, maintaining hierarchical consistency, and optimizing inventory decisions.

## Objectives

- Analyze historical retail sales data and identify demand patterns.
- Perform time-series preprocessing and feature engineering.
- Develop and evaluate multiple demand forecasting approaches.
- Maintain consistency across hierarchical forecasts.
- Estimate demand uncertainty using prediction intervals.
- Optimize inventory replenishment using Google OR-Tools.
- Visualize forecasting performance and inventory recommendations through an interactive dashboard.

## Technology Stack

| Component | Technologies |
|---|---|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Data Storage | Parquet, CSV, JSON |
| Forecasting | Seasonal Naive, Prophet, LightGBM, TFT |
| Reconciliation | Darts |
| Optimization | Google OR-Tools |
| Visualization | Plotly, Dash |
| Development | Google Colab, GitHub |

## Dataset

**M5 Forecasting Dataset**

The project uses the Walmart M5 retail sales dataset, consisting of historical sales, calendar information, and selling prices.

- 30,490 item-store time series
- 3,049 products
- 10 stores
- 3 states
- 1,913 days of historical data

Dataset source: [M5 Forecasting – Kaggle](https://www.kaggle.com/competitions/m5-forecasting-accuracy)

## System Architecture

The following diagram illustrates the end-to-end system architecture, including data preprocessing, forecasting, evaluation, reconciliation, inventory optimization, and dashboard visualization.

![System Architecture](docs/architecture%202.png)

### Implementation Workflow

1. **Data Sources:** Historical sales, calendar events, and selling prices.
2. **Preprocessing:** Data quality checks, time-series reshaping, feature engineering, and Parquet generation.
3. **Forecasting:** Seasonal Naive, Prophet, LightGBM, and Temporal Fusion Transformer.
4. **Evaluation:** Forecast accuracy assessment, model comparison, and prediction interval analysis.
5. **Reconciliation:** Hierarchical forecast reconciliation using Darts.
6. **Inventory Optimization:** Demand-driven replenishment recommendations using Google OR-Tools.
7. **Dashboard:** Interactive forecasting, evaluation, reconciliation, and inventory intelligence using Plotly and Dash.

## Key Components

### 1. Demand Forecasting
- Statistical and machine learning forecasting approaches.
- Lag-based and rolling-window features.
- Nationwide aggregate forecasting.
- Recursive multi-step forecasting.

### 2. Forecast Evaluation
- Fixed-origin model comparison.
- Rolling-origin LightGBM evaluation.
- Forecast accuracy metrics.
- Prediction interval estimation and validation.

### 3. Hierarchical Reconciliation
- Hierarchical forecast consistency.
- Darts reconciliation workflow.
- Bottom-level and aggregate forecast alignment.
- Coherence validation.

### 4. Inventory Optimization
- Demand-based inventory planning.
- Simulated starting inventory.
- Lead-time and ordering cost assumptions.
- Holding cost and stockout penalty considerations.
- Replenishment and order recommendations.

### 5. Interactive Dashboard
- Executive overview.
- Demand forecasting intelligence.
- Hierarchical reconciliation.
- Inventory optimization insights.
- Business intelligence and experimental configuration.

## Evaluation Metrics

Forecasting performance is assessed using:

- **MAE:** Mean Absolute Error.
- **RMSE:** Root Mean Squared Error.
- **WAPE:** Weighted Absolute Percentage Error.
- **RMSSE:** Root Mean Squared Scaled Error.

Evaluation protocols and forecast horizons are documented separately to ensure meaningful model comparisons.

## Repository Structure

```text
DS-02-Demand-Forecasting/
│
├── docs/
│   ├── api_documentation.md
│   ├── architecture 2.png
│   ├── architecture.md
│   ├── dashboard_design.md
│   ├── data_dictionary.md
│   ├── inventory_optimization.md
│   └── testing.md
│
├── models/
│   ├── darts_reconciliation/
│   ├── dashboard/
│   ├── forecast_evaluation/
│   └── inventory_optimization/
│
├── notebooks/
│
├── .gitignore
├── README.md
└── requirements.txt
```

## Experimental Scope and Assumptions

- Full dataset used for feature engineering and full-scale LightGBM evaluation.
- TFT and hierarchical reconciliation evaluated on selected subsets to fit available computational resources.
- Inventory optimization covers 565 item-store series.
- Evaluation populations and protocols differ; WAPE comparisons should use matched evaluation settings.
- Price-reduction features are price-change proxies, not confirmed promotional events.
- Inventory stock, lead times, and costs are simulated assumptions rather than observed M5 dataset variables.

## Project Deliverables

- Source code and implementation notebooks.
- Data preprocessing and feature engineering pipeline.
- Forecasting models and evaluation results.
- Hierarchical reconciliation outputs.
- Prediction interval analysis.
- Inventory optimization outputs.
- Interactive dashboard.
- System architecture and technical documentation.
- Testing and evaluation documentation.
- Project presentation and individual reflection.

## Project Status

**In Development – DS-02 | Nexvia Technologies**

The project combines demand forecasting, hierarchical reconciliation, inventory optimization, and interactive business intelligence into an integrated decision-support system.

---

*This project is developed as part of the Nexvia Technologies DS-02 internship program.*
