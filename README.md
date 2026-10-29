# Seattle Weather Analysis and Prediction

This project explores Seattle weather observations and applies time-series analysis to study precipitation. The Jupyter notebook covers data exploration, trend and stationarity checks, feature preparation, and an ARIMA model with weather-related exogenous variables (ARIMAX).

## Repository contents

- [`weather.ipynb`](./weather.ipynb) — analysis, visualizations, and modeling workflow.
- [`seattle-weather.csv`](./seattle-weather.csv) — daily weather observations used by the notebook.

The dataset includes date, precipitation, maximum and minimum temperature, wind, and a weather-condition label.

## Getting started

Clone the repository and install the notebook dependencies:

```bash
git clone https://github.com/AnujThakur-ai/weather-analysis-and-prediction.git
cd weather-analysis-and-prediction
python -m pip install jupyter numpy pandas matplotlib seaborn missingno statsmodels plotly scikit-learn
```

Start Jupyter and open the notebook:

```bash
jupyter notebook weather.ipynb
```

Run the notebook from top to bottom. It reads `seattle-weather.csv` from the repository directory.

## Notebook workflow

1. Load and inspect the weather data, including its columns and missing values.
2. Explore precipitation, temperature, wind, and weather conditions with plots and summary statistics.
3. Check time-series stationarity with the Augmented Dickey-Fuller test and examine differenced series.
4. Prepare features, including weather-condition encoding and differenced numeric variables.
5. Fit an ARIMA(1, 1, 1) model with selected weather variables as exogenous inputs and plot fitted precipitation values against observations.

## Notes

The notebook is an exploratory modeling project. Its final plot compares fitted values with observed precipitation; it does not report a held-out test-set evaluation or establish real-world forecasting accuracy. Results may also depend on package versions and the notebook's execution environment.

## License

No license is currently specified in this repository. Contact the repository owner before reusing or redistributing its contents.
