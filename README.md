# Punjab Stubble Burning Fire Prediction Using Machine Learning

## Project Overview

This project focuses on predicting next-day satellite fire detections in Punjab using historical NASA FIRMS satellite fire data.

The objective is to identify geographical grid cells that may experience fire detections on the following day by analyzing historical fire patterns and applying machine learning classification models.

## Objectives

- Analyze satellite fire detection data from 2020 to 2025.
- Perform data cleaning and preprocessing.
- Explore geographical and yearly fire patterns through EDA.
- Engineer features using historical fire activity and neighbouring grid cells.
- Train and compare multiple machine learning classification models.
- Evaluate the final model on unseen 2025 data.

## Dataset

**Source:** NASA FIRMS (Fire Information for Resource Management System)

The dataset contains satellite-based active fire detections.

The analysis uses data from 2020 to 2025, filtered to the study region around Punjab.

Note: Satellite fire detections are not individually verified stubble-burning incidents.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Machine Learning Models

The following classification models were implemented and compared:

1. Logistic Regression
2. K-Nearest Neighbors (KNN)
3. Naive Bayes
4. Decision Tree
5. Random Forest
6. Support Vector Machine (SVM)
7. Multi-Layer Perceptron (MLP)

Additional analysis includes regression, K-Means clustering and Principal Component Analysis (PCA).

## Model Evaluation

The final classification model was selected using PR-AUC on the validation data.

The MLP model achieved the following results on the unseen 2025 test data:

| Metric | Score |
|---|---:|
| PR-AUC | 0.730 |
| ROC-AUC | 0.883 |
| Accuracy | 0.828 |
| Precision | 0.640 |
| Recall | 0.717 |
| F1-Score | 0.676 |

## Project Structure

- `INT234Project.ipynb` - Main project notebook
- `outputs/` - Generated graphs, visualizations and analysis results

## How to Run

1. Clone this repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook.
4. Make sure the required dataset files are available in the expected folder.
5. Run the notebook cells in sequence.

Install dependencies:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Conclusion

The project demonstrates how historical satellite fire patterns can be used to predict next-day fire detections using machine learning.

The MLP classifier achieved a PR-AUC of 0.730 on the 2025 test data, outperforming the evaluated baseline approaches.

## Future Scope

- Include weather variables such as rainfall, temperature and wind speed.
- Incorporate additional satellite datasets.
- Improve geographical coverage and prediction accuracy.
- Develop an interactive fire-risk monitoring dashboard.

## Author

Shivam Kumar Singh

B.Tech CSE | Data Science

GitHub: https://github.com/shivam-rajput301/Fire-Prediction-ML
