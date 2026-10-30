# Phasenplan — Terminplaner für die THM

Kürzel: kraz

## Studie

**Ergebnis der Phase:** Studie mit Ist-Analyse, bewerteten Lösungsvarianten und Projektvorschlag (Aufwand, Meilensteine)

- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
- Aufwand schätzen und einen Meilensteinplan vorschlagen

## Systemspezifikation

**Ergebnis der Phase:** Systemspezifikation: Anwendungsfälle, Datenmodell, Dialoge, Schnittstellen zu Nachbarsystemen und Testfälle

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen

## Systemkonstruktion

**Ergebnis der Phase:** Systemkonstruktion: Architektur mit Komponenten und Schnittstellen, gewählte Technik und Implementierungsplan

- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten

## Implementierung

**Ergebnis der Phase:** Programmierte und einzeln getestete Komponenten

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt

## Integration & Einführung

**Ergebnis der Phase:** Integriertes, getestetes und vom Kunden abgenommenes System im Betrieb

- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Wartung

**Ergebnis der Phase:** Laufendes System mit behobenen Fehlern und neuen Versionen

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen** (Systemspezifikation): Schwankte zwischen Spezifikation und Konstruktion; was erlaubt ist, ist eine fachliche Entscheidung, daher Spezifikation.
- **Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen** (Wartung): Beginnt schon mit der Einführung, läuft aber dauerhaft während des Betriebs, daher Wartung.
- **Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen** (Systemkonstruktion): Die API gehört zur Schnittstelle nach außen (Spezifikation), Endpunkte und Datenformat sind aber technische Entwurfsentscheidungen, daher Konstruktion.
- **Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert** (Systemkonstruktion): Könnte auch zur Studie gehören (Machbarkeit), ich sehe es aber als Prüfung eines technischen Risikos in der Konstruktion.
- **Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt** (Integration & Einführung): Klingt nach einer Prüfung der API-Spezifikation, ist aber ein Test des fertigen Gesamtsystems, daher Integration.
- **Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde** (Systemspezifikation): Die Testfälle werden erst bei Integration und Abnahme benutzt, aber schon in der Spezifikation festgelegt, weil sie beschreiben, was vereinbart wurde.

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=konstruktion k07=studie k08=integration k09=konstruktion k10=spezifikation k11=wartung k12=implementierung k23=konstruktion k13=studie k14=spezifikation k15=konstruktion k16=integration k17=wartung k18=konstruktion k19=spezifikation k24=integration k20=integration k21=spezifikation | unsicher: k22 k11 k23 k15 k24 k21 -->
