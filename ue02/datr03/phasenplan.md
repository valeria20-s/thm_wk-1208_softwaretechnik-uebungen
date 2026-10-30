# Phasenplan — Terminplaner für die THM

Kürzel: datr03

## Studie

**Ergebnis der Phase:** Ein Lastenheft mit den Wünschen und Anforderungen der THM sowie eine erste Kostenabschätzung und ein Projektplan.

- Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Aufwand schätzen und einen Meilensteinplan vorschlagen
- Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
- Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
- Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten

## Systemspezifikation

**Ergebnis der Phase:** Ein Pflichtenheft, in dem genauer steht, welche Funktionen das System haben soll und wie die Anforderungen umgesetzt werden.

- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden

## Systemkonstruktion

**Ergebnis der Phase:** Ein technischer Bauplan, der zeigt, wie die Software aufgebaut ist, welche Komponenten es gibt und wie diese zusammenarbeiten.

- Datenbank, Programmiersprache und Web-Framework auswählen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert

## Implementierung

**Ergebnis der Phase:** Die einzelnen Funktionen und Komponenten sind programmiert und wurden getestet.

- Die Komponente „Benachrichtigung“ programmieren
- Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt

## Integration & Einführung

**Ergebnis der Phase:** Die Komponenten wurden zusammengeführt, das gesamte System getestet und bei der THM eingeführt.

- Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung
- Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
- Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
- Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
- Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt

## Wartung

**Ergebnis der Phase:** Fehler werden behoben, das System wird betreut und bei Bedarf um neue Funktionen erweitert.

- Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
- Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
- Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen

## Bei welchen Karten waren Sie unsicher — und was haben Sie abgewogen?

- **Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten** (Studie): Wahrscheinlich Studie, war mir nicht sicher

<!-- zuordnung ue02-phasenplan: k01=implementierung k02=studie k03=integration k04=spezifikation k05=wartung k22=spezifikation k06=spezifikation k07=studie k08=integration k09=konstruktion k10=studie k11=wartung k12=implementierung k23=konstruktion k13=studie k14=studie k15=konstruktion k16=integration k17=wartung k18=studie k19=spezifikation k24=integration k20=integration k21=konstruktion | unsicher: k02 -->
