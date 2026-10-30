# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben: @sohail143-ofcity

<!-- Je Abschnitt Ihrer Gliederung eine Überschrift (## für Abschnitte, ###
     für Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten würden.
     Die beiden Überschriften unten sind lediglich Platzhalter. -->

# Spezifikation des Terminplaners 

## 1. Ziel des Systems
Die Software soll es Lehrenden und Studierenden erleichtern, Sprechstunden und Prüfungstermine zu vereinbaren. Es darf keine Doppelbuchungen geben.

## 2. Wer nutzt das System?
- **Studierende:** Suchen freie Termine und buchen sie.
- **Lehrende:** Tragen freie Zeiten ein und sehen ihre gebuchten Termine.
- **Sekretariat:** Kann Termine für Lehrende verwalten oder verschieben.

## 3. Wie funktioniert die Buchung?
1. Studierende wählen im System einen Dozenten aus.
2. Ein Kalender zeigt die freien Termine an.
3. Studierende wählen einen Termin aus, tragen ihren Namen und den Grund ein und klicken auf „Buchen“.
4. Beide Seiten bekommen eine Bestätigung.

## 4. Aussehen der Seite
Oben gibt es ein Suchfeld für Dozenten. Darunter wird die Woche als Tabelle angezeigt. Freie Termine sind grün, besetzte grau.

## 5. Schnittstellen & Technik
- Das System muss sich mit dem Hochschulkonto zum Login verbinden.
- Gebuchte Termine sollen als `.ics`-Datei für Outlook/Apple Kalender exportiert werden können.
