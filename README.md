**Polski** | [English](README.en.md)

# Kurs AI — podstawy uczenia maszynowego

Notatniki z wykładów, listy ćwiczeń i projekt końcowy z wprowadzającego kursu uczenia maszynowego. Całość w notatnikach Jupyter z użyciem **pandas**, **scikit-learn** i **Keras**.

## Wykłady

| Notatnik | Temat | Zbiór danych |
|----------|-------|--------------|
| `1w-czym-sa-modele-ai-i-jak-je-uczyc.ipynb` | Czym są modele AI i jak je uczyć — podział na zbiór treningowy i testowy, klasyfikatory KNN i Random Forest, accuracy, precision, recall, F1, macierz pomyłek | `mushroom_data.csv` |
| `2w-preprocessing-i-analiza-danych.ipynb` | Preprocessing i analiza danych — brakujące wartości, kodowanie tekstu, tworzenie cech, skalowanie, pipeline'y | wiek krabów (Kaggle) |
| `3w-sieci-neuronowe.ipynb` | Sieci neuronowe w Keras — architektura, funkcja straty i optymalizator, trening, monitorowanie straty na zbiorze testowym | `car_prices.csv` |

## Listy ćwiczeń

| Folder | Zadanie | Metody |
|--------|---------|--------|
| `Ćwiczenia1` | Wykrywanie choroby serca na podstawie danych pacjenta (klasyfikacja) | Regresja logistyczna, KNN, SVM, naiwny Bayes, drzewo decyzyjne; accuracy, precision/recall, F1, krzywa precision-recall |
| `Ćwiczenia2` | Przewidywanie liczby wypożyczeń rowerów (regresja) | Usuwanie kolumn, imputacja (Simple, Iterative, KNN), one-hot encoding, skalowanie, `ColumnTransformer` + `Pipeline`, regresja liniowa; MAE, MSE, MAPE |
| `Ćwiczenia3` | Przewidywanie wyników uczniów (regresja) | Sieć neuronowa w Keras, monitorowanie straty walidacyjnej, early stopping, zmniejszanie learning rate'u |

## Projekt końcowy — `Projekt/`

Klasyfikacja **telefonów komórkowych do 4 półek cenowych** (niska, średnia, wysoka, bardzo wysoka) na podstawie ich specyfikacji.

- Preprocessing: zamiana wartości tekstowych na binarne, imputacja medianą i standaryzacja w `Pipeline`.
- Porównane modele: regresja logistyczna, Random Forest i dwie sieci neuronowe w Keras (sparse vs one-hot categorical cross-entropy, z batch normalization, dropoutem, L2, early stoppingiem i `ReduceLROnPlateau`).
- Ważone łączenie (ensembling) prawdopodobieństw z kilku modeli.
- **Najlepszy wynik:** sieć neuronowa z sparse categorical cross-entropy — **0,938** balanced accuracy i macro F1.

## Uruchamianie

```bash
pip install pandas numpy matplotlib seaborn scikit-learn tensorflow jupyter
jupyter notebook
```

Otwieraj notatnik z jego folderu, żeby działały względne ścieżki do plików CSV.
