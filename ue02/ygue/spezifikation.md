# Spezifikation Terminplaner

* Beteiligte: @52yuyu

## 1. Ziel und Zweck
Das System soll Studierenden und Lehrenden der THM ermöglichen, Sprechstunden- und Prüfungstermine digital zu vereinbaren und zu verwalten.

## 2. Zielgruppen & Akteure
* **Studierende**: Suchen und buchen Termine.
* **Lehrende**: Bieten freie Zeitslots an und verwalten Anfragen.
* **Sekretariat**: Verwaltet Ausnahmeregelungen und Raumzuweisungen.

## 3. Funktionale Anforderungen
| Funktion | Beschreibung | Priorität |
| :--- | :--- | :--- |
| Terminbuchung | Studierende wählen freie Zeitslots im Kalender aus. | Hoch |
| KI-Agent | Bucht Termine automatisch über eine REST-API. | Mittel |
| E-Mail-Benachrichtigung | Sendet Bestätigungen und Erinnerungen an Beteiligte. | Hoch |

## 4. Nicht-funktionale Anforderungen
* **Sicherheit**: Die Authentifizierung erfolgt zwingend über das Hochschulkonto (SSO).
* **Verfügbarkeit**: Das System muss auch zu Stoßzeiten (z. B. Prüfungsanmeldung) stabil erreichbar sein.
