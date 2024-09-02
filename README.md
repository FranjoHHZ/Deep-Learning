# Deep-Learning
In diesem Notebook geht es darum, ein Deep Neural Network (DNN) zu erstellen, das den "Banknote Authentication" Datensatz nutzt, um vorherzusagen, ob eine Banknote authentisch ist oder nicht.

# Ausführung
Um dieses Jupyter Notebook auszuführen, müssen Sie dem Link des oben genannten Binder-Badges folgen. Öffnen Sie das Notebook „3-Logistische_Regression_Projekt-Loesung.ipynb“. Sobald das Notbook geöffnet wurden, gehen Sie bitte auf den Reiter "Edit" und drücken Sie "Clear Outputs of all Cells". Nachdem Sie das gemacht haben, können Sie auf "Run all Cells" klicken um den Code auszuführen.

Schritte im jupyter Notebooks:
Daten einlesen und analysieren:
Zuerst wird der Datensatz bank_note_data.csv mit Pandas eingelesen und eine erste Analyse durchgeführt, um einen Überblick über die Verteilung der Klassen ("Class") zu erhalten. Visualisierungen wie Countplots und Pairplots helfen, die Daten zu erkunden und eventuelle Muster in den Merkmalen zu erkennen.

Datenvorbereitung und Standardisierung:
Um sicherzustellen, dass das Modell korrekt trainiert wird, werden die Merkmale des Datensatzes standardisiert. Dafür wird die StandardScaler-Klasse aus Scikit-Learn verwendet. Die standardisierten Daten werden dann in einem neuen DataFrame gespeichert.

Datenaufteilung:
Die standardisierten Daten werden in Trainings- und Testdatensätze aufgeteilt, um das Modell zu trainieren und seine Leistung zu evaluieren. TensorFlow benötigt die Daten im Format von NumPy Arrays, daher werden die Pandas DataFrames entsprechend konvertiert.

Modellerstellung mit TensorFlow:
Ein einfaches Deep Neural Network (DNN) wird mit TensorFlow 1.x erstellt. Die Feature-Spalten werden inferiert, und ein DNN-Classifier wird mit drei verborgenen Schichten (hidden units) erstellt. Das Modell wird auf das Trainingsset gefittet.

Modellbewertung und Vorhersagen:
Nach dem Training wird das Modell verwendet, um Vorhersagen auf dem Testset zu treffen. Ein Classification Report und eine Confusion Matrix werden erstellt, um die Modellleistung zu bewerten. Diese Metriken zeigen, wie gut das Modell in der Lage ist, zwischen authentischen und nicht-authentischen Banknoten zu unterscheiden.

Optionaler Vergleich mit einem Random Forest Classifier:
Um die Leistung des DNN zu evaluieren, wird ein Random Forest Classifier als Vergleichsmodell trainiert und getestet. Die Ergebnisse beider Modelle werden verglichen, um zu zeigen, dass das DNN in diesem Fall eine überlegene Leistung bietet.

# Ergbnisse

Die Ergbnisse zeigen hohe Genauigkeit bei der Klassifizierung der Banknoten. Der Vergleich mit einem Random Forest Classifier sollte verdeutlichen, dass das DNN in der Lage ist, noch genauere Vorhersagen zu treffen, was die Stärke von tiefen neuronalen Netzen bei komplexen Klassifikationsaufgaben herborhebt.


# Binder Badge
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/FranjoHHZ/Deep-Learning/HEAD?labpath=5-Tensorflow_Projekt-Loesung.ipynb)

