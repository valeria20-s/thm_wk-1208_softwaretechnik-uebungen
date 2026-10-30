# Spezifikation: Terminplaner für die THM

**Beteiligte:** zcoel

## 1. Zielsetzung und fachliche Anforderungen
Was soll das System leisten? Überblick über den Zweck des Systems und was der Terminplaner alles leisten muss. (Systemspezifikation).

*Beispiel:*  
Die Hochschule möchte eine Software zur Planung und Vereinbarung von Terminen: Lehrende bieten Sprechstunden und Prüfungstermine an, Studierende buchen sie, und die Sekretariate behalten den Überblick. (Beispiel ist aus dem Fall der Übung 2) Nach Buchung soll ein Bestätigungsdialog angezeigt werden.

## 2. Benutzerrollen, Authentizität und Autorisierung
Festlegung, wer Zugriff auf das System hat (Authentifizierung) und welche Aktionen die jeweiligen Rollen ausführen dürfen (Autorisierung).

*Beispiel:*  
- *Lehrende:* Dürfen eigene Sprechstundenblöcke anlegen, bearbeiten, stornieren und Anmeldungen einsehen. (haben mehr Rechte als Studenten)
- *Studierende:* Dürfen sich über ihr THM-Konto anmelden, freie Termine buchen und eigene Buchungen zurückziehen.

## 3. Systemarchitektur(Systemkonstruktion), Infrastruktur und Schnittstellen. 
Rahmenbedingungen zur technischen Einbettung (Server, Schnittstellen und Anmeldedienste). 

*Beispiel:*  
- *Infrastruktur:* Betrieb ausschließlich auf internen Hochschulservern zur Wahrung des Datenschutzes.
- *Schnittstellen:* Anbindung an das Single-Sign-On (SSO/LDAP) der THM sowie Bereitstellung einer REST-API für berechtigte KI-Agenten.

## 4. Nicht-funktionale Anforderungen/Wünsche und Kapazität
Vorgaben zu Nutzerzahlen, Antwortzeiten und Verfügbarkeit.

*Beispiel Anforderungen:*  
- *Kapazität:* Das System muss für bis zu 15.000 aktive Nutzerkonten ausgelegt sein und Lastspitzen (z. B. zu Beginn der Prüfungsanmeldephase mit bis zu 200 gleichzeitigen Buchungen) verzögerungsfrei verarbeiten. Terminplaner soll für Benutzungsberechtigte jederzeit Verfügbar sein 


