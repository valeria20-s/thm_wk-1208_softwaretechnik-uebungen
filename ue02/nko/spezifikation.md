# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet hat @nyaornela

<!-- Je Abschnitt Ihrer Gliederung eine Überschrift (## für Abschnitte, ###
     für Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten würden.
     Die beiden Überschriften unten sind lediglich Platzhalter. -->

## 1. Zielsetzung
Entwicklung einer Software für die Hochschule zur Planung und Vereinbarung von Terminen. 
 
## 2. Benutzergruppen und Rollen
- **Lehrende** Sie bieten Sprechstunden und Prüfungstermine an.
- **Studierende** Sie Können freie Termine einsehen und diese direkt buchen.
- **Sekretariate** Sie können den Überblick über angebotene und gebuchte Termine behalten.
- **KI-Agenten:** Greifen über eine Programmierschnittstelle (API) auf das System zu, um im Auftrag von Nutzerinnen und Nutzern Termine abzufragen und zu buchen. 

## 3. Funktionale Anforderungen
1. (Terminvereinbarung):** Lehrende legen freie Zeitfenster an, die von Studierenden gebucht werden können.
2. (iCal-Export):** Nach der Buchung stellt das System eine `.ics`-Datei zum Herunterladen bereit, um den Termin in externe Kalender zu importieren.
3. (Übersicht für Sekretariate):** Sekretariate können alle Termine einsehen und verwalten, um den Überblick über Buchungen zu behalten.

## 4. Schnittstellen   
 Anmeldung und Identitätsprüfung erfolgen ausschließlich über das bestehende Hochschulkonto der THM.

## 5. Nicht funktionale Anforderungen
- **Datenschutz:** Alle Daten sind sicher und nach DSGVO geschützt.
- **Nutzungsbedingungen:** Regelt die Nutzung (z. B. Absagefristen) und erfordert Zustimmung bei der Anmeldung.
