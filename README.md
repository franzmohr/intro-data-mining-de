# Data Mining

Der Data-Mining-Teil des Seminars. Er besteht aus vier Skripten, die mit kleinen, frei verfügbaren Datensätzen die wichtigsten Verfahren des Data Mining in Python vorstellen: von den Grundlagen der Sprache über Pattern Mining bis zu Klassifikation und Clusteranalyse. Der Text-Mining-Teil baut darauf auf (Repository `intro-text-mining-de`).

| # | Skript | Methoden | Daten | Pakete |
|---|---|---|---|---|
| 01 | [Python-Grundlagen](01-data-mining-python-basics.ipynb) | Zahlen, Text und Listen in Python, Grafiken mit `matplotlib` | Penn World Table 10.0 (`pwt100.xlsx`) | pandas, matplotlib |
| 02 | [Pattern Mining](02-data-mining-pattern-mining.ipynb) | Apriori, FP-Growth, Association Rules (Support, Confidence, Lift) | E-Commerce-Datensatz von Kaggle | pandas, kagglehub, mlxtend |
| 03 | [Klassifikation](03-data-mining-classification.ipynb) | Decision Tree, KNN, logistische Regression, SVM, Random Forest, Ensembles, neuronale Netze | Iris-Datensatz (in scikit-learn enthalten) | scikit-learn, mlxtend, tensorflow |
| 04 | [Clusteranalyse](04-data-mining-cluster-analysis.ipynb) | k-means mit Elbow-Methode, hierarchisches Clustering, Silhouette-Analyse, Feature Selection, Landkarten mit `geopandas` | Scotch-Whisky-Datensatz von Kaggle, Landkarte von UK (`gb.json`) | scikit-learn, kagglehub, geopandas, pyproj, seaborn |

## Ausführen

Die Skripte laufen in jeder Python-Umgebung mit Jupyter. Benötigt werden folgende Pakete (siehe auch den Abschnitt "Voraussetzungen" in Skript 01):

```bash
python -m pip install geopandas kagglehub matplotlib mlxtend numpy openpyxl pandas pyproj scikit-learn seaborn tensorflow jupyterlab
```

Die Notebooks sind **mit Ausgaben** gespeichert, sodass sie sich auch ohne Ausführen lesen lassen.

## Daten

- `pwt100.xlsx` - Penn World Table 10.0 (https://www.rug.nl/ggdc/productivity/pwt/), verwendet in Skript 01.
- `gb.json` - Landkarte des Vereinigten Königreichs (https://simplemaps.com/gis/country/gb), verwendet in Skript 04.
- Die Kaggle-Datensätze in den Skripten 02 und 04 lädt `kagglehub` beim ersten Ausführen herunter und speichert sie lokal zwischen.
