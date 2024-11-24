Hier ist eine Zusammenfassung des Codes für das README, das auf GitHub verwendet werden kann:

---

# Aktienhandels-Vorhersage und -Simulation

Dieses Projekt verwendet maschinelles Lernen zur Vorhersage von Aktienkursen und zur Simulation von Handelsstrategien. Zwei Modelle werden verwendet: eines basierend auf technischen Indikatoren und eines auf Rohdaten (OHLCV: Open, High, Low, Close, Volume). Die Vorhersagen helfen dabei, Handelsentscheidungen zu treffen, die dann in einer Simulationsumgebung getestet werden.

## Funktionsübersicht

### 1. **Vorhersagen mit Technischen Indikatoren**
Die Funktion `predict_for_date` trifft eine Vorhersage für den Aktienkurs an einem bestimmten Datum basierend auf den technischen Indikatoren der letzten 10 Tage. Sie gibt zurück, ob die Aktie gekauft, verkauft oder gehalten werden sollte. Zusätzlich wird der aktuelle Preis und der Preis des nächsten Tages angezeigt.

### 2. **Vorhersagen mit Rohdaten**
Die Funktion `predict_for_date_raw` verwendet Rohdaten (OHLCV) der letzten 10 Tage zur Vorhersage des Handelssignals. Das Modell trifft eine Entscheidung basierend auf den historischen Kursbewegungen der Aktie. Es wird ebenfalls angezeigt, ob die Aktie gekauft, verkauft oder gehalten werden sollte.

### 3. **Vorhersagen für einen Zeitraum**
Die Funktion `generate_predictions` ermöglicht die Berechnung von Handelssignalen über einen definierten Zeitraum hinweg. Sie verwendet sowohl das Modell mit technischen Indikatoren als auch das Modell mit Rohdaten, um eine umfassende Handelsstrategie zu entwickeln.

### 4. **Simulation von Handelsstrategien**
Die Funktion `simulate_trading` simuliert den Aktienhandel auf Grundlage der generierten Handelssignale. Sie berechnet die Performance der Handelsstrategie, basierend auf einem Startkapital und den Entscheidungen, die aufgrund der Vorhersagen getroffen wurden. Die Simulation berücksichtigt Kauf- und Verkaufsentscheidungen sowie das Verwalten von Beständen.

### 5. **Auswertung der Simulation**
Die Funktion `simulate_and_evaluate` führt die Handelsstrategie-Simulationen sowohl für das Modell mit technischen Indikatoren als auch für das Modell mit Rohdaten durch. Sie speichert die Ergebnisse und berechnet den prozentualen Gewinn oder Verlust der Simulation.

### 6. **Interaktive Benutzeroberfläche**
Die Funktionen `get_prediction_date` und `display_predictions` ermöglichen es dem Benutzer, Vorhersagen für ein spezifisches Datum anzufordern. Der Benutzer kann auch entscheiden, ob er detaillierte Daten der letzten 10 Tage sehen möchte und weitere Daten eingeben, um die Vorhersage für unterschiedliche Zeitpunkte zu erhalten.

### 7. **Interaktive Auswahl**
Die Funktion `handle_user_choice` bietet dem Benutzer die Wahl, entweder eine Simulation durchzuführen oder Vorhersagen für ein spezifisches Datum abzurufen. Die Simulation kann auch wiederholt werden, je nach Wunsch des Benutzers.

## Installation

1. Klonen Sie das Repository:

   ```bash
   git clone https://github.com/IhrBenutzername/stock-prediction-simulation.git
   ```

2. Installieren Sie die erforderlichen Bibliotheken:

   ```bash
   pip install -r requirements.txt
   ```

## Nutzung

Um die Simulation oder Vorhersage auszuführen, starten Sie das Programm:

```bash
python main.py
```

Wählen Sie zwischen der Durchführung der Simulation oder der Eingabe eines bestimmten Datums für eine Vorhersage. Das Programm führt automatisch die entsprechende Aktion basierend auf Ihrer Auswahl aus.

---

**Hinweis**: Achten Sie darauf, die benötigten Daten (z. B. Aktienkurse) und Modelle zu haben, um das Skript ordnungsgemäß auszuführen. Weitere Details zur Datensammlung und Modelltraining sind im Code selbst zu finden.

---

Diese Zusammenfassung für das README gibt einen klaren Überblick über die wichtigsten Funktionen des Projekts, die Nutzung und die Installation, sowie die Struktur des Codes. Sie ist gut geeignet, um anderen Nutzern auf GitHub den Einstieg in das Projekt zu erleichtern.