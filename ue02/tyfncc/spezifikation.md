
# Spezifikation des Terminplaners – Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @tyfnCC

## 1. Wünsche und Ziele der THM

Die THM wünscht sich eine Software zur Planung und Vereinbarung von Terminen. Lehrende sollen Sprechstunden und Prüfungstermine anbieten, Studierende diese buchen und Sekretariate den Überblick behalten können.

**Beispiel:** Ein Lehrender stellt einen Sprechstundentermin bereit, den ein Studierender über die Software bucht.

## 2. Benutzergruppen und ihre Aufgaben

Die Spezifikation soll festhalten, welche Funktionen Studierende, Lehrende und Sekretariate benötigen und wer welche Informationen sehen oder bearbeiten darf.

**Beispiel:** Studierende buchen verfügbare Termine; Lehrende verwalten ihr Angebot; das Sekretariat erhält eine Übersicht.

## 3. Anmeldung über das Hochschulkonto

Die Software soll mit dem vorhandenen Hochschulkonto bedienbar sein. Dazu muss geklärt werden, wie die Anmeldung technisch ermöglicht wird.

**Beispiel:** Studierende melden sich mit ihrem THM-Hochschulkonto an, statt ein zusätzliches Benutzerkonto anzulegen.

## 4. Terminverwaltung und Kalender

Die Software soll Termine zunächst als iCal-Datei zum Herunterladen anbieten. Eine direkte Integration in die Kalender der Beteiligten ist als spätere Erweiterung vorgesehen.

**Beispiel:** Nach einer Buchung lädt ein Studierender eine iCal-Datei herunter und fügt den Termin seinem Kalender hinzu.

## 5. Programmierschnittstelle (API)

Das System soll eine API besitzen, über die künftig andere Anwendungen beziehungsweise KI-Agenten auf vorgesehene Funktionen zugreifen können. Die erlaubten Vorgänge müssen beschrieben werden.

**Beispiel:** Über die API könnten verfügbare Termine abgefragt und – bei entsprechender Berechtigung – gebucht werden.

## 6. Benötigte Informationen und Ressourcen

Für die Umsetzung werden Angaben zu den Hochschulkonten und zu den benötigten Daten von Lehrenden und Studierenden gebraucht. Welche Daten tatsächlich erforderlich sind, muss mit der THM geklärt werden.

**Beispiel:** Die THM erläutert, ob für eine Buchung Name und Hochschul-E-Mail-Adresse genügen oder weitere Angaben benötigt werden.

## 7. Datenschutz und Sicherheit

Personenbezogene Daten müssen geschützt werden. Außerdem sind die Berechtigungen und vertraglichen Rahmenbedingungen für den Zugriff auf Hochschulsysteme und Daten zu klären.

**Beispiel:** Studierende dürfen keine persönlichen Buchungsdaten anderer Studierender einsehen.

## 8. Zeitplanung und Budget

Vor der Umsetzung muss geklärt werden, wie viel Zeit und Budget zur Verfügung stehen und ob es Zeiträume gibt, in denen bestimmte Arbeiten nicht möglich sind.

**Beispiel:** Die THM nennt einen gewünschten Fertigstellungstermin und das verfügbare Budget; mögliche Einschränkungen werden im Projektplan berücksichtigt.