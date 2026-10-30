# Spezifikation des Terminplaners — Gliederung und Beispiele

GitHub-Benutzernamen: AVon507

## 1. Systemziel und Rahmenbedingungen
- Beispiel: Der Terminplaner soll die Vergabe von Sprechstunden und Prüfungsterminen zwischen Studierenden, Professoren und dem Sekretariat digitalisieren und vereinfachen, ohne dass man sich per zeitaufwendigen E-Mail Absprachen darüber verständigen muss.

## 2. Funktionale Anforderungen
- Beispiel: Ein externer KI-Agent darf über die API freie Termine abfragen und buchen, hat jedoch keine Berechtigungen bestehende Prüfungstermine abzusagen.

## 3. Benutzeroberfläche und Bedienung
- Beispiel: Eine übersichtliche Wochenkalender Ansicht zeigt farblich markiert (Grün = frei, Rot = belegt), welche Zeitslots verfügbar sind oder auch nicht.

## 4. Datenschnittstellen und Datenaustausch externer Systeme
- Beispiel: Beim erfolgreichen Buchen eines Termins wird ein ICS-Kalendereintrag generiert und direkt an den Outlook-Kalender des Studierenden und der jeweiligen Hochschule übertragen.

## 5. Qualitätsanforderungen & Datenschutz
- Beispiel: Die Anmeldung erfolgt sicher über das zentrale Hochschulkonto, sodass keine Passwörter im Terminplaner selbst gespeichert werden müssen.