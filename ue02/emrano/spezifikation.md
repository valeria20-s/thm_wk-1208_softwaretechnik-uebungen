# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben: @nicmar-29, @KiruTiger, @EmranAliz


## Deadline
### Beispiele:
01.12.2026, 23:59 Uhr

## Ziel 
Software zur Planung und Vereinbarung von Termine
###  Inhalt:
- effiziente Terminplanung
- Termine anlegen und verwalten

###  Beispiele:
|Name|Datum|Uhrzeit| Anliegen|Lehrer|
|---|---|---|---|---|
|Kiruthiga|31.10.2026| 14 Uhr|Klausureinsicht |Lucke|
|...|...|...|...|...| 

## Funktion und Rahmenbedingung
### Inhalt:
- Anforderungen an ein funktionierendes System
### Beispiele:
- Lehrer legen Termine fest
- Schüler buchen Termine
- Nur Lehrer können Termine anlegen

## Benutzer und Benutzerrechte
### Inhalt:
- User 
- Admin
### Beispiele:
- Lehrende bieten Sprechstunden und Prüfungstermine an (Admins)
- Studierende buchen die Termine (User)
- Sekretariate behalten den Überblick (Admin)

## Daten
### Inhalt:
- Daten von allen Terminen
- Daten von User und Admin
### Beispiele:
 |Datentyp| Beispiel |
 |---| ---|
 |Titel| Klausurtermin|
 |Datum| 15.11.2026|
 |Uhrzeit| 14 Uhr|
 |Ort| Stadthalle|
 |User| Name|
 |Admin|Name|

## Test
### Inhalt:
- Abnahme- und Systemtests zur Sicherstellung der Funktionen 
### Beispiele:
- JUnit
- Sicherstellung, dass Termine buchbar sind