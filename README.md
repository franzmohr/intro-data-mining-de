# Data Mining

Der Data-Mining-Teil des Seminars. Er besteht aus einem Vorbereitungsskript und drei Skripten, die mit kleinen, frei verfügbaren Datensätzen die wichtigsten Verfahren des Data Mining in Python vorstellen: Pattern Mining, Klassifikation und Clusteranalyse. Die Python-Grundlagen, die dafür vorausgesetzt werden, liegen im Repository `intro-python-basics-de`. Der Text-Mining-Teil baut auf diesem Teil auf (Repository `intro-text-mining-de`).

| # | Skript | Methoden | Daten | Pakete |
|---|---|---|---|---|
| 00 | [Vorbereitungen](00-preparations.ipynb) | Installation aller benötigten Pakete | - | pip |
| 01 | [Pattern Mining](01-data-mining-pattern-mining.ipynb) | Apriori, FP-Growth, Association Rules (Support, Confidence, Lift), Multilevel Association Rules mit einer Konzepthierarchie | E-Commerce-Datensatz von Kaggle | pandas, kagglehub, mlxtend |
| 02 | [Klassifikation](02-data-mining-classification.ipynb) | Entscheidungsbaum, KNN, logistische Regression, SVM, Random Forest, Ensembles, neuronale Netze mit zwei und drei Output-Knoten, Bewertung mit Testdaten und Kreuzvalidierung | Iris-Datensatz (in scikit-learn enthalten) | scikit-learn, mlxtend, torch |
| 03 | [Clusteranalyse](03-data-mining-cluster-analysis.ipynb) | k-means, agglomeratives Clustering mit Dendrogramm, DBSCAN, Evaluation (Hopkins-Statistik, Elbow-Methode, Silhouette, Adjusted Rand Index), DENCLUE, PageRank, Stochastic Block Model, Feature Selection, Landkarten mit `geopandas` | Scotch-Whisky-Datensatz von Kaggle, Landkarte von UK (`gb.json`) | scikit-learn, scipy, kagglehub, geopandas, pyproj, seaborn, networkx |

## Folien

Die Präsentation zum Seminar liegt als [`data-mining.odp`](data-mining.odp) im OpenDocument-Format vor und lässt sich mit LibreOffice Impress oder PowerPoint öffnen. Sie führt in das Data Mining ein und stellt die Verfahren der drei Skripte vor.

## Ausführen

Die Skripte laufen in jeder Python-Umgebung mit Jupyter. Benötigt werden folgende Pakete, die sich auch über das Notebook [`00-preparations.ipynb`](00-preparations.ipynb) installieren lassen:

```bash
python -m pip install geopandas kagglehub matplotlib mlxtend networkx numpy pandas pyproj scikit-learn scipy seaborn torch jupyterlab
```

Die Notebooks sind **mit Ausgaben** gespeichert, sodass sie sich auch ohne Ausführen lesen lassen.

## Daten

- `gb.json` - Landkarte des Vereinigten Königreichs (https://simplemaps.com/gis/country/gb), verwendet in Skript 03.
- Die Kaggle-Datensätze in den Skripten 01 und 03 lädt `kagglehub` beim ersten Ausführen herunter und speichert sie lokal zwischen.

## Literatur

- Han, J., Pei, J. und Tong, H. (2023): Data Mining: Concepts and Techniques. 4. Auflage. Morgan Kaufmann.
- Kelleher, J. D., Mac Namee, B. und D'Arcy, A. (2020): Fundamentals of Machine Learning for Predictive Data Analytics: Algorithms, Worked Examples, and Case Studies. 2. Auflage. MIT Press.
