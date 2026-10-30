# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben: @nicmar-29, @KiruTiger, @EmranAliz


## Deadline
### Beispiel:
01.12.2026 23:59Uhr 


## Ziel 
### Inhalt :
- effiziente Terminplanung
- Terime anlegen und verwalten 
### Beispiel : 
| Name | Datum| Uhrzeit | Anliegen | Lehrer |
|---|---|---|---|---|
| Kiruthiga | 31.10.2026 | 14 Uhr | Klausureinsicht | Lucke |
|...|...|...|...|...|


## Funktionen und Rahmenbedingungen 
### Inhalt : 
Anforderungen an ein funktionierndes System
### Beispiel:
- Lehrer legen die Termine fest
- Schüler buchen Termine 
- Nur Lehrer können Termine anlegen


## Benutzer und Benutzerrechte 
### Inhalt :
- User
- Admin
### Beispiel
- Lehrende bieten Sprechstunden und Prüfungstermine an (Admin)
- Studierende buchen die Termine (User)
- Sekretariat behalten den Überblick (Admin)

## Daten 
### Inhalt :
- Daten von allen Terminen
- Daten von User und Admin

### Beispiel:
| Datentyp | Beispiel |
|---|---|
| Titel | Klausurtermin |
| Datum | 15.11.2026 |
| Uhrzeit | 8:00 |
| Ort | Stadthalle |
| User | Name |
| Admin | Name |

## Test
### Inhalt :
- Abnahme- und Systemtests zur Sicherstellung der Funktionen
### Beispiel:
- JUnit
- Sicherstellung, dass Termine buchbar sind
