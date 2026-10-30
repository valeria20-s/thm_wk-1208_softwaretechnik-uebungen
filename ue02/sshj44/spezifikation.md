# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben: @sshj44

## Kopie aus `notiz.md` - Gesprächsnotiz
Die Software soll sich über das Hochschulkonto bedienen lassen:
- Lehrende bieten Sprechstunden und Prüfungstermine an
- Studierende buchen sie
- Sekretariate behalten den Überblick

- Zunächst Termine als iCal-Datei zum Herunterladen anbieten, später direkt in die Kalender der Beteiligten eintragen

- soll eine API bekommen, über die KI-Agenten sie steuern können
- *Wir wollen nicht noch ein Werkzeug, das am Ende keiner benutzt.* -THM-

<!-- Kopie aus `phasenplan.md`

- Festlegen, welche Vorgänge ein KI-Agent über die API auslösen darf — z.B. freie Termine abfragen und buchen, aber keine Prüfungstermine absagen
- Bildschirmskizzen der Buchungsseite mit Studierenden durchgehen
- Die API entwerfen: Endpunkte, Datenformat und die Anmeldung der KI-Agenten festlegen
- Testfälle formulieren, an denen sich später zeigt, ob das System leistet, was vereinbart wurde
- Mit Lehrenden und Sekretariaten Schritt für Schritt beschreiben, wie ein Sprechstundentermin gebucht wird
- Beschreiben, welche Termindaten mit dem Kalendersystem der Hochschule ausgetauscht werden
-->
## Oberfläche

- Benutzeroberfläche soll dem bestehenden ähneln (Hochschulportal)

  - Reibungsfreier Übergang zu einem neu einführenden System

### Lehrende

- Sprechstunden sowie Prüfungsdaten in einem einzigen Planer anzeigen

### Studierende

- Trennung von Sprechstunden und Prüfungsdaten bei der Buchung

  - Es können *nur Sprechstunden* sowie *nur Prüfungsdaten* angezeigt werden

- Bei der Übersicht für beanspruchte Termine kann die Ansicht personalisiert werden

### Sekretariate

- Für das jeweilige Sekretariat angemessene Ansichtsoptionen für den Überblick

## Verbindung zum Hochschulkonto

- ID des Hochschulkontos wird automatisch zur Benutzererkennung für die Software
  
  - Durch Verbindung wird die Differenzierung der Benutzerfunktionen zwischen Lehrenden und Studierenden ermöglicht
  - Sekretariate bekommen eine andere zusätzliche Zugangsmethode zum System

### Studierende

- Zugriff auf Leistungen und Zulassungen jedweder Prüfungen

## Funktionalitäten

### Lehrende
- Sprechstunden anbieten

  - Beliebige Start- und Endzeit des Termins auswählen lassen
  - Überprüfen, ob diese Zeit sich nicht mit anderen Terminen überschneidet
  - Bei der Publikation des Termins wird eine vorläufige iCal-Datei automatisch erstellt. Informationen werden nach Beanspruchung des Termins vollständig ausgefüllt.

- Prüfungstermine anbieten

  - Beliebige Start- und Endzeit des Termins auswählen lassen
  - Überprüfen, ob diese Zeit sich nicht mit anderen Terminen überschneidet
  - Bei der Publikation des Termins wird eine vorläufige iCal-Datei automatisch erstellt. Informationen werden nach Beanspruchung des Termins vollständig ausgefüllt.
  - Die Einstellung der Teilnehmer-Obergrenze ermöglichen

### Studierende

- Sprechstunden buchen

  - Beliebige zur Verfügung stehende Sprechstunde kann gebucht werden
  - Buchungen ohne Beschreibung des Anlasses sind nicht möglich
  - Überprüfen, ob diese Zeit sich nicht mit anderen gebuchten Terminen überschneidet
  - Bei der Beanspruchung des Termins wird das Herunterladen der zugehörigen iCal-Datei angeboten

- Prüfungstermine buchen

  - Mit Hilfe des Hochschulkontos sind die zur Verfügung stehenden / zugelassenen Prüfungen gefiltert
  - Diese können beliebig gebucht werden
  - Überprüfen, ob diese Zeit sich nicht mit anderen gebuchten Terminen überschneidet
  - Bei der Beanspruchung des Termins wird das Herunterladen der zugehörigen iCal-Datei angeboten

### Sekretariate

- Sprechstunden und Prüfungstermine sehen

  - Jeder freigegebener Termin inklusive der dazugehörigen iCal-Datei kann gesehen werden

- iCal-Dateien bearbeiten, speichern, löschen

- Autorität zur Raumzuteilung

## iCal-Datei

- Ohne Eingriff des Sekretariats bleiben sie nur so lange erhalten, bis die Endzeit des jeweiligen Termins erreicht ist

### Inhalt bei Sprechstunden

- Anlass
- Datum
- Uhrzeit
- Raum
- Teilnehmer

### Inhalt bei Prüfungsterminen

- Modulname
- Datum
- Uhrzeit
- Raum
- Name des Lehrenden


## API

- KI-Agenten sollen sie steuern können