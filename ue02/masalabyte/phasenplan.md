# Phasenplan für das Projekt Terminplaner THM

## 1. Studie
* Die heutige Lage aufnehmen: wie Sprechstunden und Prüfungstermine bisher vereinbart werden und wo es hakt
* Eigenentwicklung, Anpassung einer Open-Source-Lösung und Kauf nebeneinanderstellen und nach Kosten und Nutzen bewerten
* Aufwand schätzen und einen Meilensteinplan vorschlagen
* **Ergebnis der Phase:** Machbarkeitsstudie und Entscheidungsgrundlage

## 2. Systemspezifikation
* Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
* Festlegen, welche Angaben zu einem Termin gehören und wie Termine, Personen und Räume zusammenhängen
* Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
* Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
* Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
* Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
* **Ergebnis der Phase:** Vollständige Systemspezifikation

## 3. Systemkonstruktion
* Das System in Komponenten zerlegen — z.B. Terminverwaltung, Benachrichtigung, Anmeldung — und deren Schnittstellen festlegen
* Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
* Datenbank, Programmiersprache und Web-Framework auswählen
* Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert
* Festlegen, in welcher Reihenfolge die Komponenten gebaut werden und welche Zwischenziele gelten
* **Ergebnis der Phase:** Systemarchitektur und Entwurfsdokumentation

## 4. Implementierung
* Die Komponente „Benachrichtigung“ programmieren
* Die fertige Komponente „Terminverwaltung“ für sich testen, ehe sie mit anderen zusammenkommt
* **Ergebnis der Phase:** Getestete Einzelkomponenten/Module

## 5. Integration & Einführung
* Terminverwaltung und Benachrichtigung zusammenführen und ihr Zusammenspiel gegen Testfälle prüfen
* Mit einem KI-Agenten prüfen, ob sich ein Sprechstundentermin vollständig über die API buchen lässt
* Das System als Ganzes unter Federführung des Qualitätsbeauftragten gegen die Testfälle prüfen
* Die THM installiert das System in ihrer eigenen Umgebung und prüft es in eigener Verantwortung (Abnahmetest)
* Probebetrieb mit einem Fachbereich, ehe die ganze Hochschule umsteigt
* **Ergebnis der Phase:** Abgenommenes, betriebsbereites Gesamtsystem

## 6. Wartung
* Einen Fehler bei der Zeitumstellung beheben, den ein Sekretariat gemeldet hat
* Eine Warteliste für ausgebuchte Termine nachrüsten, die sich die Lehrenden nach einem Semester wünschen
* Eine Hotline für Fragen der Anwenderinnen und Anwender besetzen
* **Ergebnis der Phase:** Lauffähiges System im Regelbetrieb

## Abgewogene Karten
* **Mit einem technischen Prototyp prüfen, ob die Anmeldung über das Hochschulkonto funktioniert:** Diese Karte könnte auch zur Spezifikation gehören, liegt aber Schwerpunktmäßig in der Konstruktion, da technische Machbarkeiten prototypisch evaluiert werden.