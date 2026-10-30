# Phasenplan — Terminplaner für die THM

Kürzel: wnga

## Studie

**Ergebnis der Phase:** die Machbarkeit des Projektes. (Steckbrief)

- Aufwand schätzen und einen Meilensteinplan vorschlagen

## Systemspezifikation

**Ergebnis der Phase:** Lasten-und-Pflichtenheft

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen

## Systemkonstruktion

**Ergebnis der Phase:** Architektur der Anwendung

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde

## Implementierung

**Ergebnis der Phase:** das programmierte Software

- Die Komponente „Benachrichtigung“ programmieren

## Integration & Einführung

**Ergebnis der Phase:** Teste und Innenbetriebnahme

- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt

## Wartung

**Ergebnis der Phase:** Verbesserung an der Anwendung

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen** (Systemspezifikation): ich finde die könnte entweder zur Systemspezifikation oder Systemkonstruktion.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=wartung k03=wartung k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=spezifikation k08=integration k09=konstruktion k10=integration k11=spezifikation k12=integration k23=konstruktion k13=studie k14=spezifikation k15=integration k16=integration k17=spezifikation k18=konstruktion k19=spezifikation k24=integration k20=integration k21=konstruktion | unsicher: k22 -->
