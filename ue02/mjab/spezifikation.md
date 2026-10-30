# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @mohamedof069

<!-- Je Abschnitt Ihrer Gliederung eine Überschrift (## für Abschnitte, ###
     für Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten würden.
     Die beiden Überschriften unten sind lediglich Platzhalter. -->

## Wer benutzt das System

- Lehrende/Dozenten
- Studierende 
- Sekretariate

## Was will jede Person damit machen?

- Dozenten: bieten Sprechstunden und Prüfungstermine an
- Studierende: buchen Termine 
- Sekretariate: verwalten Termine

## Wie sehen die Bildschrime aus?

Ein Kalender mit angebotenen Terminen, die von Studierenden durch Klicken gebucht werden können. 
Für das Sekretariat ein Kalender als Überblick, welche Termine wo und wann stattfinden.

## Angegebene Daten vom Termin

Raum, Uhrzeit, Anzahl Plätze für Studierende und ob der Termin eine Sprechstunde oder ein Prüfungstermin ist.

*Beispiel:*

| Angabe | Wert |
|---|---|
| Art | Sprechstunde |
| Dozent | Prof. Dr. Lucke |
| Datum und Uhrzeit | Di, 03.11.2026, 15:00-15:30 |
| Raum | A1.0.01 |
| Plätze | 0 von 30 belegt |



## Mit welchen anderen Systeme muss es interagiern?

- Anmeldung über das Hochschulkonto 
- Buchungsbestätigung über die Hochschul-E-mail

## Was darf auf keinen Fall passieren?

- Ein Studierender bucht zwei parallel laufende Termine.
- Dozenten buchen ein schon belegten Raum.

## Woran merkt man, dass das System fertig ist?

- Bestätigungs-E-Mail wird verschickt.
- Die belegten Plätze erhöhen sich, z.B. 8/15 Plätze belegt. 
- Wenn ein Termin voll ist, ist die Buchungstaste nicht ausführbar und es erscheint eine Fehlermeldung.