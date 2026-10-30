# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @B103481187342


## Geschäftsprozesse 
Lehrende bieten freie Sprechstundentermine an. Studierende können diese buchen. Das Sekretariat behält den Überblick über die Buchungen.

## Anwendungsfälle 

### Sprechstunde buchen 
1. Ein Studierender meldet sich mit seinem Hochschulkonto an.
2. Er wählt eine Lehrperson und einen freien Termin aus.
3. Das System speichert die Buchung und zeigt eine Bestätigung an.

## Benutzerschnittstelle 
Auf der Buchungsseite können Studierende eine Lehrperson auswählen und die verfügbaren Termine sehen. Über eine Schaltfläche können sie einen freien Termin buchen.

## Objektmodell
Ein Termin hat ein Datum, eine Uhrzeit und gehört zu einer Lehrperson. Ein Studierender kann einen freien Termin buchen. Zu einem Termin kann auch ein Raum gehören.

## Nachbarsysteme und Schnittstellen 
Die Anmeldung erfolgt über das Hochschulkonto. Termine sollen als iCal-Datei heruntergeladen werden können. Außerdem ist eine API vorgesehen, über die KI-Agenten Termine buchen können.
  