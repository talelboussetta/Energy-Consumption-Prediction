# Energy Consumption Prediction

This project involves predicting energy consumption in a household using various power meters. The dataset contains data collected over time, including features like global active power, voltage, and sub-metering values for different appliances in the home.

## Dataset Overview
- **Global_active_power**: Total active power consumed by the house (in kilowatts).
- **Global_reactive_power**: Reactive power used in the system.
- **Voltage**: The voltage of the electricity supply (in volts).
- **Sub_metering_1, Sub_metering_2, Sub_metering_3**: Energy consumption by individual appliances (kitchen, laundry, and water heater/AC).
- **Date & Time**: Time of the reading (in `dd/mm/yyyy HH:MM:SS` format).

## Problem Statement
The goal of this project is to predict energy consumption patterns in a household based on the features provided. Specifically, I am aiming to predict global active power, based on the sub-metering values and other power-related metrics.

## Data Cleaning & Preprocessing
1. Combined **Date** and **Time** columns into a single **datetime** column.
2. Extracted useful features from the datetime, such as hour, day, month, weekday, and whether it's a weekend.
3. Handled missing values by replacing `?` with `NaN` and dropped rows with invalid data.
4. Visualized energy consumption patterns for different appliances.

## Model
- **Linear Regression** was used to predict energy consumption based on the available features.
- Evaluated using **Mean Absolute Error (MAE)**, **Mean Squared Error (MSE)**, and **R² Score** to assess model performance.

## Results
- **MAE**: 0.0281
- **MSE**: 0.00201
- **R² Score**: 0.9986

## Conclusion
The model performs exceptionally well, with an R² score of nearly 1, meaning it explains 99.86% of the variance in energy consumption. This indicates the model’s ability to predict energy usage accurately based on the given features.

## Files Included
- **data/**: Contains the dataset used for training and testing.
- **notebooks/**: Jupyter notebook containing the full workflow, from data preprocessing to model training and evaluation.
- **requirements.txt**: A list of dependencies required to run the project.

## License
Feel free to use and modify this code. Acknowledgment of the original work is appreciated.
