# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @Mohamadfiras23


## 1. Ausgangssituation und Zielsetzung

Bisher werden Termine an der THM über verschiedene Wege organisiert, beispielsweise über den THM-Organizer, Moodle oder per E-Mail. Die neue Software soll die Terminvereinbarung vereinfachen und Studierenden ermöglichen, Sprechstundentermine online zu buchen. Nach der Anmeldung mit dem THM-Konto sollen nur die für den jeweiligen Studierenden relevanten Termine angezeigt werden.

## 2. Benutzergruppen und Berechtigungen
Die Software soll von Studierenden, Professoren und Sekretariaten genutzt werden, wobei jede Benutzergruppe unterschiedliche Berechtigungen erhält.

Studierende sollen nur die Termine der Professoren sehen, bei denen sie aktuell für ein Modul angemeldet sind. Sie dürfen freie Termine buchen, ändern und stornieren.

Professoren können ihre eigenen Termine erstellen und verwalten. Die Sekretariate sollen eine Übersicht über die Termine aller betreuten Professoren erhalten.

## 3. Terminbuchung und Terminverwaltung
Studierende melden sich mit ihrem THM-Konto an und sehen die Professoren ihrer aktuell belegten Module. Sie können freie Sprechstundentermine auswählen, buchen, ändern oder stornieren. Ein Termin darf nicht gleichzeitig von mehreren Studierenden gebucht werden.

Professoren können wiederkehrende Sprechstunden festlegen, beispielsweise jeden Montag von 10:00 bis 12:00 Uhr. Bei Abwesenheit können sie einzelne Termine oder ganze Zeiträume absagen.

## 4. Automatische Benachrichtigungen
Bei einer erfolgreichen Terminbuchung erhalten Studierende automatisch eine Bestätigung. Wird ein Termin durch den Professor abgesagt, informiert die Software alle betroffenen Studierenden.

Der Professor kann entweder eine automatisch erstellte Nachricht verwenden oder selbst eine persönliche Mitteilung schreiben. Über die Buchungsbestätigung können Studierende ihre Termine ändern oder stornieren.

## 5. Feiertage und Abwesenheiten
Die Software soll gesetzliche Feiertage in Hessen automatisch berücksichtigen. Beispielsweise dürfen am Pfingstmontag keine regulären Sprechstundentermine zur Buchung angeboten werden.

Professoren können bei Urlaub oder Krankheit einzelne Sprechstunden oder ganze Zeiträume absagen. Bereits gebuchte Studierende sollen darüber automatisch informiert werden.

## 6. Kalenderexport (iCal)
Nach einer erfolgreichen Terminbuchung können Studierende den Termin freiwillig als iCal-Datei herunterladen und in ihren persönlichen Kalender übernehmen.

Die Datei soll wichtige Informationen wie Datum, Uhrzeit, Dauer, Professor und Ort des Termins enthalten. Eine automatische Synchronisierung mit dem Kalender ist zunächst nicht vorgesehen.

## 7. API für KI-Agenten
Die Software soll eine Programmierschnittstelle (API) besitzen, über die KI-Agenten auf die Terminverwaltung zugreifen können.

Ein KI-Assistent kann beispielsweise freie Sprechstundentermine suchen und nach Zustimmung des Studenten einen passenden Termin buchen. Dabei darf der KI-Agent nur auf die Funktionen und Daten zugreifen, für die der jeweilige Student berechtigt ist.

