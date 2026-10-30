# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben: @Feng002

<!-- Je Abschnitt Ihrer Gliederung eine Überschrift (## für Abschnitte, ###
     für Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten würden.
     Die beiden Überschriften unten sind lediglich Platzhalter. -->

## 1. Ziel und Umfang

Die Software soll die Vereinbarung von Sprechstunden und Prüfungsterminen an der THM vereinfachen. Lehrende stellen Termine bereit, Studierende buchen sie und Sekretariate behalten der Überblick.

### 1.1 Erste Ausbaustufe

Gebuchte Termine können als iCal-Datei heruntergeladen werden. Eine direkte Verbindung zu den Kalendern die Beteiligten ist für eine spätere Ausbaustufe vorgesehen.

## 2. Nutzer und Berechtigungen

Die Spezifikation muss beschreiben, wer das System verwendet und welche Aktionen erlaubt sind.

### 2.1 Rollen

Lehrende können eigene Termine anbieten. Studierende können freie Termine ansehen und buchen. Sekretariate benötigen eine Übersicht über die Termine ihres Bereichs.

### 2.2 Anmeldung

Die Anmeldung erfolgt über das Hochschulkonto. Ein Studierender darf beispielsweise keine Termine im Namen eines Lehrenden anbieten.

## 3. Funktionen und Abläufe

Hier wird beschrieben, was die Nutzer Schritt für Schritt im System tun können.

### 3.1 Termine anbieten

Ein Lehrender gibt für eine Sprechstunde Datum, Uhrzeit und eine mögliche Anzahl an Plätzen ein. Danach erscheint der Termin für Studierende als buchbar.

### 3.2 Termin buchen

Ein Studierender wählt einen freien Termin aus und bestätigt die Buchung. Der Termin darf danach nicht gleichzeitig an eine andere Person vergeben werden.

### 3.3 Termine verwalten

Ein Sekretariat sieht, welche Termine angeboten und welche bereits gebucht wurden. Ob und bis wann Studierende selbst absagen dürfen, muss noch mit der THM geklärt werden.

## 4. Benötigte Daten

Für jede Funktion muss feststehen, welche Angaben gespeichert und angezeigt werden.

### 4.1 Daten eines Termins

Zu einem Termin gehören beispielsweise Datum, Beginn, Ende, Lehrender, Art des Termins und verfügbare Plätze. Bei einer Buchung kommt die Zuordnung zum Studierenden hinzu.

## 5. Schnittstellen

Das Entwicklerteam muss wissen, mit welchen anderen Systemen der Terminplaner Daten austauscht.

### 5.1 Kalenderdatei

Nach der Buchung kann ein Studierender eine iCal-Datei herunterladen. Diese enthält beispielsweise Titel, Datum, Uhrzeit und Ort des Termins.

### 5.2 API für KI-Agenten

Über die API können berechtigte KI-Agenten freie Termine abfragen und Buchungen auslösen. Welche Aktionen ein Agent genau ausführen darf, muss festgelegt werden; Prüfungstermine soll er beispielsweise nicht ohne Berechtigung absagen können.

## 6. Qualität und Schutz der Daten

Neben den Funktionen sind Anforderungen an die Nutzung und den Umgang mit persönlichen Daten nötig.

### 6.1 Datenschutz

Studierende sollen nur ihre eigenen Buchungen sehen. Ein Lehrender sieht die Personen, die seine Termine gebucht haben, aber keine fremden Termine anderer Lehrender.

### 6.2 Verständliche Bedienung

Ein Studierender soll erkennen können, ob ein Termin noch frei ist und ob eine Buchung erfolgreich war. Fehlermeldungen sollen erklären, was zu tun ist.

## 7. Prüfung und offene Fragen

Die THM und das Entwicklerteam brauchen Beispiele, mit denen sie später prüfen können, ob die Software das Vereinbarte leistet.

### 7.1 Beispiel für einen Testfall

Ein Studierender bucht den letzten freien Platz einer Sprechstunde. Danach zeigt das System den Termin als ausgebucht an und lässt keine weitere Buchung zu.

### 7.2 Noch zu klärende Punkte

Mit der THM ist zu klären, ob Studierende Buchungen selbst absagen dürfen und welche Frist dafür gilt. Die Antwort muss vor der Umsetzung in die Spezifikation aufgenommen werden.
