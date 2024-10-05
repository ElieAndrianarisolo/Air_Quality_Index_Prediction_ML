# Air Quality Index Prediction using Machine Learning

This project aims to predict the Air Quality Index (AQI) using time-series forecasting with the FB Prophet algorithm. The dataset used in this project is sourced from the UCI Machine Learning Repository, and contains data on air quality measurements. The project involves data cleaning, handling missing values, and performing time-series forecasting.

## Dataset

- **Source**: [Air Quality Dataset](https://archive.ics.uci.edu/dataset/360/air+quality)
- **Description**: The dataset contains hourly averaged responses from an array of 5 metal oxide chemical sensors embedded in an air quality monitoring device. The device was deployed on the field in a significantly polluted area of an Italian city at road level.
- **File Format**: CSV

## Project Steps

### 1. Data Collection & Processing

- Load the dataset from a CSV file into a pandas DataFrame.
- Clean the data by removing unwanted columns and handling missing values. Specifically, values marked as `-200` in the dataset are treated as missing and replaced with the mean of the respective column.

### 2. Data Transformation

- Convert date and time information from the dataset into a format suitable for time-series analysis.
- Combine the date and time columns into a single timestamp column.

### 3. Time Series Forecasting

- Use the FB Prophet algorithm to forecast future AQI values.
- Train the model on the preprocessed data, and predict the AQI for future time periods.

### 4. Visualization

- Plot the forecasted values and the forecast components using FB Prophet’s built-in plotting functions.

## Usage

1. Load the dataset by running the provided script.
2. The script cleans the data, handles missing values, and prepares it for analysis.
3. The FB Prophet model is trained on the dataset to predict future air quality index values.
4. Forecasted results are plotted to show predictions over the next 365 hours.

## References

- [FB Prophet Documentation](https://facebook.github.io/prophet/docs/quick_start.html)
- [UCI Air Quality Dataset](https://archive.ics.uci.edu/dataset/360/air+quality)