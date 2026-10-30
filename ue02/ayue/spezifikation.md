# Spezifikation des Terminplaners — Gliederung und Beispiele

---
Bearbeitet von: [aunal6006-pixel](https://github.com/aunal6006-pixel) (Kürzel: ayue)

--- 
---

## 1. Wer benutzt die SW
ST buchen Termine, DZ trägt freie Zeiten ein, SK kontrolliert.

## 2. Was muss die SW können?
Login über THM-Ecampus, Termin reservieren, Bestätigungs-E-Mail senden und Kalender-Eintrag (.ics) bereitstellen.

## 3. Wie soll die Seite aussehen?
Kalenderansicht mit Wochentagen und Uhrzeiten. Freie Termine sind grün markiert, besetzte sind rot.

## 4. Automatisierung durch AI
Bot fragt freie Termine automatisiert ab und kann selbstständig buchen.

## 5. Regeln festlegen
Kein Termin darf im selben Zeitfenster doppelt gebucht werden (für jeden anderen geblockt).

## 6. Testen

### 6.1 Testbeispiel
**Test:** ST Alpha bucht einen freien 14:00-Uhr-Termin und ST beta will auch.

Erwartetes Ergebnis: Der Termin wechselt sofort auf rot (ausgebucht), ist für ST Beta gesperrt und ST Alpha erhält eine Bestätigungs-E-Mail.

### 6.2 Beta-Phase einführen
**Testphase:** Zuerst testet nur ein Fachbereich die SW, bevor alle an der THM sie nutzen.

---

## Legende

| Abkürzung | Bedeutung |
|---|---|
| ST | Studenten   |
| DZ | Dozenten    |
| SK | Sekretariat |