# Phasenplan — Terminplaner für die THM

Kürzel: snab

## Studie

**Ergebnis der Phase:** Machbarkeitsnachweis, Kosten-Nutzen-Analyse und eine Entscheidung über den Projektstart.

- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten

## Systemspezifikation

**Ergebnis der Phase:** Ein vollständiges Pflichtenheft.

- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt

## Systemkonstruktion

**Ergebnis der Phase:** Ein Software-Architekturkonzept.

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen

## Implementierung

**Ergebnis der Phase:** Fertig programmierter Quellcode und getestete Einzelkomponenten.

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde

## Integration & Einführung

**Ergebnis der Phase:** Ein vollständiges Gesamtsystem im Live-Betrieb.

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen

## Wartung

**Ergebnis der Phase:** Ein laufendes und angepasstes System.

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen** (Integration & Einführung): Abgewogen zwischen Systemspezifikation und Integration & Einführung, weil ich nicht genau verstanden habe, ob es hier um das UI geht oder um die Einführung für die Studierenden.
- **Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde** (Implementierung): Abgewogen zwischen Konstruktion und Implementierung.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=integration k05=wartung k22=spezifikation k06=konstruktion k07=spezifikation k08=integration k09=konstruktion k10=integration k11=spezifikation k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=integration k16=integration k17=wartung k18=studie k19=studie k24=integration k20=integration k21=implementierung | unsicher: k10 k21 -->
