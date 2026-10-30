# Phasenplan — Terminplaner für die THM

Kürzel: qho

## Studie

**Ergebnis der Phase:** Machbarkeitsstudie mit Projektvorschlag

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen

## Systemspezifikation

**Ergebnis der Phase:** Spezifikationen der Anordnung

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Systemkonstruktion

**Ergebnis der Phase:** Technischer Systementwurf

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Datenbank, Programmiersprache und Web-Framework auswählen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen

## Implementierung

**Ergebnis der Phase:** Programmierte Komponenten

- Die Komponente „Benachrichtigung“ programmieren
- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen

## Integration & Einführung

**Ergebnis der Phase:** Getestet und eingeführtes System

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt

## Wartung

**Ergebnis der Phase:** Gewartetes und weiterentwickeltes System

- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

Keine Karte markiert.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=konstruktion k03=implementierung k04=spezifikation k05=integration k22=spezifikation k06=studie k07=spezifikation k08=integration k09=konstruktion k10=spezifikation k11=konstruktion k12=implementierung k23=implementierung k13=spezifikation k14=spezifikation k15=konstruktion k16=integration k17=konstruktion k18=spezifikation k19=spezifikation k24=integration k20=wartung k21=wartung | unsicher: – -->
