🇵🇱 **Polski** | 🇬🇧 [English](README.en.md)

# 🤖 Kurs AI — od pierwszego modelu do sieci neuronowych

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?logo=scikitlearn&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-D00000?logo=keras&logoColor=white) ![pandas](https://img.shields.io/badge/pandas-150458?logo=pandas&logoColor=white)

> 🎓 Kurs uczenia maszynowego prowadzony przez koło naukowe **CyberTech** (Politechnika Wrocławska)

Moje notatniki z wykładów, rozwiązania list zadań i projekt końcowy. 📓

## 🏆 Projekt końcowy — przewidywanie półki cenowej telefonu

Na podstawie specyfikacji telefonu (RAM, bateria, aparat, 4G, Wi-Fi…) model przewiduje, czy telefon jest tani, średni, drogi czy bardzo drogi. 📱

- 🧹 Preprocessing w `Pipeline`: kodowanie wartości tekstowych, uzupełnianie braków, standaryzacja
- ⚔️ Porównanie modeli: regresja logistyczna, Random Forest i dwie sieci neuronowe w Keras (BatchNorm, Dropout, L2, early stopping, `ReduceLROnPlateau`)
- 🤝 Łączenie modeli (ensembling)
- 🥇 **Najlepszy wynik: 0,938** balanced accuracy i macro F1 (sieć neuronowa)

## 📝 Listy zadań

| | Zadanie | Czego użyłem |
|---|---|---|
| ❤️ `Ćwiczenia1` | Wykrywanie choroby serca (klasyfikacja) | regresja logistyczna, KNN, SVM, naiwny Bayes, drzewo decyzyjne; precision, recall, F1 |
| 🚲 `Ćwiczenia2` | Przewidywanie liczby wypożyczeń rowerów (regresja) | imputacja (Simple, Iterative, KNN), one-hot encoding, `ColumnTransformer`, regresja liniowa |
| 🎓 `Ćwiczenia3` | Przewidywanie wyników uczniów (regresja) | sieć neuronowa w Keras, early stopping, harmonogram learning rate |

Notatniki `1w`–`3w` to materiały z wykładów (pierwsze modele, preprocessing, sieci neuronowe).

## 🚀 Uruchomienie

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow jupyter
jupyter notebook
```
