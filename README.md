# Nationwide Demand Forecasting and Inventory Optimization

**Nexvia Technologies | DS-02 Project**

## Project Overview

This project develops an end-to-end demand forecasting and inventory optimization system using the M5 Forecasting dataset.

It combines statistical and machine learning forecasting models with hierarchical forecast reconciliation, prediction intervals, and operations research to support data-driven inventory planning.

The system aims to forecast product demand across multiple stores and categories, evaluate forecasting performance, and generate inventory replenishment recommendations.

## Objectives

- Analyze historical retail sales data.
- Develop meaningful time-series features.
- Compare multiple demand forecasting approaches.
- Maintain consistency across hierarchical forecasts.
- Estimate demand uncertainty using prediction intervals.
- Optimize inventory decisions using Google OR-Tools.
- Visualize forecasts, performance metrics, and inventory recommendations.

## Technology Stack

| Component | Technologies |
|---|---|
| Programming | Python |
| Data Processing | Pandas, NumPy |
| Data Storage | Parquet |
| Forecasting | Naive, Prophet, LightGBM, Temporal Fusion Transformer (TFT) |
| Reconciliation | Darts |
| Optimization | Google OR-Tools |
| Visualization | Plotly, Dash |
| Development | Google Colab, GitHub |

## System Architecture

The proposed workflow consists of:

1. Data ingestion and preprocessing
2. Feature engineering
3. Demand forecasting
4. Hierarchical reconciliation
5. Prediction interval estimation
6. Inventory optimization
7. Interactive dashboard visualization

## Dataset

**M5 Forecasting Dataset**

The project uses historical Walmart retail sales data, together with calendar information and selling prices.

Dataset source: [M5 Forecasting – Kaggle](https://www.kaggle.com/competitions/m5-forecasting-accuracy)

## Current Progress

- [x] M5 dataset downloaded and prepared.
- [x] Historical sales data processed.
- [x] Calendar and price data merged.
- [x] Parquet feature files generated.
- [x] Lag and rolling features generated.
- [x] LightGBM training dataset prepared.
- [ ] Naive forecasting model
- [ ] Prophet forecasting model
- [ ] LightGBM evaluation
- [ ] TFT forecasting model
- [ ] Hierarchical reconciliation
- [ ] Prediction intervals
- [ ] Inventory optimization
- [ ] Plotly Dash dashboard
- [ ] Testing and documentation

## Evaluation Metrics

Forecasting performance will be evaluated using:

- Weighted Absolute Percentage Error (WAPE)
- Root Mean Squared Scaled Error (RMSSE)

Actual evaluation results will be added after model execution.

## Project Deliverables

- Working demonstration or screen recording
- GitHub source code and documentation
- System architecture diagram
- Data and API documentation
- Model evaluation and test results
- Interactive forecasting dashboard
- Project presentation and individual reflection

## Project Status

**In Development**

This project is being developed as part of Nexvia Technologies DS-02.

---

*Note: Model performance, optimization results, and dashboard capabilities will be documented after implementation and validation.*
