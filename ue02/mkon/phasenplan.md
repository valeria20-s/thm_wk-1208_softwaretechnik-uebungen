# Phasenplan — Terminplaner für die THM

Kürzel: mkon

## Studie

**Ergebnis der Phase:** Am Ende liegt ein Lastenheft vor.

- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Systemspezifikation

**Ergebnis der Phase:** Am Ende liegt ein Fachkonzept vor.

- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen

## Systemkonstruktion

**Ergebnis der Phase:** Am Ende liegt eine Beschreibung der späteren Systembestandteile und deren Zusammenspiel vor.

- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert

## Implementierung

**Ergebnis der Phase:** Komponenten, die programmiert und getestet wurden.

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt

## Integration & Einführung

**Ergebnis der Phase:** Ein getestetes Gesamtsystem, mit einem  Fehlerprotokoll.

- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung

## Wartung

**Ergebnis der Phase:** Am Ende liegt ein von Fehlern bereinigtes, technisch angepasstes und um neue Funktionen erweitertes System vor.

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt** (Implementierung): Ich war mir unsicher, ob diese Karte eher zur Phase Integration gehört, da dies die Phase des Testens ist, aber hier wird eine einzelne Komponente getestet, welches zur Implementierung zugeordnet wird.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=konstruktion k16=integration k17=wartung k18=studie k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k12 -->
