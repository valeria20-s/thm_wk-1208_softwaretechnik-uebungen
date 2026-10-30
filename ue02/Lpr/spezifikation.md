# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @LorenzPrz

## 1. Ziel
Was soll der Terminplaner alles können?

Beispiel:
Studenten soll es erleichtert werden, Termine bei Dozente Online zu buchen, ohne dabei Emails hin und her zu schicken. 
> Hinweis: Es soll zwischen Prüfungs- und Sprechstundenterminen unterschieden werden können.

## 2. Funktionen des Terminplaners
Was muss das Programm alles können?
### 2.1 Fuktionen für Studenten
Beispiel:
- Filtern von freien Sprechstunden und Klausurterminen eines Dozenten
- Einen freien Termin buchen könne
- Eine gebuchte Sprechstunde stornieren können (z.B. 24 oder 48 Stunden vorher).

### 2.2 Funktionen für Dozenten
Beispiel:
- Zeitfenster für Sprechstunden oder Klausurtermine anlegen.
- Eine Übersicht aller gebuchten Termine einsehen könne
- Termine absagen, falls etwas unerwartetes passiert, der Student wird dann informiert.

## 3. Zeitfenster und Terminarten
Wann können Termine überhaupt stattfinden und welche Arten gibt es?

Beispiel: 
Termine gibt es in der Regel nur montags bis freitags von 8:00 bis 18:50 Uhr.
- Sprechstundentermin: Ein Gesrpäch zwischen Student und Dozent max. 45min.
- Prüfungstermin: Dauer und Datum wird von Dozent festgelegt

## 4. Benötigte Daten für eine Buchung
Welche Daten müssen bei einer Buchung angegeben werden?

Beispiel:
| Vorname | Nachname | MatrikelNr | Grund | Modul | 
|---|---|---|---|---|
| -blank- | -blank- | -blank- | -blank- | -blank- |

## 5. Benutzerobberfläche
Wie soll der Terminplaner aussehen?

### 5.1 Kalender
Beispiel: 
- Es gibt ein Suchfeld für den Dozenten und eine Klausur.
- Wenn man nach einem Dozenten sucht werden alle noch freien Sprechstunden grün angezeigt, vergebene werden ausgeblendet und Klausurtermine rot angezeigt.
- Wenn man nach einer Klausur sucht, wird nur die Klausur angezeigt mit bestimmter Bezeichnung.

### 5.2 Buchungsansicht
Beispiel:
Klickt man auf einen freien Termin öffnet sich ein kleines Fenster dort füllt man eine Tabelle oder Formular mit allen nötigen Daten aus und bestätigt die Buchung mit einem Buttton.