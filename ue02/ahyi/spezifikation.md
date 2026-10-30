# Spezifikation des Terminplaners — Gliederung und Beispiele
<!--
Beteiligte Personen (GitHub-Benutzername):
- YonkoYikit063
-->

# Spezifikation: Terminplaner für die THM

## 1. Ziel und Kontext des Systems
- **Zweck:** Beschreibt den groben Rahmen, die Problemstellung und wer das System nutzt.
- **Beispiel:** Das System dient der webbasierten Terminvergabe an der THM zwischen Lehrenden, Studierenden und Sekretariaten zur Reduzierung von E-Mail-Absprachen.

## 2. Benutzerrollen und Rechte
- **Zweck:** Definiert, wer welche Aktionen im System durchführen darf.
- **Beispiel:** 
  - *Lehrende:* Können Sprechstundenslots anlegen, ändern und stornieren.
  - *Studierende:* Können freie Slots buchen und eigene Buchungen einsehen.

## 3. Funktionale Anforderungen
- **Zweck:** Beschreibt detailliert die konkreten Funktionen und Abläufe der Anwendung.
- **Beispiel:** Wenn ein Studierender einen freien Termin bucht, wird der Slot blockiert, eine Bestätigungsmail versendet und eine `.ics`-Kalenderdatei generiert.

## 4. Schnittstellen und Integration
- **Zweck:** Legt fest, wie das System mit externen Systemen und Daten kommuniziert.
- **Beispiel:** 
  - Login via THM-LDAP / SSO (Hochschulkonto).
  - REST-API für externe KI-Agenten zur Abfrage freier Prüfungstermine.

## 5. Nicht-funktionale Anforderungen
- **Zweck:** Bestimmt Rahmenbedingungen wie Leistung, Sicherheit und Datenschutz.
- **Beispiel:** Einhaltung der DSGVO (keine öffentlich einsehbaren Klarnamen in Buchungslisten) und eine Server-Antwortzeit unter 500 ms bei Seitenaufrufen.

## …

…

## …

…
