# Rollen — Terminplaner für die THM

Mitgearbeitet haben @muxstii

## Der Kunde

| Bereich | Wer ist das an der THM? | Woran machen Sie es fest? |
|---|---|---|
| Fachbereich (eigentlicher Auftraggeber) | Die Hochschulleitung (Vizepräsidium für Studium und Lehre) stellvertretend für Lehrende, Studierende und Sekretariate | Deren Ziel, die Terminvereinbarung zu vereinfachen, soll das Projekt erreichen. Die Hochschulleitung stellt das Budget und trifft die grundsätzlichen Entscheidungen, die Endanwender sitzen in den Fachbereichen. |
| IT-Bereich | Das Hochschulrechenzentrum (HRZ) der THM | Es betreibt das System später und stellt die Systembasis bereit, z.B. die Anmeldung über das Hochschulkonto und die Server. Was das System leisten soll, bestimmt es nicht. |

## Das Projektteam

Vier Personen: A, B, C und D.

| Rolle | Wer |
|---|---|
| Projektmanager | A |
| Projektleiter | B |
| Chefdesigner | C |
| Entwickler | C, B |
| Qualitätsbeauftragter | D |

Diese Rollen haben wir zusammengelegt, da der Chefdesigner die Architektur am besten kennt und sie als Entwickler direkt umsetzen kann. Der Projektleiter entwickelt in einem so kleinen Team zusätzlich mit, damit genug Kapazität für die Implementierung bleibt.

Diese Rollen halten wir getrennt, da der Qualitätsbeauftragte unabhängig prüfen muss: Wer selbst entwickelt, übersieht eher die eigenen Fehler, und unter Termindruck würde die Prüfung zuerst gekürzt. Ebenso trennen wir Projektmanager und Projektleiter, damit Budget und Personal nicht von derselben Person verantwortet werden, die im Alltag die Ergebnisse liefern muss.

## Drei Situationen

| Situation | Wer entscheidet? | Wer muss davon erfahren? |
|---|---|---|
| Ein Sekretariat wünscht sich während der Implementierung zusätzlich eine Raumbuchung. | Der Auftraggeber (Hochschulleitung) entscheidet, ob die Erweiterung beauftragt wird, nachdem der Projektleiter den Aufwand mit dem Chefdesigner abgeschätzt hat. Das Sekretariat allein kann das nicht entscheiden. | Projektmanager (Kosten, Vertrag, Termin), Projektleiter, Team und das Sekretariat |
| Der Systemtest zeigt, dass Benachrichtigungen bei vielen gleichzeitigen Buchungen erst nach Minuten ankommen. | Der Projektleiter entscheidet über die Behebung, der Chefdesigner über die technische Lösung. Ist die Antwortzeit nicht spezifiziert, klärt der Auftraggeber, was akzeptabel ist. | Qualitätsbeauftragter, Entwickler, Projektmanager falls sich der Termin verschiebt, ggf. das HRZ, falls die Ursache in der Infrastruktur liegt |
| Um den Einführungstermin zu halten, braucht das Projekt zwei weitere Entwickler. | Der Projektmanager, denn er stellt Personal und Budget bereit. Der Projektleiter meldet den Bedarf. | Projektleiter und Team, der Auftraggeber, falls sich Kosten oder Vertrag ändern |