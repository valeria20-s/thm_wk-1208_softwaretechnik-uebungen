# Phasenplan — Terminplaner für die THM

Kürzel: flk

## Studie

**Ergebnis der Phase:** Informationsgewinn der Umgebung

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Aufwand schätzen und einen Meilensteinplan vorschlagen

## Systemspezifikation

**Ergebnis der Phase:** …

- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Systemkonstruktion

**Ergebnis der Phase:** …

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen

## Implementierung

**Ergebnis der Phase:** …

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Integration & Einführung

**Ergebnis der Phase:** …

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen

## Wartung

**Ergebnis der Phase:** …

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen** (Systemkonstruktion): Ich war mir unsicher: Eselsbrücke -> [...]spezifikation -> Wie es (am Ende) aussehen soll. [...]konstruktion ->  Wie es implementiert werden soll
- **Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt** (Implementierung): Bevor es Integriert und Eingefürt wird, sollte man es in einer sicheren Umgebung testen. (Test before Production)

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=konstruktion k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=studie k11=wartung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=integration k16=integration k17=wartung k18=spezifikation k19=konstruktion k24=integration k20=implementierung k21=integration | unsicher: k06 k12 -->
