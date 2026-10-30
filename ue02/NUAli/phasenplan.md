# Phasenplan — Terminplaner für die THM

Kürzel: NUAli

## Studie

**Ergebnis der Phase:** Wie das Projekt umgesetzt werden soll.

- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Systemspezifikation

**Ergebnis der Phase:** Alle Anforderungen des Systems

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden

## Systemkonstruktion

**Ergebnis der Phase:** Technischer Entwurf

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen

## Implementierung

**Ergebnis der Phase:** Programmier Software.

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt

## Integration & Einführung

**Ergebnis der Phase:** Getestete und eingeführtes System.

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen

## Wartung

**Ergebnis der Phase:** Fehlerbehebungen und updates.

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten** (Studie): Nicht sicher, ob es zu Studie oder zur Systemkonstruktion gehört.
- **Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen** (Integration & Einführung): Wäre da nicht auch in Wartung?

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=konstruktion k11=implementierung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=implementierung k16=integration k17=spezifikation k18=konstruktion k19=spezifikation k24=implementierung k20=studie k21=spezifikation | unsicher: k02 k08 -->
