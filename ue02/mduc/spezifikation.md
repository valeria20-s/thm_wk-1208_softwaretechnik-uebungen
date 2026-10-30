# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @mauritzduchardt

## 1. Ziel und Benutzerrollen

In diesem Abschnitt wird festgehalten, wer das System nutzen darf und welche Rechte die einzelnen Rollen haben.

*Beispiel:*  
- **Studierende:** Dürfen freie Sprechstundentermine suchen, buchen und eigene Termine absagen.  
- **Lehrende:** Geben freie Zeitslots frei, sehen Teilnehmerlisten ein und können Termine verschieben.  
- **Sekretariat:** Kann Termine im Namen von Lehrenden anlegen oder bearbeiten.  
- **KI-Agent:** Darf automatisiert freie Slots abfragen und Termine für Studierende reservieren, aber keine Termine absagen.

---

## 2. Fachliche Abläufe (Use Cases)

Hier wird Schritt für Schritt beschrieben, wie die wichtigsten Vorgänge im System ablaufen und wie mit Ausnahmen umgegangen wird.

*Beispiel: Sprechstundentermin buchen*  
1. Ein Studierender wählt eine Lehrperson und einen verfügbaren Zeitslot aus.  
2. Der Studierende gibt seinen Namen, die THM-Mailadresse und kurz den Grund des Termins ein.  
3. Das System prüft die Verfügbarkeit, sperrt den Slot für andere und schickt eine Bestätigung an beide Personen.  
*Fehlerfall:* Wurde der Slot während der Eingabe bereits vergeben, meldet das System den Konflikt und schlägt freie Nachbar-Slots vor.

---

## 3. Benutzeroberfläche und Eingabemasken

Dieser Abschnitt zeigt anhand einfacher Skizzen oder Beschreibungen, wie die Seiten für den Nutzer aufgebaut sein müssen.

*Beispiel: Buchungsansicht für Studierende*  
- Oben gibt es ein Dropdown-Menü zur Auswahl von Fachbereich und Lehrperson.  
- Darunter liegt ein Monatskalender: Tage mit freien Slots sind grün markiert.  
- Beim Klick auf einen Tag erscheint eine Liste der freien Uhrzeiten.  
- Am Ende folgt ein einfaches Eingabeformular mit Pflichtfeldern (Name, Matrikelnummer, Anliegen) und dem Button „Verbindlich buchen“.

---

## 4. Fachliches Datenmodell

Hier wird festgelegt, welche Daten das System verwalten muss und wie diese fachlich zusammenhängen.

*Beispiel:*  
- **Termin:** Besteht aus Datum, Uhrzeit (von/bis), Status (frei, reserviert, abgesagt), Raum oder Zoom-Link und Fachbereich.  
- **Beziehungen:**  
  - Ein Termin gehört immer genau zu einer Lehrperson und einem Raum.  
  - Ein gebuchter Termin ist genau einem Studierenden zugeordnet.  
  - Eine Lehrperson kann mehrere freie Termine an einem Tag anbieten.

---

## 5. Externe Schnittstellen und Berechtigungen

Beschreibt, wie das System mit bereits vorhandenen Systemen der THM und automatisierten Schnittstellen kommuniziert.

*Beispiel:*  
- **THM-Kalendersystem:** Gebuchte Termine werden automatisch als `.ics`-Kalendereintrag an den Mailserver der THM übertragen, damit sie im Outlook-Kalender der Lehrperson auftauchen.  
- **KI-Agenten-API:** Der Agent erhält Lesezugriff auf freie Termine und darf Buchungsanfragen senden. Versucht der Agent Prüfungstermine abzusagen, wird die Anfrage mit einem Fehlercode abgewiesen.

---

## 6. Qualitätsanforderungen und Randbedingungen

Definiert Rahmenbedingungen, die das System einhalten muss, damit es im Hochschulalltag zuverlässig und sicher läuft.

*Beispiel:*  
- **Datenschutz:** Die Anmeldedaten und Notizen zu einem Termin werden 30 Tage nach Stattfinden des Termins automatisch gelöscht.  
- **Performance:** Die Kalenderübersicht muss auch während der Stoßzeiten innerhalb von wenigen Sekunden laden.

---

## 7. Testfälle zur Abnahme

Konkrete Szenarien, mit denen am Ende geprüft wird, ob das fertige System die Anforderungen der Spezifikation erfüllt.

*Beispiel: Testfall „Verhinderung von Doppelbuchungen“*  
- **Ausgangslage:** Ein Zeitslot am Montag um 10:00 Uhr bei Prof. Müller ist frei.  
- **Ablauf:** Zwei Studierende klicken zeitgleich im Browser auf „Verbindlich buchen“ für genau diesen Slot.  
- **Erwartetes Ergebnis:** Nur einer der beiden erhält die Buchungsbestätigung. Der andere erhält sofort die Meldung, dass der Termin bereits vergeben ist, und es entsteht keine Doppelbelegung.