# Phasenplan — Terminplaner für die THM

Kürzel: my55

## Studie

**Ergebnis der Phase:** rahmenbedingungen festgelegt

- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Aufwand schätzen und einen Meilensteinplan vorschlagen

## Systemspezifikation

**Ergebnis der Phase:** fachkonzept vorgelegt

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen

## Systemkonstruktion

**Ergebnis der Phase:** technische konstruktion wie das projekt aufgebaut wird

- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen

## Implementierung

**Ergebnis der Phase:** technischer abcshluss des projekts

- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Die Komponente „Benachrichtigung“ programmieren

## Integration & Einführung

**Ergebnis der Phase:** Livestart des projekts

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung

## Wartung

**Ergebnis der Phase:** Fehlerbehebung

- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

Keine Karte markiert.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=wartung k03=integration k04=spezifikation k05=wartung k22=konstruktion k06=konstruktion k07=implementierung k08=implementierung k09=konstruktion k10=studie k11=spezifikation k12=konstruktion k23=konstruktion k13=studie k14=spezifikation k15=implementierung k16=implementierung k17=wartung k18=konstruktion k19=spezifikation k24=konstruktion k20=implementierung k21=implementierung | unsicher: – -->
