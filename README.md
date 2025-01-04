
# Predicting IMDb Scores Using Features from Movie Titles and Credits

## Overview
This project aims to predict IMDb scores for movies using features extracted from movie titles and credits. By leveraging machine learning techniques, the study developed models to provide accurate predictions of IMDb scores. The key finding highlights the Random Forest model's superior performance in terms of predictive accuracy.

---

## Features
1. **Data Integration**: Combines titles and credits datasets to create a comprehensive dataset.
2. **Feature Engineering**: Includes features like `description_length`, `character_length`, and `genres`.
3. **Machine Learning Models**:
   - Random Forest (with hyperparameter tuning).
   - Linear Regression.
4. **Evaluation Metrics**: Performance evaluated using MSE, MAE, and RMSE.

---

## Materials and Methods

### Datasets
- **Titles Dataset**: Contains information about movie titles, descriptions, genres, and runtime.
- **Credits Dataset**: Includes details about cast and crew, their names, and roles.

### Data Preparation
1. Addressed missing values to maintain data integrity.
2. Engineered additional features like `description_length` and `character_length`.
3. Merged datasets on the `id` field to create a unified dataset.

### Machine Learning Techniques
1. Feature Selection: Selected numerical and categorical features for the models.
2. Hyperparameter Tuning: Optimized Random Forest hyperparameters using GridSearchCV.

---

## Experimental Results

| Model              | MSE  | MAE  | RMSE |
|--------------------|-------|------|------|
| Random Forest      | 0.35  | 0.45 | 0.59 |
| Linear Regression  | 0.42  | 0.50 | 0.65 |

- **Best Model**: Random Forest achieved the best performance due to its ability to handle complex feature interactions.

---

## Visualizations
1. **Pair Plot**: Showed relationships between features like `description_length`, `runtime`, and IMDb scores.
2. **Histogram**: Displayed the distribution of IMDb scores, highlighting score density.

---

## Discussion
1. **Key Findings**:
   - Features like `description_length` and `character_length` significantly influence IMDb scores.
   - Random Forest outperformed Linear Regression in accuracy and robustness.
2. **Limitations**:
   - Potential overfitting in models.
   - Exclusion of features like audience reviews and social media sentiment.

---

## Conclusions
- The study successfully developed a predictive model for IMDb scores using features from titles and credits.
- Random Forest demonstrated superior predictive capabilities.
- The results provide actionable insights for filmmakers and marketers to guide production and marketing strategies.

---

## Future Work
- Incorporate additional features like audience reviews and social media sentiment.
- Explore advanced models to further improve prediction accuracy.

---

## How to Run
1. **Setup**: Install necessary Python libraries (`scikit-learn`, `pandas`, etc.).
2. **Data Loading**: Prepare and load the titles and credits datasets.
3. **Model Training**: Run the machine learning scripts to train and evaluate models.
4. **Visualization**: Generate visualizations for insights into the data and results.

---

## Acknowledgments
This project is a demonstration of using machine learning for predictive analytics in the film industry, providing insights for stakeholders to make data-driven decisions.
