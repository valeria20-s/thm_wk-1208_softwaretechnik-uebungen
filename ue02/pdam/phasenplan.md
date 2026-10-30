# Phasenplan — Terminplaner für die THM

Kürzel: pdam

## Studie

**Ergebnis der Phase:** Lastenheft

- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert

## Systemspezifikation

**Ergebnis der Phase:** Pflichtenheft

- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden

## Systemkonstruktion

**Ergebnis der Phase:** Softwareentwurf

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen

## Implementierung

**Ergebnis der Phase:** Programmcode

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt

## Integration & Einführung

**Ergebnis der Phase:** Einsatzbereites Gesamtsystem

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen

## Wartung

**Ergebnis der Phase:** Gewartete und weiterentwickelte Software

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen** (Integration & Einführung): Ich habe dies der Systemspezifikation zugeordnet, weil festgelegt wird was das System fachlich erlauben soll. Man kann es aber auch der System Systemkonstruktion zuordnen.
- **Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen** (Integration & Einführung): Ich habe sie der Integration zugeordnet statt der der Wartung, da die Hotline zu Beginn zur Verfügung steht
- **Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt** (Implementierung): Ich habe es eher der Implementierung statt der Integration zugeordnet, da das komplette System erst getestet werden muss bevor es zusammengeführt wird
- **Aufwand schätzen und einen Meilensteinplan vorschlagen** (Studie): Ich habe dies in der Studie zugeordnet, da sie die Machbarkeit und den Umfang des Projekts festlegt. Man könnte es aber auch der Systemkonstruktion zuordnen
- **Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert** (Studie): Ich habe mich hier ebenfalls für die Studie anstatt der Implementierung entschieden, weil damit früh die technische Machbarkeit geprüft wird
- **Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt** (Integration & Einführung): Ich habe den Probebetrieb eher der Integration statt der Wartung zugeordnet, da es vor den vollständigen Nutzen erprobt wird

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=integration k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=integration k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=studie k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k22 k11 k12 k13 k15 k20 -->
