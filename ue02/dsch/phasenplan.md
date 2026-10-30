# Phasenplan — Terminplaner für die THM

Kürzel: dsch

## Studie

**Ergebnis der Phase:** Studie mit Grobkonzept und Aufwandsschätzung

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert


## Systemspezifikation

**Ergebnis der Phase:** Spezifikation, also was das System fachlich leisten soll

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden

## Systemkonstruktion

**Ergebnis der Phase:** Konstruktion mit Komponenten, Schnittstellen und Technikauswahl

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen

## Implementierung

**Ergebnis der Phase:** programmierte und einzeln getestete Komponenten

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde

## Integration & Einführung

**Ergebnis der Phase:** integriertes und eingeführtes System

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Wartung

**Ergebnis der Phase:** korrigierte bzw. erweiterte Versionen des laufenden Systems

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen** (Systemspezifikation): War mir unsicher zwischen spec und Konstruktion, weil es um Funktionen geht, aber auch um die API
- **Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen** (Wartung): War mir unsicher zwischen Einführung und Wartung, weil die Hotline schon beim Start helfen kann, aber auch in dem Fall später gebraucht wird
- **Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden** (Systemspezifikation): War mir unsicher zwischen Spec und Konstruktion, da man festlegt, welche Daten gebraucht und wie sie ausgetauscht werden

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=studie k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=konstruktion k20=integration k21=implementierung | unsicher: k22 k11 k19 -->
