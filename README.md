# Mining Quality Prediction

## Project Overview
**Quality Prediction in a Mining Process**

This project explores real industrial data from a flotation plant, one of the most important parts of a mining process, to help manufacturing plants become more efficient.

### Context
It is not always easy to find databases from real-world manufacturing plants, especially mining plants. This database comes from a flotation plant.

The main goal is to use this data to predict how much impurity (silica) is in the ore concentrate. Since this impurity is measured every hour, predicting the silica content can empower engineers with early information to take corrective actions in advance. This helps reduce impurities and benefits the environment by reducing the amount of ore that goes to tailings.

### Dataset Description
The dataset contains process data from a flotation plant used to concentrate iron ore.
- **Column 1:** Time and date range (March 2017 to September 2017). Some columns were sampled every 20 seconds, while others were sampled hourly.
- **Columns 2 & 3:** Quality measures of the iron ore pulp right before it is fed into the flotation plant.
- **Columns 4 - 8:** Important variables that impact the final ore quality.
- **Columns 9 - 22:** Process data, including level and air flow inside the flotation columns, which impact ore quality.
- **Last 2 Columns:** Final iron ore pulp quality measurement from the lab.

**Target Variable:** The last column, which represents the `% of silica in the iron ore concentrate`.

### Project Goals (Expected Submission)
1. **Minute-by-Minute Prediction:** Is it possible to predict `% Silica Concentrate` every minute?
2. **Forecasting Horizon:** How many steps (hours) ahead can we predict `% Silica in Concentrate`? This helps engineers act in a predictive and optimized way, mitigating the percentage of iron sent to tailings.
3. **Feature Independence:** Is it possible to predict `% Silica in Concentrate` without using the `% Iron Concentrate` column (as they are highly correlated)?

## Environment Setup
This project uses the following dependencies:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `jupyter`
- `xgboost`

To set up the environment, install the dependencies using the provided `requirements.txt`:
```bash
pip install -r requirements.txt
```
