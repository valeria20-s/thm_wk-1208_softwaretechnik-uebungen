# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @nivbl10

## 1. Ziel und Abgrenzung

**Beispiel:** Der Terminplaner ersetzt E-Mail, Bürotür-Listen, Doodle und DFN-Terminplaner für Sprechstunden und Prüfungstermine. Später kommt die Kalenderintegration, Raumplanung gehört nicht dazu.

## 2. Rollen und Rechte

**Beispiel:** Lehrende legen Angebote an, Studierende buchen, Sekretariate sehen die Termine der zugeordneten Lehrenden.

## 3. Schnittstellen

### 3.1 Hochschulkonto

**Beispiel:** Anmeldung nur über das THM-Hochschulkonto.

### 3.2 iCal-Export

**Beispiel:** Termine gibt es als iCal-Datei zum Herunterladen.

### 3.3 API für KI-Agenten

**Beispiel:** Die API bietet dieselben Funktionen wie die Oberfläche, KI-Agenten handeln nur mit den Rechten des angemeldeten Nutzers.

## 4. Funktionale Anforderungen

Der Kern des Dokuments: Was kann das System? Jede Anforderung bekommt eine Nummer, damit man sich darauf beziehen kann.

**Beispiel:**

- Nr. 1: Lehrende können Termine anbieten, zum Beispiel für ihre Sprechstunde.
- Nr. 2: Studierende können einen freien Termin buchen.
- Nr. 3: Nach der Buchung bekommen beide eine Bestätigung per E-Mail.

## 5. Geschäftsregeln

**Beispiel:** Höchstens [2] offene Buchungen pro Studierendem und Lehrendem, Stornierung bis [24] Stunden vor dem Termin.

## 6. Datenschutz und Sicherheit

**Beispiel:** Studierende sehen nur eigene Buchungen, personenbezogene Daten werden nach [12] Monaten gelöscht.

## 7. Offene Punkte und Änderungshistorie

**Beispiel:** Ansprechperson der THM, Einführungstermin und Werte der Geschäftsregeln.