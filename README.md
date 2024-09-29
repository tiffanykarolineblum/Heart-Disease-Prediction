# Herzkrankheit Vorhersage Projekt

## Übersicht
Dieses Projekt zielt darauf ab, die Präsenz von Herzkrankheiten bei Patienten mit Hilfe verschiedener Machine-Learning-Algorithmen vorherzusagen. Der verwendete Datensatz enthält verschiedene Merkmale wie Alter, Cholesterinwerte, maximale Herzfrequenz und weitere, um prädiktive Modelle zu erstellen, die klassifizieren, ob ein Patient an einer Herzkrankheit leidet.

Wir wenden mehrere Machine-Learning-Modelle an, bewerten deren Leistung anhand verschiedener Metriken und vergleichen die Ergebnisse, die auf skalierten und normalisierten Eingabedaten basieren. Das Ziel ist es, das Modell zu identifizieren, das die höchste Genauigkeit und Effizienz bei der Vorhersage von Herzkrankheiten bietet.

## Verwendete Machine-Learning-Modelle
Die folgenden Machine-Learning-Algorithmen wurden in diesem Projekt implementiert:
1. **K-Nearest Neighbors (KNN)**
2. **Logistische Regression**
3. **Naive Bayes**
4. **Random Forest Classifier**

Jedes Modell wird sowohl auf **skalierten** als auch auf **normalisierten** Datensätzen evaluiert.

## Metriken
Die folgenden Leistungsmetriken werden zur Bewertung der Modelle verwendet:
- **Genauigkeit (Accuracy)**: Der Anteil der korrekt vorhergesagten Instanzen an allen Instanzen.
- **F1-Score**: Das harmonische Mittel von Präzision und Recall, welches beide Metriken ausgleicht.
- **Präzision (Precision)**: Der Prozentsatz der positiven Vorhersagen, die tatsächlich korrekt sind.
- **Recall**: Die Fähigkeit, alle tatsächlichen positiven Fälle korrekt zu identifizieren.
- **ROC AUC Score**: Misst die Fähigkeit des Modells, zwischen positiven und negativen Klassen zu unterscheiden.
- **Log Loss**: Eine Metrik, die die auf Wahrscheinlichkeiten basierenden Vorhersagen des Modells bewertet.

## Datensatz
Der in diesem Projekt verwendete Datensatz enthält mehrere Merkmale, die für Herzkrankheiten relevant sind, darunter:
- **age**: Alter des Patienten
- **chol**: Cholesterinwert
- **thalach**: Maximale Herzfrequenz
- **trestbps**: Ruheblutdruck
- **oldpeak**: ST-Depression, induziert durch Bewegung

Der Datensatz wird vorverarbeitet und fehlende Werte werden behandelt, bevor die Modelle trainiert werden.

## Projektablauf
1. **Datenvorbereitung**:
    - Fehlende Werte behandeln und Merkmale vorbereiten.
    - Daten mithilfe von `StandardScaler` und `Normalizer` skalieren und normalisieren.
  
2. **Modelltraining**:
    - Trainiere und evaluiere jedes der oben genannten Modelle auf skalierten und normalisierten Daten.

3. **Modellbewertung**:
    - Die Leistung wird anhand der oben genannten Metriken bewertet.
    - Die Ergebnisse werden in Balkendiagrammen visualisiert, um einen einfachen Vergleich zu ermöglichen.

## Zusammenfassung der Ergebnisse
- Der **Random Forest Classifier** zeigt in beiden Szenarien (skaliert und normalisiert) die beste Leistung mit hohen Genauigkeits-, Recall- und ROC-AUC-Werten.
- **KNN** und **Naive Bayes** zeigen eine hohe **Präzision**, haben jedoch einen niedrigeren **Recall**, was bedeutet, dass sie möglicherweise einige positive Fälle übersehen.
- Die **Logistische Regression** bietet eine ausgewogene Leistung und ist eine solide Alternative, wenn ein Gleichgewicht zwischen Präzision und Recall wichtig ist.


