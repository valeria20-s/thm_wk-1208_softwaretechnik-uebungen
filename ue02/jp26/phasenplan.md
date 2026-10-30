# Phasenplan — Terminplaner für die THM

Kürzel: jp26

## Studie

**Ergebnis der Phase:** Lastenheft

- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Aufwand schätzen und einen Meilensteinplan vorschlagen

## Systemspezifikation

**Ergebnis der Phase:** Pflichtenheft

- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden

## Systemkonstruktion

**Ergebnis der Phase:** Technische und fachliche softwarearchitektur mit Komponenten und Schnittstellen n

- Datenbank, Programmiersprache und Web-Framework auswählen
- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen

## Implementierung

**Ergebnis der Phase:** Programmierte und getestete Komponenten

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat

## Integration & Einführung

**Ergebnis der Phase:** Getestetes, abgenommenes und eingefügtes System

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen

## Wartung

**Ergebnis der Phase:** Fehlerbehebung, Anpassung, Erweiterung und Anwenerbetreuung

- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen** (Systemspezifikation): geraten
- **Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde** (Wartung): geraten

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=implementierung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=konstruktion k11=wartung k12=implementierung k23=spezifikation k13=studie k14=spezifikation k15=konstruktion k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=integration k20=integration k21=wartung | unsicher: k23 k21 -->
