# Rollen — Terminplaner für die THM

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @antoniogub3

## Der Kunde

| Bereich | Wer ist das an der THM? | Woran machen Sie es fest? |
|---|---|---|
| Fachbereich (eigentlicher Auftraggeber) | Lehrende und Sekretariate des Fachbereichs | Sie bieten die Termine an und haben das Problem, das der Terminplaner löst. |
| IT-Bereich | Das Rechenzentrum der THM | Es betreibt das Hochschulkonto und das Kalendersystem, an die der Terminplaner angebunden wird. |

## Das Projektteam

Vier Personen: A, B, C und D.

| Rolle | Wer |
|---|---|
| Projektmanager | A |
| Projektleiter | A |
| Chefdesigner | B |
| Entwickler | C |
| Qualitätsbeauftragter | D |

Diese Rollen haben wir zusammengelegt: Projektmanager und Projektleiter (A), da bei einem Team von vier Personen Kundenkontakt, Planung und Steuerung nicht auf zwei Personen verteilt werden müssen.

Diese Rollen halten wir getrennt: Entwickler und Qualitätsbeauftragter, da wer etwas baut, es nicht selbst prüfen sollte. Außerdem Chefdesigner und Entwickler, damit der Entwurf unabhängig von der Umsetzung bewertet wird.

## Drei Situationen

| Situation | Wer entscheidet? | Wer muss davon erfahren? |
|---|---|---|
| Ein Sekretariat wünscht sich während der Implementierung zusätzlich eine Raumbuchung. | Projektmanager (A), da es Umfang und Kosten ändert, nach Rücksprache mit dem Kunden | Kunde, Chefdesigner, Entwickler, Qualitätsbeauftragter |
| Der Systemtest zeigt, dass Benachrichtigungen bei vielen gleichzeitigen Buchungen erst nach Minuten ankommen. | Chefdesigner (B), da es um den Entwurf geht, gemeinsam mit dem Projektleiter (A) | Entwickler, Qualitätsbeauftragter, Projektmanager; der Kunde nur, wenn sich der Termin verschiebt |
| Um den Einführungstermin zu halten, braucht das Projekt zwei weitere Entwickler. | Projektmanager (A), da es um Budget und Personal geht | Kunde, Entwickler, Chefdesigner, Qualitätsbeauftragter |