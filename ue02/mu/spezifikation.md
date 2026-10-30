# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @MelissaUpietz

<!-- Je Abschnitt Ihrer Gliederung eine Überschrift (## für Abschnitte, ###
     für Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten würden.
     Die beiden Überschriften unten sind lediglich Platzhalter. -->

## Die Aufgabe der Software
Die Software soll die Planung und Buchung von Sprechstunden und Prüfungsterminen an der THM vereinfachen.
Die Studierenden sollen freie Sprechstundentermine sehen können und somit auch einen passenden Termin buchen können.

## Benutzer und Anmeldung
Die Software wird von Studierenden, Lehrenden und von Mitarbeitern des Sekreteriats verwendet. 
Man meldet sich über sein Hochschulkonto an. Die studierende Person kann hier die verfügbaren Termine der Lehrenden Person einsehen und buchen.

## Termine buchen
Lehrende können Termine zur Verfügung stellen und Studierende können diese buchen. Zu einem Termin gehören Datum, Uhrzeit, Lehrperson und die Art des Termins (als Liste). Die Termine sollen hier zeitlich geordnet angezeit werden, damit alles übersichtlich ist. Bei der Buchung gibt es ebenfalls ein Feld, wo der Studierende seinen Namen mit Matrikelnummer eingeben muss, damit nochmals überprüft wird, wer den Termin bucht.

## Export und API
Nach der Buchung kann ein Studierender eine iCal-Datei herunterladen und den Termin in seinen eigenen Kalender importieren. Zusätzlich soll es eine API geben, über die bestimmte Aktionen ausgeführt werden können.

## Regeln
Bereits belegte Termine können nicht gebucht werden. Ein KI Agent darf freie Sprechstundentermine suchen und buchen aber keine Prüfungstermine absagen.

## Fehlermeldungen
Es soll getestet werden, ob eine zweite Buchung des selben Termins abgelehnt wird. Wenn nicht kommt es zu einer Fehelermeldung. Das Gleiche passiert wenn kein Name mit Matrikelnummer bei der Buchung eingegeben wird.