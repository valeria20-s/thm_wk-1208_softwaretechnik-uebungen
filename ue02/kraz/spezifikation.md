# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @kamyabrz

## 1. Ziel und Ausgangslage

Hier steht kurz, warum die THM den Terminplaner will und was heute nicht gut läuft.

> Heute werden Sprechstunden per E-Mail, mit Listen an der Bürotür oder mit Doodle vereinbart. Das ist unübersichtlich. Der Terminplaner soll alles an einem Ort bündeln.

## 2. Wer benutzt das System?

Eine Liste der Benutzergruppen und was sie im System machen dürfen.

| Rolle | Was sie macht |
|---|---|
| Lehrende | bieten Sprechstunden und Prüfungstermine an |
| Studierende | buchen und stornieren Termine |
| Sekretariat | sieht alle Termine ihres Fachbereichs und kann sie ändern |
| KI-Agent | fragt freie Termine ab und bucht im Auftrag einer Person |

## 3. Funktionen

Jede Funktion wird Schritt für Schritt beschrieben, so wie ein Benutzer sie erlebt.

### 3.1 Sprechstunde anbieten

1. Lehrende meldet sich mit dem Hochschulkonto an.
1. Sie legt einen Zeitraum fest, z.B. dienstags 10–12 Uhr, in 15-Minuten-Slots.
1. Die Slots sind danach für Studierende sichtbar.

### 3.2 Termin buchen

1. Student meldet sich an und sucht die Lehrende.
1. Er wählt einen freien Slot und gibt kurz den Grund an.
1. Er bekommt eine Bestätigung und eine iCal-Datei zum Herunterladen.

### 3.3 Termin absagen

Ein Student kann bis 2 Stunden vorher absagen. Der Slot ist danach wieder frei.

## 4. Daten

Welche Angaben zu einem Termin gehören und wie sie zusammenhängen.

| Angabe | Beispiel |
|---|---|
| Datum und Uhrzeit | 04.11.2026, 10:15–10:30 |
| Art | Sprechstunde oder Prüfung |
| Lehrende | Prof. Lucke |
| Raum | A1.0.01 |
| gebucht von | ein Student (oder noch frei) |

Ein Termin gehört immer zu genau einer Lehrenden und einem Raum. Eine Lehrende hat viele Termine.

## 5. Bedienoberfläche

Eine kurze Beschreibung der wichtigsten Seiten, am besten mit Skizze.

- **Startseite:** Suchfeld für Lehrende und eine Liste "Meine Termine"
- **Buchungsseite:** Kalender der Woche, freie Slots grün, belegte grau
- **Übersicht fürs Sekretariat:** Tabelle mit allen Terminen des Tages

## 6. Schnittstellen zu anderen Systemen

Mit welchen Systemen der Terminplaner Daten austauscht.

- **Hochschulkonto:** Anmeldung läuft über das bestehende THM-Login, kein eigenes Passwort.
- **iCal-Datei:** jeder gebuchte Termin kann als `.ics`-Datei heruntergeladen werden.
- **API für KI-Agenten:** ein Agent darf freie Termine abfragen und buchen, aber keine Prüfungstermine absagen.

## 7. Rechte und Datenschutz

Wer was sehen darf.

Studierende sehen nur, ob ein Slot frei ist, aber nicht, wer ihn gebucht hat. Den Grund für den Termin sieht nur die Lehrende.

## 8. Weitere Anforderungen

Dinge wie Geschwindigkeit, Verfügbarkeit oder Bedienbarkeit.

- Das System soll auch auf dem Handy gut funktionieren.
- Eine Buchung soll in weniger als 2 Sekunden bestätigt sein.
- Auch wenn zu Semesterbeginn viele gleichzeitig buchen, darf kein Slot doppelt vergeben werden.

## 9. Abnahme und Testfälle

Woran man am Ende sieht, ob das System macht, was vereinbart wurde.

| Testfall | Erwartetes Ergebnis |
|---|---|
| Zwei Studierende buchen gleichzeitig denselben Slot | nur einer bekommt ihn, der andere sieht eine Meldung |
| KI-Agent versucht, einen Prüfungstermin abzusagen | das System lehnt ab |

## 10. Was (noch) nicht dazugehört

Damit das Entwicklerteam weiß, was es nicht bauen muss.

- Direkte Eintragung in Outlook oder andere Kalender kommt erst später.
- Raumbuchung ist nicht Teil dieser Version.
