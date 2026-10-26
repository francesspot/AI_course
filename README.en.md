🇵🇱 [Polski](README.md) | 🇬🇧 **English**

# 🤖 AI Course — From a First Model to Neural Networks

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-D00000?logo=keras&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)

> 🎓 Machine-learning course run by the **CyberTech** student research group (Wrocław University of Science and Technology)

Lecture notebooks, exercise solutions and the final project.

## 🏆 Final project — predicting a phone's price range

From a phone's specs (RAM, battery, camera, 4G, Wi-Fi…) the model predicts whether it's low, medium, high or very high cost.

- Preprocessing in a `Pipeline`: encoding text values, filling in missing data, standardisation
- Models compared: logistic regression, Random Forest and two Keras neural networks (BatchNorm, Dropout, L2, early stopping, `ReduceLROnPlateau`)
- Model ensembling
- **Best result: 0.938** balanced accuracy and macro F1 (neural network)

## 📝 Exercises

| Folder | Task | What I used |
|---|---|---|
| `Ćwiczenia1` | Detecting heart disease (classification) | logistic regression, KNN, SVM, Naive Bayes, decision tree; precision, recall, F1 |
| `Ćwiczenia2` | Predicting bike rentals (regression) | imputation (Simple, Iterative, KNN), one-hot encoding, `ColumnTransformer`, linear regression |
| `Ćwiczenia3` | Predicting student performance (regression) | Keras neural network, early stopping, learning-rate scheduling |

Notebooks `1w`–`3w` are the lecture materials (first models, preprocessing, neural networks). The notebooks are in Polish.

## 🚀 Run it

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow jupyter
jupyter notebook
```
