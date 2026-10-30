# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @AfremAydin

## 1. Ziel der Software

Der Terminplaner soll die Terminvereinbarung an der THM einfacher machen. Statt Termine per E-Mail oder über verschiedene Programme zu vereinbaren, soll alles über ein System laufen.

## 2. Benutzer des Systems

Studierende sollen Termine buchen können. Lehrende sollen Sprechstunden und Prüfungstermine anbieten können. Die Sekretariate sollen einen Überblick über die Termine haben.

## 3. Funktionen

Lehrende können freie Termine erstellen und Studierende können diese buchen oder absagen. Bereits gebuchte Termine sollen nicht noch einmal vergeben werden.

## 4. Ablauf einer Buchung

Ein Student meldet sich an, sucht einen Lehrenden und wählt einen freien Termin aus. Anschließend bestätigt er die Buchung und bekommt eine Bestätigung angezeigt.

## 5. Benötigte Daten

Zu jedem Termin müssen Informationen wie Datum, Uhrzeit, Dauer und Lehrender gespeichert werden. Außerdem muss erkennbar sein, ob ein Termin noch frei oder bereits gebucht ist.

## 6. Anmeldung und Berechtigungen

Die Anmeldung soll über das THM-Hochschulkonto erfolgen. Studierende dürfen Termine buchen, aber keine Termine von Lehrenden erstellen.

## 7. Kalender und Schnittstellen

Gebuchte Termine sollen heruntergeladen und in den eigenen Kalender übernommen werden können. Über eine API sollen auch KI-Agenten freie Termine suchen und buchen können.

## 8. Bedienung und Überprüfung

Die Software soll einfach zu bedienen sein und auch auf dem Handy funktionieren. Bei einem Test könnte geprüft werden, ob zwei Studierende denselben Termin gleichzeitig buchen können. Das System darf nur eine Buchung zulassen.