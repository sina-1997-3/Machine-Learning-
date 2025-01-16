# Machine Learning Projekt

Repository-Link: [Machine Learning Projekt](https://github.com/sina-1997-3/Machine-Learning-.git)

## Übersicht

Die **Main.ipynb** Datei enthält die vollständige Implementierung. Dies umfasst die Datenvorbereitung, Feature Engineering, Modelltraining, Evaluierung und die Einreichung von Vorhersagen. Die wichtigsten Schritte im Notebook sind wie folgt:

1. **Daten Laden und Validierung**:
   - Die notwendigen Datendateien (`umsatzdaten_gekuerzt.csv`, `kiwo.csv`, `wetter.csv` und `feiertage.csv`) werden geladen und auf Fehler überprüft.
   - Fehlende oder inkonsistente Datumsformate werden behandelt und korrigiert.

2. **Feature Engineering**:
   - Neue Merkmale wie Wochentag, Monat, Quartal und Feiertagsnähe werden erstellt.
   - Die Temperatur wird in die Kategorien "Kalt", "Mild" und "Warm" unterteilt.
   - Rollende Durchschnitte des Umsatztrends über 7 Tage werden berechnet.

3. **Daten Zusammenführen**:
   - Die Datensätze werden basierend auf dem `Datum` zusammengeführt und die relevanten Merkmale für die Analyse beibehalten.

4. **Fehlende Werte Behandeln**:
   - Fehlende Werte werden durch den Median für numerische Merkmale und den Modus für kategorische Variablen ersetzt.

5. **Modelltraining**:
   - **Lineare Regression**: Ein Basismodell für lineare Regression wird erstellt und auf den Daten trainiert.
   - **Neurales Netzwerk**: Ein Deep Learning Modell wird mit Keras erstellt, wobei Schichten wie Dense und Dropout zur Regularisierung verwendet werden. Das Modell wird mit Early Stopping trainiert, um Überanpassung zu vermeiden.

6. **Evaluierung und Einreichung**:
   - Die Modelle werden mit Metriken wie R² und Adjustiertem R² für die lineare Regression sowie Verlust für das neuronale Netzwerk bewertet.
   - Vorhersagen werden auf den Validierungsdaten gemacht und die Ergebnisse in einer CSV-Datei (`submission.csv`) gespeichert.

## Präsentation  

Die Präsentation des Projekts finden Sie unter:  
[Presentation.pptx](Presentation)  

## Anforderungen

Um dieses Projekt auszuführen, benötigen Sie folgende Bibliotheken:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `tensorflow`
- `lightgbm`

### Installation der Anforderungen

Um alle benötigten Bibliotheken zu installieren, können Sie den folgenden Befehl ausführen:

```bash
pip install -r requirements.txt
```

## Cover Image

![Project Cover Image](Praesentation.png)