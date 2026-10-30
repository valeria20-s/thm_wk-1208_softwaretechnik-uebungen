# Phasenplan — Terminplaner für die THM

Kürzel: skrl78

## Studie

**Ergebnis der Phase:** Studienbericht mit Ausgangslage, Lösungsalternativen und Machbarkeit

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Aufwand schätzen und einen Meilensteinplan vorschlagen

## Systemspezifikation

**Ergebnis der Phase:** Systemspezifikation mit Anforderungen, Daten und Testfällen

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen

## Systemkonstruktion

**Ergebnis der Phase:** Systementwurf mit Komponenten, Schnittstellen und Technologieentscheidungen

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen

## Implementierung

**Ergebnis der Phase:** Implementierte und einzeln getestete Komponenten

- Die Komponente „Benachrichtigung“ programmieren

## Integration & Einführung

**Ergebnis der Phase:** Integriertes, geprüftes und eingeführtes Gesamtsystem

- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen

## Wartung

**Ergebnis der Phase:** Korrigiertes und erweitertes System

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen** (Integration & Einführung): Die Hotline kann zur Integration und Einführung gehören, wenn sie den Anwendern beim Start hilft, oder zur Wartung, wenn sie dauerhaft betrieben wird.
- **Aufwand schätzen und einen Meilensteinplan vorschlagen** (Studie): Die Aufwandsschätzung kann zur Studie gehören, wenn sie der Projektentscheidung dient, oder zur Systemkonstruktion, wenn sie die Umsetzung konkret plant.
- **Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert** (Studie): Der Prototyp kann zur Studie gehören, wenn die technische Machbarkeit geprüft wird, oder zur Systemkonstruktion, wenn eine konkrete technische Lösung erprobt wird.
- **Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten** (Systemkonstruktion): Die Reihenfolge kann zur Systemkonstruktion gehören, wenn die Umsetzung geplant wird, oder zur Studie, wenn zunächst ein grober Projektplan erstellt wird.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=integration k12=konstruktion k23=konstruktion k13=studie k14=spezifikation k15=studie k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k11 k13 k15 k18 -->
