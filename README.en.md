[Polski](README.md) | **English**

# AI Course — Machine Learning Basics

Lecture notebooks, exercise lists and a final project from an introductory machine-learning course. Everything is in Jupyter notebooks using **pandas**, **scikit-learn** and **Keras**. The notebooks are written in Polish.

## Lectures

| Notebook | Topic | Dataset |
|----------|-------|---------|
| `1w-czym-sa-modele-ai-i-jak-je-uczyc.ipynb` | What AI models are and how they learn — train/test split, KNN and Random Forest classifiers, accuracy, precision, recall, F1, confusion matrix | `mushroom_data.csv` |
| `2w-preprocessing-i-analiza-danych.ipynb` | Preprocessing and data analysis — missing values, encoding text, feature engineering, scaling, pipelines | crab age (Kaggle) |
| `3w-sieci-neuronowe.ipynb` | Neural networks in Keras — architecture, loss and optimiser, training, monitoring test loss | `car_prices.csv` |

## Exercise lists

| Folder | Task | Methods |
|--------|------|---------|
| `Ćwiczenia1` | Detecting heart disease from patient data (classification) | Logistic Regression, KNN, SVM, Naive Bayes, Decision Tree; accuracy, precision/recall, F1, precision-recall curve |
| `Ćwiczenia2` | Predicting bike rentals (regression) | Dropping columns, imputation (Simple, Iterative, KNN), one-hot encoding, scaling, `ColumnTransformer` + `Pipeline`, linear regression; MAE, MSE, MAPE |
| `Ćwiczenia3` | Predicting student performance (regression) | Keras neural network, validation loss monitoring, early stopping, learning-rate scheduling |

## Final project — `Projekt/`

Classifying **mobile phones into 4 price ranges** (low, medium, high, very high cost) from their specifications.

- Preprocessing: mapping text values to binary, median imputation and standardisation in a `Pipeline`.
- Models compared: Logistic Regression, Random Forest and two Keras neural networks (sparse vs one-hot categorical cross-entropy, with batch normalisation, dropout, L2, early stopping and `ReduceLROnPlateau`).
- Weighted ensembles of the models' predicted probabilities.
- **Best result:** the neural network with sparse categorical cross-entropy — **0.938** balanced accuracy and macro F1.

## Running

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow jupyter
jupyter notebook
```

Open a notebook from its own folder so the relative paths to the CSV files work.
