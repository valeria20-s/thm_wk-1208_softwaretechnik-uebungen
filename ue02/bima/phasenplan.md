# Phasenplan — Terminplaner für die THM

Kürzel: bima

## Studie

**Ergebnis der Phase:** Ein Dokument mit Ist-Analyse, Anforderungen, Lösungsvarianten, Empfehlung und Projektplan (Lastenheft)

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Aufwand schätzen und einen Meilensteinplan vorschlagen

## Systemspezifikation

**Ergebnis der Phase:** Ein Fachkonzept (Pflichtenheft), das die fachlichen Anforderungen genau beschreibt

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen

## Systemkonstruktion

**Ergebnis der Phase:** Die Beschreibung der Systembestandteile (Komponenten und Schnittstellen) und der technischen Architektur

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert

## Implementierung

**Ergebnis der Phase:** Programmierte und getestete Komponenten

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Integration & Einführung

**Ergebnis der Phase:** Ein getestetes, vom Kunden abgenommenes und eingeführtes (Teil-)System

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Wartung

**Ergebnis der Phase:** Ein weiter betreutes System, dessen Fehler beseitigt und das bei Bedarf angepasst oder erweitert wird

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen** (Systemspezifikation): Ich war unsicher, ob das Konstruktion ist, weil es um die API geht. Aber was der Agent tun darf, ist eine fachliche Entscheidung. Darum Systemspezifikation.
- **Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen** (Systemkonstruktion): Ich war unsicher, ob das Spezifikation ist, weil die API gewünscht wurde. Aber Endpunkte und Datenformat zeigen, wie es technisch gebaut wird. Darum Systemkonstruktion.
- **Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten** (Implementierung): Ich dachte an Konstruktion. Aber in der Vorlesung gehört die Planung mit Zwischenzielen und der Reihenfolge zur Implementierung.
- **Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt** (Integration & Einführung): Ich war unsicher, ob das Implementierung ist, weil getestet wird. Aber hier wird das ganze System über die API geprüft. Das ist ein Systemtest, also Integration.
- **Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde** (Systemspezifikation): Ich dachte zuerst an Integration, weil getestet wird. Aber die Testfälle sagen, was vereinbart wurde. Darum gehören sie zur Systemspezifikation.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=konstruktion k16=integration k17=wartung k18=implementierung k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k22 k23 k18 k24 k21 -->
