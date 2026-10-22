# 🏐 Live Scoreboard Overlay

Ein schlankes, hochperformantes Live-Scoreboard-Overlay für OBS Studio und Web-Streams zur Anzeige von Live-Spieldaten im Volleyball.

---

## 📸 Features

* **Automatische Farberkennung:** Extrahiert die Haupt-Akzentfarbe aus den Teamlogos für ein dynamisches Design.
* **Dynamische Aufschlag-Anzeige:** Platzsparendes, pulsierendes Signal für das aufschlagende Team.
* **Stream-Optimiertes UI:** Transparenter Dark-Mode mit Unschärfe-Effekt (`backdrop-filter`), flüssigen Animationen und hoher Lesbarkeit.
* **Dynamischer Tab-Titel:** Zeigt die aktuellen Paarung direkt im Browser-Tab an (`Team Heim - Team Gast`).

---

## 🚀 Bedienung & Nutzung (OBS Studio)

### 1. Browserquelle einrichten
1. Öffne **OBS Studio**.
2. Füge im Bereich *Quellen* eine neue **Browserquelle** hinzu.
3. Trage die URL deiner Scoreboard-Datei/Domain ein und hänge die Parameter für das gewünschte Spiel an.

### 2. URL-Parameter
Verwende die folgenden URL-Parameter, um das Scoreboard zu steuern:

```text
[https://deine-domain.de/scoreboard.html?match=SPIEL_ID&assoc=VERBAND](https://deine-domain.de/scoreboard.html?match=SPIEL_ID&assoc=VERBAND)

Parameter,Beschreibung,Beispiel
match,Eindeutige ID des Spiels,9f93d1e6-58df-4116...
assoc / verband,Kürzel des zuständigen Verbands,wvv


3. Empfohlene Einstellungen in OBS
Breite: 1920 (oder 1280)

Höhe: 1080 (oder 720)

FPS: 30 oder 60

Benutzerdefiniertes CSS: (leer lassen)

Haken setzen bei: Szenenaktivierung neu laden (optional)

⚙️ Tech Stack
Frontend: HTML5, CSS3 (Flexbox, CSS Variables, Animations), JavaScript (ES6+)

Integration: OBS Browser Source / Webview
