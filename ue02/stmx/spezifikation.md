# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): **@sinanmsallem**

<!-- Je Abschnitt Ihrer Gliederung eine Überschrift (## für Abschnitte, ###
     für Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten würden.
     Die beiden Überschriften unten sind lediglich Platzhalter. -->

## 1. Einleitung und Zielsetzung
- Das System ersetzt E-Mails und Aushänge an der Hochschule durch eine Software zur Planung und Vereinbarung von Terminen wie Sprechstunden oder Prüfungsterminen.

## 2. Anforderungen
> Die neue Software soll über das Hochschulkonto bedienbar sein. In einer ersten Ausbaustufe stellt sie Termine als iCal-Datei bereit; eine Integration in den Kalender der Beteiligten kann später folgen.


### 2.1 Akteure
| Rolle | Beschreibung|
|---|---|
| Lehrende | Bieten Sprechstunden und Prüfungstermine an |
| Studierende | Können angebotene Termine buchen oder absagen |
| Sekreteriate| Verwalten Termine / behalten Überblick |


### 2.2 Benutzeroberfläche
**Die Benutzeroberfläche soll folgende Punkte unbedingt aufweisen:**
1. Anmeldung über Hochschulkonto
2. Schaltflächen zur Buchung/Absage eines Termins
3. Übersicht über bereits bestehende Termine mit Datum, Uhrzeit und gegebenfalls Raum

