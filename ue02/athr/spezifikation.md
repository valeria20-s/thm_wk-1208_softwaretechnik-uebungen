# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @offenbach0699

<!-- Je Abschnitt Ihrer Gliederung eine Überschrift (## für Abschnitte, ###
     für Unterabschnitte) und darunter ein Beispiel aus dem Terminplaner,
     d.h. so, wie Sie den Sachverhalt in diesem Abschnitt festhalten würden.
     Die beiden Überschriften unten sind lediglich Platzhalter. -->




## 1. Ist-Analyse und Rahmenbedingungen
Beschreibt das aktuelle Umfeld, bestehende Probleme bei der Terminvergabe sowie die technischen und organisatorischen Randbedingungen.

* **Beispiel:** Bisher erfolgt die Terminvergabe per E-Mail oder mündlich, was zu Doppelbelegungen und hohem Abstimmungsaufwand führt. Das System muss DSGVO-konform sein und die Anmeldung über das bestehende Hochschulkonto (Single Sign-On) unterstützen.

## 2. Funktionale Anforderungen (Anwendungsfälle)
Detaillierte Beschreibung aller Funktionen, die das System für Studierende, Lehrende und Sekretariate bereitstellen muss.

* **Beispiel:** **Terminbuchung durch Studierende:** Ein:e Studierende:r wählt aus den freigegebenen Zeitslots einer/eines Lehrenden einen Termin aus, gibt den Buchungsgrund an und erhält eine automatisierte Bestätigungs-E-Mail.

## 3. Schnittstellen und Systemintegration
Definition aller externen Systeme, APIs und Datenformate, mit denen der Terminplaner kommunizieren muss.

* **Beispiel:** **Kalender-Schnittstelle:** Das System tauscht Termindaten bidirektional mit dem zentralen Exchange-/Kalendersystem der Hochschule über eine REST-API im JSON-Format aus, um Konflikte zu vermeiden.

## 4. Nicht-funktionale Anforderungen und KI-Einsatz
Anforderungen an Leistung, Sicherheit, Usability sowie die genauen Grenzen für den Einsatz des KI-Agenten.

* **Beispiel:** **KI-Berechtigungen:** Der KI-Agent darf über die API eigenständig freie Termine abfragen und buchen, hat jedoch striktes Verbot, bestehende Prüfungstermine abzusagen oder zu verschieben.

## 5. Testfälle und Abnahmekriterien
Kriterien und konkrete Testfälle, anhand derer das fertige System geprüft und abgenommen wird.

* **Beispiel:** **Testfall TF-01 (Kollisionsprüfung):** Wenn zwei Studierende gleichzeitig denselben Zeitslot buchen wollen, muss das System den Slot für den ersten erfolgreichen Request reservieren und dem zweiten Nutzer einen Hinweis auf die Überschneidung anzeigen.