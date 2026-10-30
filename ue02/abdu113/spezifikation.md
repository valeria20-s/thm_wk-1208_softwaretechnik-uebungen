# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @abdu113

## 1. Zielbestimmung und Zielgruppen
Erklärung: Das System hilft Studierenden, Lehrenden und Sekretariaten an der THM beim Buchen von Sprechstunden.

Beispiel: Ein Student wählt im Portal einen freien Termin beim Professor aus und bucht diesen direkt.

## 2. Funktionalität und Anwendungsfälle (Use Cases)
Erklärung: Das sind die Aufgaben, die das Programm für den Nutzer erledigen kann.

Beispiel: 
- Termin buchen: Der Nutzer wählt eine Uhrzeit, gibt den Grund an und schickt die Buchung ab.
- iCal-Download: Nach der Buchung kann der Termin als Kalender-Datei heruntergeladen werden.

## 3. Benutzeroberfläche und Benutzerführung
Erklärung: So sieht die Webseite aus und so wird sie bedient.

Beispiel: Freie Termine werden im Kalender grün angezeigt, ausgebuchte grau. Ein Klick auf ein grünes Feld öffnet das Formular.

## 4. Schnittstellen (API & Login)
Erklärung: So verbindet sich das Programm mit dem Hochschulkonto und mit KI-Agenten.

Beispiel: 
- *
Login: Die Anmeldung läuft einfach über das normale THM-Hochschulkonto.
- KI-API: Ein KI-Agent kann über eine Schnittstelle abfragen, welche Termine noch frei sind.

## 5. Nicht-funktionale Anforderungen
Erklärung: Das sind wichtige Regeln für Sicherheit, Datenschutz und Geschwindigkeit.

**Beispiel:** 
- Datenschutz: Nur der Professor und das Sekretariat können sehen, wer den Termin gebucht hat.
- Geschwindigkeit: Die Suche nach freien Terminen darf nicht länger als eine Sekunde dauern.