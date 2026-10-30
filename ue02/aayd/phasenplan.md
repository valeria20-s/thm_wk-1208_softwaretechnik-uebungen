# Phasenplan — Terminplaner für die THM

Kürzel: aayd

## Studie

**Ergebnis der Phase:** Lastenheft mit Ist-Analyse, Anforderungen, Lösungsvarianten, Empfehlung und Projektplan

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Aufwand schätzen und einen Meilensteinplan vorschlagen

## Systemspezifikation

**Ergebnis der Phase:** Fachkonzept (Pflichtenheft) mit detaillierten fachlichen Anforderungen und Modellen

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde

## Systemkonstruktion

**Ergebnis der Phase:** Festgelegte Softwarearchitektur mit Komponenten, Schnittstellen und technischer Infrastruktur

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert

## Implementierung

**Ergebnis der Phase:** Programmierte und einzeln getestete Softwarekomponenten

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Integration & Einführung

**Ergebnis der Phase:** Integriertes, getestetes, abgenommenes und eingeführtes System

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Wartung

**Ergebnis der Phase:** Betreutes und gewartetes System mit Fehlerbehebungen und Erweiterungen

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen** (Systemspezifikation): Auch die technische API muss diese Regeln umsetzen. Ich ordne die Tätigkeit der Systemspezifikation zu, weil hier zunächst die fachlichen Berechtigungen festgelegt werden.
- **Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert** (Systemkonstruktion): Der Prototyp könnte bereits in der Studie zur Machbarkeitsprüfung dienen. Technische Prototypen gehören aber zur Systemkonstruktion, weshalb ich diese Phase wähle.
- **Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten** (Implementierung): Eine solche Planung könnte bereits Teil der Studie sein. Hier geht es aber konkret um die Reihenfolge der Komponentenimplementierung, deshalb wähle ich Implementierung.
- **Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden** (Systemspezifikation): Auch die Systemkonstruktion beschäftigt sich mit Schnittstellen. Hier wird jedoch zunächst fachlich beschrieben, welche Daten ausgetauscht werden sollen. Deshalb wähle ich Systemspezifikation.
- **Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde** (Systemspezifikation): Die Testfälle werden später bei der Integration ausgeführt. Da sie hier zunächst aus den vereinbarten Anforderungen abgeleitet werden, ordne ich die Tätigkeit der Systemspezifikation zu.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=konstruktion k16=integration k17=wartung k18=implementierung k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k22 k15 k18 k19 k21 -->
