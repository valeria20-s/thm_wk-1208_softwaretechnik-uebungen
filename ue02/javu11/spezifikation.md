# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): 
> javu11

## Zielgruppendefinition
- Lehrende
- Schüler
- Sekreteriat

## Zielbild definieren
### Was gehört in einen Termin?
1. Datum
1. Raumzuordnung
1. Buchende Person
1. Lehrende Person
1. ....

### UX Spezifikationen
1. Grüne Akzente für die Farbe der THM
1. Einheitliche Schrift wie aus der Website
1. ....

## As-is Prozess
> Modellierung ggf. mithilfe eines BPMN Modells

### Lehrende
- Manuelle Terminvergabe über Mail, physischen Listen...
### Schüler
- Terminbuchung aktuell über Mail, physischen Listen, Netzwerkzeuge
### Sekreteriat
- s.o.

## To-be Prozess
### Lehrende
- Sprechstundeneingabe/ Verwaltung von Terminen der Lehrenden
### Schüler
- Der Termin soll zukünftig nur noch auf einem System gebucht werden
- Eingabe von folgenden Infos benötigt:
     - Matrikelnummer
     - Vor-& Nachname
### Sekreteriat
- Fungiert als Verwaltungs- & Kontrollinstanz
- Benötigt Zugriff auf alle Kalender


## Integration in bestehende Systemlandschaft
- Welche Systeme gibt es?
     - Website
     - Netzwerkzeuge
     - E-Mail
     - Cloud/ Datenbanken der THM
- Welche Schnittstellen werden benötigt (API's)?
     - Kalendar der Lehrenden
     - KI Agenten
- Welche Systeme werden abegschafft?
     - Systeme bleiben bestehen, wobei die Terminbuchung nur noch üer die Software läuft

## Einsatz von KI Agenten
- Rolle von KI
- Welche prozese sollen mit KI gesteuert werden? Welche nicht?
- Welhe technischen Voraussetzungen muss das system erfüllen?

## Zeitlicher Rahmen
Der Terminplanner soll für das kommende Sommersemester eingesetzt werden. Ein erster Entwurf für einen Test soll für den Fachbereich MND in 3 Monaten verfügbar sein.
