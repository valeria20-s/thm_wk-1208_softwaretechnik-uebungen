# Spezifikation: Terminplaner für die THM

Mitarbeit: antoniogub3

## 1. Ziel und Abgrenzung

Der Terminplaner vereinbart Sprechstunden- und Prüfungstermine zwischen Lehrenden, Studierenden und Sekretariaten. Nicht enthalten: Raumverwaltung der gesamten Hochschule.

## 2. Beteiligte und Rollen

| Rolle | Darf |
|---|---|
| Studierende | Freie Termine sehen und buchen |
| Lehrende | Termine anbieten und verwalten |
| Sekretariat | Alle Termine einsehen |

## 3. Anmeldung

Die Anmeldung erfolgt über das Hochschulkonto. Beispiel: Wer nicht angemeldet ist, sieht keine Termine.

## 4. Terminbuchung

Ablauf: Studierende wählen Lehrende, sehen freie Zeiten, buchen einen Termin und erhalten eine Bestätigung.

## 5. Terminverwaltung

Lehrende legen Termine an, ändern oder sagen sie ab. Beispiel: Ein gebuchter Termin kann nur mit Benachrichtigung der Studierenden abgesagt werden.

## 6. Benachrichtigungen

Beispiel: Bei jeder Buchung oder Absage geht eine Nachricht an die Beteiligten.

## 7. Kalender-Export

Termine werden als iCal-Datei zum Herunterladen angeboten. Später optional direkter Eintrag in die Kalender.

## 8. API für KI-Agenten

Beispiel: Ein KI-Agent darf freie Termine abfragen und buchen, aber keine Prüfungstermine absagen.

## 9. Datenmodell

Beispiel: Ein Termin gehört zu genau einer lehrenden Person, einer Person als Teilnehmer und einem Raum.

## 10. Nicht-funktionale Anforderungen

Beispiel: Die Buchungsseite lädt in unter 2 Sekunden und ist auf dem Handy bedienbar.

## 11. Testfälle und Abnahme

Beispiel: Ein Doppelbuchungsversuch desselben Termins wird abgelehnt.

## 12. Offene Punkte

Beispiel: Bis wann das System eingeführt sein soll, klärt die THM.