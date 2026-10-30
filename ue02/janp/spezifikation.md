# Spezifikation des Terminplaners — Gliederung und Beispiele

*Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @vincrusch @IceSand296*


## 1. Allgemein

### 1.1 Ziel
Mit dem Terminplaner sollen Lehrende und Studierende in der Lage sein Termine zu erstellen und zu verwalten.


### 1.2 Benutzer

Studierende können ihre eigenen Termine bearbeiten und löschen, Lehrende können Termine für Studierende erstellen.

| Rechte | Administratoren | Lehrende | Studierende |
| --- | --- | --- | --- |
| Erstellen | Alle | Eigene und für Studierende | Eigene|
| Bearbeiten | Alle | Eigene und für Studierende | Eigene |
| Löschen | Alle | Eigene und für Studierende | Eigene |
| Administratorenrechte| Alle | Keine | Keine |



## 2. Funktionen und Daten

### 2.1 Funktionen

- Termine
    - erstellen
    - anzeigen
    - ändern
    - löschen 
- Zu Terminen zu- und absagen.


### 2.2 Termindaten
Welche Informationen zu jedem Termin gespeichert werden.

Jeder Termin hat: 
- Titel
- Datum Anfang
- Datum Ende
- Uhrzeit Anfang
- Uhrzeit Ende 
- Beschreibung
- ggf. Ort



## 3. Bedienung und Technik

### 3.1 Benutzeroberfläche
Eine klassische Kalenderansicht (Mo - So) mit obiger Navigationsleiste, in der die Funktionen dargestellt werden.


### 3.2 Technische Anforderungen
Terminplaner soll in einem Webbrowser funktionieren. Spätere implementierung als App möglich.



## 4. Sicherheit

### 4.1 Sicherheit
Nutzer könn nur die von ihnen erstellten Termine bearbeiten und löschen, außerdem können sie nur die für sie freigegeben Termine sehen.