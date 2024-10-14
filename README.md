# Exoplanet Detection and Classification 🌌

*Unlocking the mysteries of distant worlds through data science.*

## Table of Contents
1. [Introduction](#introduction)
2. [Project Objectives](#project-objectives)
3. [Data Collection](#data-collection)
4. [Data Processing](#data-processing)
5. [Exploratory Data Analysis & Visualization](#exploratory-data-analysis--visualization)
6. [Modeling & Machine Learning](#modeling--machine-learning)
7. [Results](#results)
8. [Interpretation & Insights](#interpretation--insights)
9. [Conclusion](#conclusion)
10. [Technologies Used](#technologies-used)
11. [Getting Started](#getting-started)
12. [Acknowledgements](#acknowledgements)

## Introduction

The study of exoplanets opens a fascinating window into the complexities of our universe, showcasing the diversity of planetary systems beyond our own. By examining these distant worlds, we gain insights into their formation, composition, and potential habitability.

## Project Objectives

- **Data Exploration:** Analyze and visualize exoplanet data to uncover patterns and insights.
- **Classification Modeling:** Develop predictive models to classify exoplanet candidates.
- **Hypothesis Testing:** Validate findings to ensure reliability.
- **Policy Recommendations:** Provide actionable insights for future research and exploration.

## Data Collection

Data was sourced from the [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu/), which includes detailed measurements and observational data collected by the Kepler mission.

### Dataset Features Include:
- **Orbital Parameters:** Orbital period, transit epoch, impact parameter.
- **Planetary Characteristics:** Radius, equilibrium temperature, insolation flux.
- **Stellar Properties:** Effective temperature, surface gravity, radius.
- **Disposition Labels:** Classification of observations (Confirmed, Candidate, False Positive).

## Data Processing

- **Handling Missing Values:** Imputed missing values and dropped columns with excessive missing data.
- **Feature Engineering:** Renamed columns for readability and created new features where applicable.
- **Data Standardization:** Scaled numerical features for consistent model training.

## Exploratory Data Analysis & Visualization

Conducted in-depth EDA to understand data distributions, relationships, and patterns.

### Key Visualizations:
1. **Disposition Score Distribution**
2. **Planetary Radius by Disposition**
3. **Orbital Period vs. Planetary Radius**
4. **Correlation Heatmap**

## Modeling & Machine Learning

Explored multiple classification algorithms:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)

Used stratified train-test splitting and standardized features to ensure robust model evaluation.

## Results

### Model Performance Comparison:

| Classifier                  | Accuracy  | Precision | Recall  | F1 Score |
|-----------------------------|-----------|-----------|---------|----------|
| Logistic Regression          | 90.24%    | 90.46%    | 90.24%  | 90.23%   |
| **Random Forest**            | **92.20%**| **92.24%**| **92.20%**| **92.19%** |
| K-Nearest Neighbors (KNN)    | 85.54%    | 85.75%    | 85.54%  | 85.37%   |
| Decision Tree                | 88.12%    | 88.12%    | 88.12%  | 88.12%   |
| Support Vector Machine (SVM) | 90.24%    | 90.52%    | 90.24%  | 90.15%   |

The **Random Forest** classifier outperformed other models, indicating its robustness in handling complex datasets with multiple features.

## Interpretation & Insights

- **False Positives:** A significant number of observations were false positives, highlighting the challenges in exoplanet detection.
- **Orbital Periods:** Most exoplanets have shorter orbital periods, suggesting they are closer to their host stars.
- **Planetary Sizes:** Predominance of Earth-sized planets, but detection biases favor larger planets due to more pronounced transit signals.
- **Equilibrium Temperatures:** Majority have lower temperatures, crucial for assessing habitability.

## Conclusion

This project successfully demonstrates the application of data science and machine learning techniques in exoplanet detection and classification. The findings contribute to our understanding of planetary systems and can aid future research in the search for potentially habitable worlds.

## Technologies Used

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SciPy
- **Tools:** Jupyter Notebook

## Getting Started

### Clone the Repository:

```bash
git clone https://github.com/your_username/exoplanet-detection.git
```

### Install Dependencies:
```bash
pip install -r requirements.txt
```
### Run the Jupyter Notebook:
```bash
jupyter notebook Exoplanet_Detection_and_Classification.ipynb
```
### Acknowledgements
- **NASA Exoplanet Archive: For providing the comprehensive dataset.**
- **Kepler Mission Team: For their invaluable contributions to exoplanet research.**
- **Mentors and Educators: For guidance and support throughout the project.**
