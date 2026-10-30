# Phasenplan — Terminplaner für die THM

Kürzel: hams

## Studie

**Ergebnis der Phase:** Gegliedertes Dokument - Lastenheft

- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt

## Systemspezifikation

**Ergebnis der Phase:** Ein Fachkonzept mit : Fachlichen Erläuterungen, Anwendungsfälle, Benutzerschnittstellen, Objektmodell, Nachbarsystemschnittstelle

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen

## Systemkonstruktion

**Ergebnis der Phase:** Technische architektur mit einem fertigen Prototyp und Schnittstellen der Innen- Außensicht Komponenten

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Die Komponente „Benachrichtigung“ programmieren
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen

## Implementierung

**Ergebnis der Phase:** Programmierte und getestete Komponenten. Tests wiederholbar und gegen Schnittstellen entwickelt

- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt

## Integration & Einführung

**Ergebnis der Phase:** Getestetes (Teil-)System

- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen

## Wartung

**Ergebnis der Phase:** Fertiges und laufendes System, dass in Betrieb bleibt.

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen
- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

Keine Karte markiert.

<!-- zuordnung ue02-phasenplan: k01=konstruktion k02=konstruktion k03=wartung k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=studie k14=studie k15=integration k16=integration k17=wartung k18=studie k19=spezifikation k24=implementierung k20=integration k21=implementierung | unsicher: – -->
