# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben: @ttpr21

## 1. Welche Funktionen gibt es?
Zusammenfassung aller Funktionen:
| Funktion | Wer? | Was soll passieren? |
|---|---|---|
| Login | Alle | Anmeldung beim Terminplaner |
| Buchung eines Sprechstundentermins | Studierende | Studierende sollen Sprechstunden beim Lehrenden buchen können |
| Buchung eines Prüfungstermins | Studierende | Studierende müssen sich bei Prüfungen anmelden können |
| Form der Bereitstellung der Termine | Studierende | als iCal-Datei |

### 1.1 Login
Beispiel:
- es wird sich über die Hochschulemail eingeloggt
- es muss die Hochschulemail angegeben werden und im nächsten Feld das Passwort

### 1.2 Buchung eines Sprechstundentermins
Beispiel:
- jeder Lehrende hat einen öffentlichen Kalender
- Studierende können diesen einsehen und Termine buchen
- das Sekretariat kann Termine verschieben und behält den Überblick
- wurde ein Slot gebucht verschwindet er - beide Gesprächspartner sollen eine Nachricht erhalten
- es soll möglich sein, einen Termin zu verschieben oder abzusagen per Klick, der Slot soll dann automatisch wieder frei werden

### 1.3 Buchung eines Prüfungstermins
Beispiel:
- Studierende bekommen eine Nachricht, wenn sie sich für eine Klausur anmelden
- der Lehrende kann eine maximale Anzahl an Prüflingen festlegen
- nur der Lehrende kann sehen wer sich angemeldet hat

### 1.4 Bereitstellung der Termine 
Beispiel:
- als iCal-Datei zum Herunterladen bereit


## 2. Wie soll die UI aussehen? 
Beispiel:
- Demo Version damit das Frontend eine Idee hat, wie die Anwendung am Ende aussehen soll, rot = besetzt & grün Stunde ist verfügbar

### 2.1 Bedienoberflächen
Beispiel:
- Mockup für Login, Buchung eines Sprechstundentermins & Buchung eines Prüfungstermins

## 3. Woher werden die Daten bezogen für bspw. Prüfungstermine? 
Beispiel:
- es werden Nachbarsysteme benötigt, z.B. der Hochschulkalender für die Prüfungstermine

## 4. Schnittstellen
Beispiel:
- KI Agenten sollen sich darüber steuern lassen z.B. zur Erstellung von Terminen