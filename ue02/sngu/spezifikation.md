# Spezifikation: Terminplaner für die THM

**Beteiligte:** sonnyn8

---

## 1. Ausgangslage und Zielsetzung

Die THM benötigt eine zentrale Anwendung zur Terminbuchung zwischen Lehrenden und Studierenden, um E-Mail-Verkehr und Aushänge an Bürotüren abzulösen.

*Beispiel:*
Das System soll Sprechstunden und Prüfungstermine verwalten. Lehrende stellen freie Zeiten bereit, Studierende buchen diese direkt online.

## 2. Zielgruppen und Zugriffsrechte

Die Benutzergruppen der Software sowie deren Berechtigungen im System.

*Beispiel:*
| Rolle | Rechte |
| --- | --- |
| **Studierende** | Freie Termine einsehen, Termine buchen und eigene Buchungen absagen. |
| **Lehrende** | Sprechstunden anlegen, eigene Termine verwalten und Buchungen einsehen. |
| **Sekretariat** | Übersicht über Termine aller Lehrenden des Fachbereichs einsehen. |

## 3. Funktionale Anforderungen

Spezifische Funktionen, die das Entwicklerteam der Hochschule umsetzen muss.

*Beispiel:*
* **Hochschulkonto-Login:** Anmeldung ausschließlich über den zentralen Shibboleth-/SSO-Dienst der THM.
* **iCal-Export:** Generierung einer `.ics`-Datei nach erfolgreicher Buchung für den Import in Kalender-Apps.
* **API-Schnittstelle:** REST-API zur Steuerung der Terminbuchung durch KI-Agenten.

## 4. Nicht-funktionale Anforderungen

Qualitätskriterien, Leistungsvorgaben und gesetzliche Rahmenbedingungen.

*Beispiel:*
* **Datenschutz:** Es dürfen nur notwendige Daten (Name, E-Mail der THM) gespeichert werden; Löschung nach Ablauf des Semesters.
* **Benutzerfreundlichkeit:** Die Benutzeroberfläche muss auf mobilen Endgeräten (Smartphones) ohne Einschränkungen nutzbar sein.

## 5. Benutzeroberfläche und Datenmodell

Musterentwürfe der Seitenstrukturen und benötigte Datenfelder für Entwickler.

*Beispiel:*
Formular *„Sprechstunde anlegen“*:
- Datum (TT.MM.JJJJ)
- Uhrzeit von / bis
- Slot-Dauer (z.B. 15 Minuten)
- Raum / Online-Link
