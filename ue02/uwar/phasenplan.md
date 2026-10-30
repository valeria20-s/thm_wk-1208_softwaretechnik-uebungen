# Phasenplan — Terminplaner für die THM

Kürzel: uwar

## Studie

**Ergebnis der Phase:** Studie mit Empfehlung und Aufwandsschätzung. Entscheidungsgrundlage, ob und wie das Projekt durchgeführt wird

- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert

## Systemspezifikation

**Ergebnis der Phase:** Fachkonzept (Pflichtenheft) , vollständige fachliche Beschreibung des Systems samt Testfällen

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen

## Systemkonstruktion

**Ergebnis der Phase:** DV-Konzept Komponenten, Schnittstellen und technische Architektur des Systems

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen

## Implementierung

**Ergebnis der Phase:** Programmierte und einzeln getestete Komponenten

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen

## Integration & Einführung

**Ergebnis der Phase:** Abgenommenes und in Betrieb genommenes System beim Auftraggeber

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt

## Wartung

**Ergebnis der Phase:** Gepflegtes System im laufenden Betrieb — Fehler behoben, Erweiterungen eingearbeitet

- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen
- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen** (Systemspezifikation): Spezifikation, weil die Skizzen mit den Anwendern abgestimmt werden und zeigen, WAS das System können soll; für die Konstruktion spräche, dass eine Skizze bereits Gestaltung ist.
- **Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert** (Studie): Studie, weil der Prototyp die technische Machbarkeit für die Entscheidung klären soll; für die Konstruktion spräche, dass hier bereits technisch gearbeitet wird.
- **Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten** (Systemkonstruktion): Konstruktion, weil die Reihenfolge aus den Abhängigkeiten der Komponenten folgt und diese erst dort feststehen; für die Studie spräche, dass Meilensteine zur Projektplanung gehören.
- **Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt** (Integration & Einführung): Integration, weil hier das Gesamtsystem gegen einen echten Anwendungsfall geprüft wird; für die Implementierung spräche, dass es ein technischer Test der eigenen Schnittstelle ist.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=implementierung k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=studie k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k10 k15 k18 k24 -->
