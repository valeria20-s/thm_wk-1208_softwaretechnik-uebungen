# Phasenplan — Terminplaner für die THM

Kürzel: fortnitepro

## Studie

**Ergebnis der Phase:** …

- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert

## Systemspezifikation

**Ergebnis der Phase:** …

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen

## Systemkonstruktion

**Ergebnis der Phase:** …

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Implementierung

**Ergebnis der Phase:** …

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt

## Integration & Einführung

**Ergebnis der Phase:** …

- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt

## Wartung

**Ergebnis der Phase:** …

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen** (Systemspezifikation): Systemspezifikation, aber nicht sicher
- **Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen** (Systemspezifikation): Systemspezifikation, aber nicht sicher
- **Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen** (Integration & Einführung): Integration & Einführung, aber nicht sicher
- **Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten** (Systemkonstruktion): Systemkonstruktion, aber nicht sicher
- **Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden** (Systemspezifikation): Systemspezifikation, aber nicht sicher
- **Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt** (Integration & Einführung): Integration & Einführung, aber nicht sicher
- **Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt** (Integration & Einführung): Integration & Einführung, aber nicht sicher

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=integration k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=studie k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k10 k14 k16 k18 k19 k24 k20 -->
