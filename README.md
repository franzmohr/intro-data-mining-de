# Data Mining

Der Data-Mining-Teil des Seminars. Er besteht aus drei Skripten, die mit kleinen, frei verfügbaren Datensätzen die wichtigsten Verfahren des Data Mining in Python vorstellen: Pattern Mining, Klassifikation und Clusteranalyse. Die Python-Grundlagen, die dafür vorausgesetzt werden, liegen im Repository `intro-python-basics-de`. Der Text-Mining-Teil baut auf diesem Teil auf (Repository `intro-text-mining-de`).

| # | Skript | Methoden | Daten | Pakete |
|---|---|---|---|---|
| 02 | [Pattern Mining](02-data-mining-pattern-mining.ipynb) | Apriori, FP-Growth, Association Rules (Support, Confidence, Lift) | E-Commerce-Datensatz von Kaggle | pandas, kagglehub, mlxtend |
| 03 | [Klassifikation](03-data-mining-classification.ipynb) | Decision Tree, KNN, logistische Regression, SVM, Random Forest, Ensembles, neuronale Netze | Iris-Datensatz (in scikit-learn enthalten) | scikit-learn, mlxtend, torch |
| 04 | [Clusteranalyse](04-data-mining-cluster-analysis.ipynb) | k-means mit Elbow-Methode, hierarchisches Clustering, Silhouette-Analyse, Feature Selection, Landkarten mit `geopandas` | Scotch-Whisky-Datensatz von Kaggle, Landkarte von UK (`gb.json`) | scikit-learn, kagglehub, geopandas, pyproj, seaborn |

## Folien

Die Präsentation zum Seminar liegt als [`data-mining.odp`](data-mining.odp) im OpenDocument-Format vor und lässt sich mit LibreOffice Impress oder PowerPoint öffnen. Sie führt in das Data Mining ein und stellt die Verfahren der drei Skripte vor.

## Ausführen

Die Skripte laufen in jeder Python-Umgebung mit Jupyter. Benötigt werden folgende Pakete:

```bash
python -m pip install geopandas kagglehub matplotlib mlxtend networkx numpy pandas pyproj scikit-learn seaborn torch jupyterlab
```

Die Notebooks sind **mit Ausgaben** gespeichert, sodass sie sich auch ohne Ausführen lesen lassen.

## Daten

- `gb.json` - Landkarte des Vereinigten Königreichs (https://simplemaps.com/gis/country/gb), verwendet in Skript 04.
- Die Kaggle-Datensätze in den Skripten 02 und 04 lädt `kagglehub` beim ersten Ausführen herunter und speichert sie lokal zwischen.
