# California Housing Price Prediction

This project implements a data analysis pipeline for predicting housing prices in California using the **California Housing Dataset**. The pipeline includes data preprocessing, visualization, and feature engineering to prepare the dataset for machine learning models.

## Features

- **Data Loading**: Fetches and loads the dataset from a remote source.
- **Data Exploration**: Visualizes distributions, correlations, and geographical patterns.
- **Preprocessing**:
  - Handles missing data with imputation.
  - Generates new features such as `rooms_per_household` and `bedrooms_per_room`.
- **Stratified Sampling**: Ensures representative training and test sets.
- **Geospatial Analysis**: Visualizes geographical trends in the data.

## Tools and Libraries

- **Python**: Core programming language.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib**: For visualizations.
- **NumPy**: For numerical computations.
- **Scikit-learn**: For data preprocessing and machine learning utilities.

## Dataset

The dataset is a CSV file containing the following columns:

- `longitude`, `latitude`: Location of the houses.
- `housing_median_age`, `total_rooms`, `total_bedrooms`, `population`, `households`, `median_income`: Demographic and housing features.
- `median_house_value`: Target variable (house value).
- `ocean_proximity`: Proximity to the ocean.

Example rows:

```csv
longitude,latitude,housing_median_age,total_rooms,total_bedrooms,population,households,median_income,median_house_value,ocean_proximity
-122.23,37.88,41.0,880.0,129.0,322.0,126.0,8.3252,452600.0,NEAR BAY
-122.22,37.86,21.0,7099.0,1106.0,2401.0,1138.0,8.3014,358500.0,NEAR BAY
```

## Usage

1. **Clone the repository**:

   ```bash
   git clone https://github.com/your-username/california-housing.git
   cd california-housing
   ```

2. **Install the required dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

3. **Run the script**:
   ```bash
   python main.py
   ```

## Results

The project performs exploratory data analysis, feature engineering, and prepares the dataset for training machine learning models to predict housing prices in California.

### Key Insights:

- **Correlation Analysis**: `median_income` has the strongest positive correlation with `median_house_value`.
- **Geospatial Trends**: Houses closer to the ocean generally have higher median values.
- **Feature Engineering**: New features like `rooms_per_household` improved model performance by better capturing relationships in the data.

### Visualizations:

- **Geographical Distribution**: Scatter plots show housing prices and population densities across California.
- **Histogram Analysis**: Visualizes feature distributions for understanding data ranges and skews.

## How to Contribute

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and push to your branch.
4. Submit a pull request for review.

