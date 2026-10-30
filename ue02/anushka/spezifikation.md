# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @sadimadi22, @marroer19-hub, @anushka667

---

> *Begründung der Gliederung:* Die Spezifikation folgt einer logischen Struktur von den allgemeinen Zielen und Rollen (Kapitel 1) über die konkreten Funktionen für Anwender (Kapitel 2) und technische Schnittstellen (Kapitel 3) bis hin zur visuellen Darstellung (Kapitel 4) und qualitativen Rahmenbedingungen (Kapitel 5).

---

## 1. Zielbestimmung und Zielgruppe

### 1.1 Zielsetzung des Systems
Das System soll eine einfache Online-Plattform sein, über die Termine an der THM schnell und unkompliziert vereinbart werden können. Lehrende, Studierende und Sekretariate sollen Sprechstunden und Prüfungen ohne ständiges E-Mail-Schreiben organisieren können.

### 1.2 Zielgruppen und Benutzerrollen
Es gibt drei Hauptrollen im System:
- *Lehrende:* Tragen freie Zeiten für Sprechstunden oder Prüfungen ein.
- *Studierende:* Suchen freie Termine aus und buchen diese direkt.
- *Sekretariat:* Hat den Überblick über alle Termine und hilft bei Problemen oder Überschneidungen.

---

## 2. Funktionalitäten (Anwendungsfälle)

### 2.1 Terminverwaltung für Lehrende
Lehrende können neue Terminblöcke anlegen, festlegen wie lange ein Termin dauert (z. B. 15 Minuten) und sehen, wer sich eingetragen hat.

### 2.2 Terminbuchung für Studierende
Studierende wählen einen Dozenten aus, suchen einen freien Slot und geben kurz an, worum es geht (z. B. "Frage zu Übung 2").

### 2.3 Benachrichtigungen und Export
Wenn ein Termin gebucht wird, bekommen alle eine Bestätigung per Mail. Außerdem kann man den Termin als iCal-Datei herunterladen und im eigenen Kalender speichern.

---

## 3. Schnittstellen und Systemintegration

### 3.1 Login mit dem Hochschulkonto
Man meldet sich einfach mit seinen normalen THM-Zugangsdaten an.
- *Beispiel:* Die Authentifizierung erfolgt über das zentrale SSO-System der THM (Shibboleth/CAS) mit Matrikelnummer und Passwort.

### 3.2 Schnittstelle für KI-Agenten (API)
Das System soll eine API haben, damit auch KI-Agenten Termine abfragen und buchen können.

- *Was die KI darf:* Freie Termine suchen und für Studierende buchen.
- *Was die KI nicht darf:* Sie darf keine Prüfungstermine stornieren.

---

## 4. Benutzeroberfläche und Bedienkonzept

### 4.1 Seitenansicht und Buchungsablauf
Die Buchungsseite soll übersichtlich sein und auch auf dem Smartphone gut funktionieren.



+-------------------------------------------------------------+
| [THM-Logo]  Terminbuchung Prof. Mustermann                 |
+-------------------------------------------------------------+
| Datum: 12.11.2026 | Uhrzeit: 14:00 - 14:15 Uhr              |
| Grund: [ Fragen zur Abschlussarbeit                       ] |
|                                                             |
| [ Jetzt verbindlich buchen ]   [ Abbrechen ]               |
+-------------------------------------------------------------+



---

## 5. Qualitätsanforderungen und Rahmenbedingungen

### 5.1 Datenschutz und Sicherheit
Alle Daten werden sicher behandelt und bleiben auf den Servern der THM.
- *Beispiel:* Termindaten und Namen von Studierenden werden spätestens 30 Tage nach Ablauf des Termins automatisch gelöscht.

### 5.2 Geschwindigkeit
Die Webseite muss auch dann schnell laden, wenn viele Studierende gleichzeitig einen Termin buchen wollen (z. B. zu Beginn der Anmeldephase).
- *Beispiel:* Die Reaktionszeit des Systems darf bei bis zu 500 gleichzeitigen Zugriffen maximal 2 Sekunden betragen.