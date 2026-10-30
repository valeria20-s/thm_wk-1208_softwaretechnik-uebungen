# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben  @muxstii


## 1. Ziel des Systems

Der Terminplaner soll den Studierenden und Lehrenden der THM helfen, Termine einfacher zu planen und zu buchen.
Lehrende können Termine anbieten und Studierende können diese online buchen.

## 2. Benutzer des Systems

Es gibt drei Benutzergruppen: Studierende, Lehrende und Sekretariat.
Studierende buchen Termine, Lehrende erstellen und verwalten Termine und das Sekretariat hilft bei der Organisation.

## 3. Funktionen des Terminplaners

### 3.1 Anmeldung

Die Benutzer melden sich mit ihrem THM-Konto an.
Das System erkennt, ob der Benutzer ein Studierender oder ein Lehrender ist.

### 3.2 Termine erstellen

Lehrende können neue Termine mit Datum, Uhrzeit und Ort erstellen.
Sie können ihre Termine auch ändern oder löschen.

### 3.3 Termine buchen und absagen

Studierende können freie Termine auswählen und buchen.
Wenn sie einen Termin nicht wahrnehmen können, können sie ihn wieder absagen.

## 4. Ablauf der Terminbuchung

### 4.1 Einen Termin buchen

Der Studierende meldet sich an und sucht einen freien Termin aus.
Nach der Bestätigung wird die Buchung gespeichert und der Studierende bekommt eine Bestätigung.

### 4.2 Einen Termin absagen

Der Studierende öffnet seine Buchungen und wählt den Termin aus, den er absagen möchte.
Danach wird der Termin wieder für andere Studierende freigegeben.

## 5. Daten und Informationen

### 5.1 Termindaten

Zu jedem Termin werden Datum, Uhrzeit, Dauer, Ort und die zuständige Lehrperson gespeichert.
Außerdem muss angezeigt werden, ob der Termin noch frei oder bereits gebucht ist.

### 5.2 Buchungsdaten

Das System speichert, welcher Studierende welchen Termin gebucht hat.
So können Studierende ihre Buchungen ansehen und Lehrende sehen, wer einen Termin gebucht hat.

## 6. Benutzeroberfläche

### 6.1 Terminübersicht

Die Benutzer sehen eine Übersicht mit allen verfügbaren Terminen.
Freie und bereits gebuchte Termine sollen leicht zu unterscheiden sein.

### 6.2 Buchungsseite

Wenn ein Studierender einen Termin auswählt, werden die wichtigsten Informationen angezeigt.
Nach dem Buchen erscheint eine Bestätigung.

## 7. Schnittstellen

### 7.1 THM-Konto

Die Anmeldung soll über das bestehende THM-Konto funktionieren.
Die Benutzer sollen kein zusätzliches Konto erstellen müssen.

### 7.2 KI-Agenten und Kalenderexport

KI-Agenten sollen über eine Schnittstelle freie Termine suchen und Buchungen durchführen können, wenn sie berechtigt sind.
Außerdem sollen Benutzer ihre Termine als iCal-Datei herunterladen können.

## 8. Sicherheit und Zuverlässigkeit

Persönliche Daten dürfen nur von berechtigten Personen eingesehen werden.
Das System muss außerdem verhindern, dass zwei Studierende denselben Termin gleichzeitig buchen.

## 9. Tests und Abnahme

Vor der Fertigstellung wird getestet, ob die Anmeldung, die Buchung und die Absage von Terminen funktionieren.
Die THM überprüft anschließend, ob das System die beschriebenen Anforderungen erfüllt.
