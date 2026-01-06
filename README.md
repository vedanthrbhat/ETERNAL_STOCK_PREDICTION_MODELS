# ETERNAL_STOCK_PREDICTION_MODELS
This project explores practical machine learning approaches for financial time-series forecasting using historical OHLCV (Open, High, Low, Close, Volume) data.

## 👤 Personal Project Overview

I built this project as a **personal learning exercise** to better understand how different machine learning models behave when applied to **financial time-series data**.

Rather than focusing only on predictive accuracy, my objective was to explore the **practical limitations, strengths, and trade-offs** of commonly used ML models on noisy, real-world market data.

I began with **Linear Regression** as a baseline to observe simple trend-following behavior and quickly saw why linear models struggle with non-stationary price series. This provided a clear reference point for evaluating more complex models.

I then implemented a **Random Forest Regressor** to capture non-linear patterns using lagged prices, rolling statistics, and volume. While this improved short-term performance, it also highlighted how tree-based models tend to converge toward a stable value when forecasting far into the future.

Finally, I built an **XGBoost model**, which I treated as the most realistic industry-style approach. To address the flat-line behavior seen in price-level prediction, I reformulated the problem to **predict returns instead of prices** and reconstructed future prices from those returns. This change significantly improved forecast behavior and aligned better with professional best practices in financial modeling.

Throughout the project, I emphasized:
- Time-aware train/test splitting
- Avoiding data leakage
- Understanding model behavior rather than overfitting results
- Clear visualization and evaluation of predictions

This project reflects how I approach machine learning problems:  
by focusing on **correct methodology, interpretability, and realistic expectations**, rather than treating models as black boxes.
