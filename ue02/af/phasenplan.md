# Phasenplan — Terminplaner für die THM

Kürzel: af

## Studie

**Ergebnis der Phase:** Lastenheft mit Entscheidung, ob und wie das Projekt umgesetzt wird

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert

## Systemspezifikation

**Ergebnis der Phase:** Pflichtenheft

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden

## Systemkonstruktion

**Ergebnis der Phase:** Systementwurf

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Implementierung

**Ergebnis der Phase:** Getestete Komponenten

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt

## Integration & Einführung

**Ergebnis der Phase:** eingeführtes System

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt

## Wartung

**Ergebnis der Phase:** verbesserte Systemversion

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Datenbank, Programmiersprache und Web-Framework auswählen** (Systemkonstruktion): Konstruktion oder schon in der Studie wegen Kosten? (Die Wahl ist eine technische Entscheidung und gehört deshalb in die Konstruktion. Sie beeinflusst aber auch die Kosten und könnte darum schon in der Studie eine Rolle spielen.)
- **Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen** (Wartung): Einführung (Start) oder Wartung (Dauerbetrieb)? (Die Hotline begleitet den laufenden Betrieb, deshalb Wartung. Sie wird aber meist schon bei der Einführung eingerichtet.)
- **Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert** (Studie): Studie (Machbarkeit) oder Konstruktion (Technik) Ich habe die Karte in die Studie gelegt, weil der Prototyp klären soll, ob das Projekt überhaupt machbar ist. Weil er aber schon technisch ist, könnte er auch zur Systemkonstruktion gehören.
- **Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden** (Systemspezifikation): Welche Daten ausgetauscht werden, ist eine fachliche Frage und gehört damit zur Spezifikation. Wie sie ausgetauscht werden, ist eine technische Frage und gehört zur Konstruktion.
- **Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt** (Integration & Einführung): Es ist ein Test des ganzen Systems und gehört deshalb zur Integration. Unklar ist, ob  Systemtest prüfen oder die THM als Abnahmetest.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=studie k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k09 k11 k15 k19 k24 -->
