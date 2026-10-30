# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @Doederich

## 1. Ziel und Abgrenzung

Der Terminplaner soll Sprechstunden und Prüfungstermine an der THM an einer
Stelle bündeln, statt per E-Mail, Türlisten oder Doodle. Zuerst gibt es nur
den iCal-Download, die Kalenderanbindung kommt später.

## 2. Begriffe

- **Terminangebot:** ein freier Zeitraum, den eine lehrende Person anbietet
- **Buchung:** ein Terminangebot, das eine studierende Person reserviert hat

## 3. Nutzergruppen

| Gruppe | Was sie darf |
|---|---|
| Lehrende | Termine anbieten, ändern, löschen |
| Studierende | Termine ansehen, buchen, absagen |
| Sekretariat | Termine der Lehrenden einsehen |
| KI-Agenten | Aufgaben für eine Person erledigen, aber nur mit deren Rechten |

## 4. Funktionen

Als Studentin oder Student möchte ich einen freien Termin in der Sprechstunde
von Prof. X buchen, damit ich sicher einen Platz habe.

Anforderung F1: Ein Termin darf nicht doppelt gebucht werden können.

## 5. Daten

Terminangebot: Lehrende Person, Art, Start, Ende, Anzahl Plätze
Buchung: Terminangebot, studierende Person, Status (gebucht / abgesagt)

## 6. Oberfläche

Skizze: Eine Wochenübersicht mit freien Terminen als Kacheln. Wenn man auf
eine Kachel klickt, öffnet sich ein Fenster mit dem Button „Buchen“.

## 7. Schnittstellen

- Anmeldung über das Hochschulkonto
- iCal: Download einer .ics-Datei mit Titel, Start, Ende und Ort
- API für KI-Agenten

## 8. Qualität und Abnahme

Anforderung: Die Terminliste soll auch bei vielen gleichzeitigen Nutzern in
unter 2 Sekunden laden.

Abnahmetest: Ist ein Termin mit einem Platz schon gebucht und versucht eine
zweite Person ihn zu buchen, wird das abgelehnt und es werden andere freie
Termine vorgeschlagen.

Noch offen: Dürfen Sekretariate für Lehrende Termine buchen oder absagen?