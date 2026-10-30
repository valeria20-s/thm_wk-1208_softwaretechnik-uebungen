# Phasenplan — Terminplaner für die THM

Kürzel: dszp

## Studie

**Ergebnis der Phase:** …

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen

## Systemspezifikation

**Ergebnis der Phase:** …

- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Systemkonstruktion

**Ergebnis der Phase:** …

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Implementierung

**Ergebnis der Phase:** …

- Die Komponente „Benachrichtigung“ programmieren
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt

## Integration & Einführung

**Ergebnis der Phase:** …

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen

## Wartung

**Ergebnis der Phase:** …

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

Keine Karte markiert.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=konstruktion k05=wartung k22=implementierung k06=konstruktion k07=studie k08=integration k09=konstruktion k10=studie k11=wartung k12=spezifikation k23=spezifikation k13=studie k14=spezifikation k15=integration k16=integration k17=spezifikation k18=konstruktion k19=studie k24=implementierung k20=integration k21=integration | unsicher: – -->
