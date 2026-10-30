# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @Talhakc22

## 1. Ziel und Zweck

Der Terminplaner soll die Terminvereinbarung zwischen Studierenden und Lehrenden vereinfachen und bürokratischen Aufwand reduzieren.

Die Software soll rund um die Uhr erreichbar sein. Studierende sollen Termine unabhängig von den Öffnungszeiten der Sekretariate anfragen können.

## 2. Benutzer und Rollen

### Studierende

Studierende können verfügbare Termine einsehen, Terminanfragen stellen und bereits vereinbarte Termine verwalten.

Eine Stornierung soll ohne Angabe von Gründen bis zu zwölf Stunden vor dem Termin möglich sein.

### Lehrende

Lehrende können verfügbare Zeitfenster freigeben, sperren und eingehende Terminanfragen genehmigen oder ablehnen.

### Sekretariate

Die Sekretariate erhalten einen Überblick über relevante Termine und unterstützen die organisatorische Verwaltung.

## 3. Funktionale Anforderungen

### Terminverwaltung

Studierende können freie Zeitfenster auswählen und eine Terminanfrage absenden.

Bis zur Entscheidung der Lehrperson wird das Zeitfenster als vorläufig reserviert gekennzeichnet.

Eine endgültige Buchung erfolgt erst nach Genehmigung durch die zuständige Lehrperson.

Wird eine Anfrage abgelehnt, ist das Zeitfenster wieder verfügbar, sofern die Lehrperson es nicht gesperrt hat.

### Benachrichtigungen

Wird ein bereits gebuchter Termin frei, können interessierte Studierende automatisch darüber informiert werden.

Benachrichtigt werden ausschließlich Studierende, die sich zuvor freiwillig für diese Funktion angemeldet haben.

Dadurch sollen frei gewordene Termine möglichst effizient neu vergeben werden.

## 4. Nichtfunktionale Anforderungen

### Leistung und Reaktionsgeschwindigkeit

Die Software soll Anfragen schnell verarbeiten und Änderungen der Terminverfügbarkeit zeitnah anzeigen.

Insbesondere bei gleichzeitigen Buchungsanfragen muss verhindert werden, dass ein Zeitfenster mehrfach verbindlich vergeben wird.

Konkrete Antwortzeitgrenzen und Belastungsszenarien müssen noch festgelegt werden.

### Verfügbarkeit

Der Terminplaner soll grundsätzlich rund um die Uhr zugänglich sein, damit Studierende auch außerhalb der üblichen Hochschulzeiten Termine organisieren können.

## 5. Schnittstellen

### Hochschulkonto

Die Anmeldung erfolgt über das bestehende Hochschulkonto der THM.

Die Software soll hierfür mit dem Authentifizierungssystem der Hochschule verbunden werden, sodass keine separate Registrierung erforderlich ist.

### Stundenplan und Sekretariat

Der Terminplaner soll Informationen mit dem bestehenden Stundenplansystem und den zuständigen Sekretariaten austauschen.

Dadurch soll verhindert werden, dass Lehrenden Termine während ihrer regulären Lehrveranstaltungen zugewiesen werden.

### iCal

Vereinbarte Termine sollen zunächst als iCal-Datei zum Herunterladen bereitgestellt werden.

Dadurch können die Termine in persönliche Kalender übernommen werden. Eine spätere direkte Kalendersynchronisation bleibt als Erweiterungsmöglichkeit bestehen.

### API für KI-Agenten

Die Software soll eine Programmierschnittstelle (API) bereitstellen, über die berechtigte KI-Agenten verfügbare Termine abfragen und Terminanfragen übermitteln können.

Die KI-Agenten dürfen keine eigenständige Genehmigung erteilen. Die endgültige Entscheidung liegt weiterhin bei der zuständigen Lehrperson.

## 6. Geschäftsregeln und Einschränkungen

- Terminanfragen benötigen die Zustimmung der zuständigen Lehrperson.
- Eine vorläufige Reservierung ist nicht mit einer bestätigten Buchung gleichzusetzen.
- Abgelehnte Zeitfenster werden wieder freigegeben, sofern keine Sperrung vorliegt.
- Studierende können bestätigte Termine bis zwölf Stunden vor Beginn ohne Angabe von Gründen stornieren.
- Automatische Benachrichtigungen setzen die freiwillige Anmeldung der Studierenden voraus.
- KI-Agenten dürfen keine Berechtigungen zur eigenständigen Termingenehmigung erhalten.

## 7. Offene Fragen

Vor der endgültigen Umsetzung müssen weitere Punkte mit der THM abgestimmt werden:

- Wie lange darf eine unbeantwortete Terminanfrage ein Zeitfenster blockieren?
- Welche konkreten Antwortzeiten muss die Software einhalten?
- Wie erfolgt die technische Anbindung an das bestehende Stundenplansystem?
- Welche Aufgaben und Berechtigungen sollen die Sekretariate erhalten?

Die beschriebenen Erweiterungen und Geschäftsregeln sind zunächst Vorschläge und müssen vor einer verbindlichen Umsetzung mit dem Auftraggeber abgestimmt werden.