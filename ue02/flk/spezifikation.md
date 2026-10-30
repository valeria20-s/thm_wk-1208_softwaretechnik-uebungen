# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): [@Falkitop](https://github.com/Falkitop) [@LemonTiger1992](https://github.com/LemonTiger1992)

## Der Fall

Die Hochschule möchte eine Software zur Planung und Vereinbarung von Terminen: Lehrende bieten Sprechstunden und Prüfungstermine an, Studierende buchen sie, und die Sekretariate behalten den Überblick.

## IST-Zustand
Bisher erfolgt die Vereinbarung per E-Mail, über Listen an der Bürotür oder mit Werkzeugen wie dem DFN-Terminplaner oder Doodle.

## SOLL-Zustand
Die neue Software soll über das Hochschulkonto bedienbar sein. In einer ersten Ausbaustufe stellt sie Termine als iCal-Datei zum Herunterladen bereit; eine Integration in die Kalender der Beteiligten kann später folgen. Zudem soll das System eine Programmierschnittstelle (i.e., eine API) erhalten, über welche es sich auch durch KI-Agenten steuern lässt.

### Generelle Anforderungen
* **Kommollitonen:** Termine buchen...
* **Professoren:** Temrine zur Verfügung stellen...
* **Sekretariat:** Übersicht von Terminen...


### Wie soll es aussehen
* **Kommollitonen:** Übersicht Tabelle der Profs...
* **Professoren:** Übersicht ihrer Termine und Belegungen...
* **Sekretariat:** Übersicht aller Termine und Belegungen der Profs...

## Erweitbarkeit
Ein Kalender soll später hinzugefügt werden können...