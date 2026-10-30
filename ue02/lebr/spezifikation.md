# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @leiak24


## Funktionalität des Systems 
1. Lehrkräfte bieten Termine an 
2. Studierende können diese auf Wunsch buchen
3. Termin erscheint im Kalneder der Studierende 

## Nutzergruppe

| Gruppe | Was sie im System tut |
| --- | --- |
| Studierende | Buchen sich eigenständig angebotene Termine |
| Lehrkräfte | Bieten buchbare Termine an |
| Sekretariat | Behält alle Planungen im Überblick |



## Bedienung des Systems 

Die Bedienung des Systems erfolgt über das Hochschulkonto, wo Lehrende ihre Termine anbieten und Studierende sich so ihren Wunschtermin buchen können. Auf dem Hochschulkonto gibt es einen Abschnitt "Sprechstunden" wo der jeweilige Name des Lehrenden mit jeweils einem Drop-down-Menü der verfügbaren Uhrzeiten steht.

## Vorgaben und Schnittstellen

Die Termine sollen als **iCal-Datei** heruntergeladen werden können und später zum persönlichen Kalender hinzugefügt werden. Eine API sollte auch vorhanden sein, damit KI-Agenten mitsteuern können. Nachdem ein Termin gebucht wurde wird im Kalender angeziegt welche Termine im Konflikt zueinander stehen können und ob der Termin final gebucht werden soll, beim Akzeptieren wird der Termin automatisch gebucht.

## Erreichen des Ziels 

Die Fertigstellung des Systems gilt als abgeschlossen,wenn: 

- ohne Probleme Termine gebucht werden können
- die gebuchten Termine im Kalender der Studierenden angezeigt werden  
- das System brauchbar und benutzt wird 