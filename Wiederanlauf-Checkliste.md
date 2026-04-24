# Wiederanlauf-Checkliste PERT-Methode

Diese Checkliste hilft dabei, nach einem Neustart von Codex oder nach einer Unterbrechung schnell den richtigen Arbeitsstand zu finden.

## 1. Zielstand prüfen

- Aktuellen Arbeitsordner öffnen: `/Users/bernhard/Documents/KI-Projekte/PERT-Methode`
- Prüfen, ob `index.html` vorhanden ist
- Prüfen, ob `vendor/` vorhanden ist
- Prüfen, ob `vendor/fonts/` vorhanden ist

## 2. Wichtige Dateien

- `index.html` = aktuelle PERT-Anwendung
- `README.md` = Projektbeschreibung
- `vendor/chart.umd.min.js` = lokale Chart-Bibliothek
- `vendor/html2canvas.min.js` = lokaler PDF-/Canvas-Helfer
- `vendor/jspdf.umd.min.js` = lokaler PDF-Export
- `vendor/fonts/Geist-Latin.woff2` = lokale Schriftdatei
- `vendor/fonts/Geist-LatinExt.woff2` = lokale Schriftdatei für erweiterte Zeichen
- `vendor/fonts/GeistMono-Latin.woff2` = lokale Monospace-Schriftdatei

## 3. Wichtige Funktionen der App

- `Projektdatei speichern` = aktuelle Eingaben als JSON-Datei herunterladen
- `Projektdatei laden` = JSON-Datei auswählen und aktuelles Projekt ersetzen
- `Demo-Vorlage laden` = fest im Code hinterlegte Demodaten laden
- `Neues Projekt` = aktuelle Eingaben löschen und leere Maske öffnen
- `PDF exportieren` = aktuelle Ansicht als PDF erzeugen

## 4. Wenn etwas fehlt

- Fehlen nur einzelne Runtime-Dateien, dann zuerst `vendor/` vollständig prüfen
- Fehlt `index.html`, zuerst den letzten lokalen oder GitHub-Stand wiederherstellen
- Fehlen Font-Dateien, dann muss die App auf Fallback-Schriften ausweichen

## 5. Start für die Arbeit

1. Prüfen, ob der aktuelle Stand vollständig ist
2. Falls nötig, Dateien aus dem letzten sicheren Stand wiederherstellen
3. Danach nur noch auf diesem Stand weiterarbeiten
