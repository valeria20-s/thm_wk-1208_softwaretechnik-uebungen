# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben: @andel0

## 1. Wünsche des Auftraggebers und Rahmenbedingungen

- Die Technische Hochschule Mittelhessen benötigt eine Software, die es Lehrenden ermöglicht, Sprechstunden und Prüfungstermine für Studierende anzubieten. 
> Beispiel: Lehrender A stellt Termine jeglicher Art online und ermöglicht es Studierenden je nach Status (bspw. eingeschrieben im Kurs oder nicht) sich anzumelden:

| Lehrender | Art des Termins | Zugänglich für | Anmeldefrist | Abmeldefrist |
|---|---|---|---|---|
| Dr. Prof. Mustermann | Prüfungstermin | Nur für im Kurs eingeschriebene | 27.12.2029 bis 06.01.2030 | 10.01.2030 |  

## 2. Benutzerschnittstelle und KI-Assistenz

- Ein Chatbot im E-Campus, der dieselben Zugriffsrechte wie der Nutzer selbst hat und bei der Buchung sowie bei Fragen rund um Termine unterstützt.
> Beispiel: Der Chatbot soll auf Anfrage des Users Termine buchen und dazugehörige Informationen des Lehrenden mitteilen. Aus Sicherheitsgründen soll er jedoch keine Termine eigenständig absagen können, dies muss der User manuell ausführen.

## 3. Geschäftsprozesse und Anwendungsfälle (Use Cases)

- Der Kernprozess umfasst das Erstellen, Buchen und Verwalten von Terminen durch Lehrende und Studierende.
> Beispiel (Ablauf einer Buchung): 
> 1. Studierender ruft die Terminübersicht im E-Campus auf.
> 2. Filterung nach verfügbaren Sprechstunden von „Dr. Prof. Mustermann“.
> 3. Klick auf „Termin buchen“ -> System prüft, ob die Frist eingehalten ist und der Studierende im Kurs ist.
> 4. Bestätigung wird angezeigt und ein iCal-Eintrag generiert.
