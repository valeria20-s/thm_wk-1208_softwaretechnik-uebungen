<!-- GitHub-Benutzername: masalabyte -->

# Entwurf zur Systemspezifikation: THM Terminplaner

## 1. Ausgangssituation und Ziel
Das System soll die Terminvereinbarung an der THM digitalisieren.
* **Beispiel:** Studierende buchen Sprechstunden künftig über Hochschul -LogIn statt per Zettel an der Bürotür.

## 2. Benutzer und Rollen
Wer bedient das System?
* **Beispiel:** Lehrende legen freie Zeiten an; Studierende können  diese Zeiten buchen.

## 3. Kernfunktionen
Was muss das System können?
* **Beispiel:** Nach einer Buchung wird automatisch eine `.ics`-Kalenderdatei für den Download erzeugt.

## 4. Schnittstellen
Die Anbindung an andere Systeme.
* **Beispiel:** Eine REST-API (`/api/slots`), über die KI-Agenten freie Termine automatisiert abfragen können.

## 5. Qualität und Rahmenbedingungen
Wichtige Vorgaben für den Betrieb.
* **Beispiel:** Der LogIn erfolgt über das Hochschulkonto der THM.