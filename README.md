# Homestay Pricing Prediction Project

## Overview
This project is aimed at building a predictive model to estimate the `log_price` of homestay listings based on comprehensive analysis of various features including characteristics, amenities, and host information. By leveraging machine learning techniques and exploratory data analysis (EDA), the goal is to provide actionable insights for both homestay hosts and potential guests.

## Contents
1. **Feature Engineering**
   - In this stage, the dataset is enriched by creating new features that provide additional insights into the listings. For instance, `Host_Tenure` is calculated to measure the experience of hosts, `Amenities_Count` quantifies the property offerings, and `Days_Since_Last_Review` assesses listing activity and relevance.

2. **Exploratory Data Analysis (EDA)**
   - Through EDA, we delve into the dataset to uncover patterns and relationships. We analyze how pricing (`log_price`) correlates with both categorical features like `room_type` and numerical features like `accommodates`. Tools such as correlation matrices, histograms, and scatter plots are utilized for deeper exploration.

3. **Geospatial Analysis**
   - Geographical data is analyzed to understand regional pricing trends. Listings are plotted on a map using latitude and longitude data to visually assess price distribution. This analysis helps in identifying if certain neighborhoods or proximity to city centers influence pricing.

4. **Sentiment Analysis on Textual Data**
   - Textual data from the `description` field is subjected to sentiment analysis. By extracting sentiment scores, we aim to determine whether positive or negative descriptions influence listing prices. This analysis adds a qualitative dimension to our predictive model.

5. **Amenities Analysis**
   - The `amenities` provided in the listings are thoroughly parsed and analyzed. Statistical tests are applied to identify which amenities are most associated with higher or lower prices. Insights from this analysis inform both pricing strategy and model inputs.

6. **Categorical Data Encoding**
   - Categorical variables such as `room_type`, `city`, and `property_type` are converted into a format suitable for machine learning analysis using one-hot encoding. This ensures that the model can interpret these variables as distinct features without any ordinal implication.

7. **Model Development and Training**
   - Predictive models including linear regression, RandomForest, and GradientBoosting are developed and trained to estimate `log_price`. The model-building process is documented, specifying the choice of algorithms and rationale behind them.

8. **Model Optimization and Validation**
   - Models are systematically optimized using techniques like grid search to experiment with different hyperparameters settings. Validation is performed through techniques like k-fold cross-validation to ensure the model generalizes well to unseen data.

9. **Feature Importance and Model Insights**
   - Trained models are analyzed to identify which features significantly impact `log_price`. Model-specific methods such as feature importance scores and SHAP values are employed to gain insights into feature contributions.

10. **Predictive Performance Assessment**
    - The performance of the final model is critically evaluated on a reserved test set using metrics such as RMSE and R-squared. Detailed analysis of residuals is provided to check for any patterns that might suggest model biases or misfit.

## Usage
1. **Dataset**: Ensure the "Homestays_Data.csv" dataset is available for analysis.
2. **Environment Setup**: Set up your Python environment with necessary libraries such as pandas, numpy, scikit-learn, and geopandas.
3. **Notebook Execution**: Execute the provided Jupyter notebook or Python scripts to run through the project tasks sequentially.








