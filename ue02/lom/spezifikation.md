# Spezifikation des Terminplaners – Gliederung und Beispiele

Mitarbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit):  
@1Lawand

## 1. Ziel und Zweck des Systems

**Beispiel:** Der Terminplaner soll die Vereinbarung von Sprechstunden und Prüfungsterminen an der THM vereinfachen. Studierende sollen verfügbare Termine finden und buchen können. Lehrende und Sekretariate sollen ihre Termine übersichtlich verwalten können.

## 2. Benutzer und Rollen

**Beispiel:** Das System unterscheidet zwischen Studierenden, Lehrenden und Sekretariaten. Studierende können Termine buchen oder absagen. Lehrende können Sprechstunden anbieten und ihre verfügbaren Zeiten verwalten. Sekretariate unterstützen die Organisation.

## 3. Funktionale Anforderungen

**Beispiel:** Studierende sollen einen freien Sprechstundentermin auswählen und verbindlich buchen können. Nach erfolgreicher Buchung zeigt das System eine Bestätigung an. Bereits belegte Termine dürfen nicht erneut vergeben werden.

## 4. Nichtfunktionale Anforderungen

**Beispiel:** Die Buchungsseite soll auf Smartphones und Computern gut bedienbar sein. Persönliche Daten dürfen nur für berechtigte Personen sichtbar sein. Das System soll auch bei vielen gleichzeitigen Zugriffen zuverlässig funktionieren.

## 5. Daten und Informationsmodell

**Beispiel:** Zu einem Termin gehören eine eindeutige Kennung, Datum, Uhrzeit, Dauer, Raum und zuständige Lehrperson. Eine Buchung verbindet einen Termin mit einer studierenden Person.

## 6. Benutzeroberfläche

**Beispiel:** Auf der Buchungsseite werden verfügbare Termine in einer übersichtlichen Liste angezeigt. Studierende wählen einen Termin aus und bestätigen die Buchung. Anschließend erscheint eine verständliche Erfolgsmeldung.

## 7. Schnittstellen zu anderen Systemen

**Beispiel:** Der Terminplaner soll Termine als iCal-Datei bereitstellen, damit sie in Kalenderprogramme übernommen werden können. Außerdem soll eine API ermöglichen, dass berechtigte KI-Agenten freie Termine abfragen und Sprechstundentermine buchen.

## 8. Sicherheit und Zugriffsrechte

**Beispiel:** Die Anmeldung erfolgt über das Hochschulkonto. Studierende dürfen nur ihre eigenen Buchungen verwalten. Ein KI-Agent darf keine Prüfungstermine absagen, wenn ihm dafür keine Berechtigung erteilt wurde.

## 9. Test- und Abnahmekriterien

**Beispiel:** Wenn eine studierende Person einen freien Termin erfolgreich bucht, muss dieser anschließend als belegt angezeigt werden. Versucht eine zweite Person denselben Termin zu buchen, muss das System die Doppelbuchung verhindern.

## 10. Rahmenbedingungen und Abgrenzung

**Beispiel:** Der Terminplaner soll in der IT-Umgebung der THM betrieben werden können. Die erste Version unterstützt die Buchung von Terminen und den Export als iCal-Datei. Eine direkte Synchronisation mit allen Kalenderprogrammen ist zunächst nicht vorgesehen.
