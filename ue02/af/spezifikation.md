# Spezifikation des Terminplaners — Gliederung und Beispiele

Mitgearbeitet haben (GitHub-Benutzernamen, auch bei Einzelarbeit): @mes-byte.

## 1 Einleitung

### 1.1 Zweck des Dokuments

Dieses Dokument beschreibt die Anforderungen an einen webbasierten Terminplaner, mit dem Studierende Sprechstundentermine bei Lehrenden der THM buchen können. Es ist die Grundlage für die Konstruktion und Implementierung durch das Entwicklerteam der THM.

### 1.2 Glossar

| Begriff | Bedeutung |
|---|---|
| Slot | buchbares Zeitfenster einer Sprechstunde, z. B. 15 Minuten |

### 1.3 Referenzen

- Gesprächsprotokolle mit der THM (TT.MM.JJJJ)

- Datenschutzrichtlinie der THM

### 1.4 Verbindlichkeit der Anforderungen

| Verbindlichkeit (Prio) | Bedeutung | Beispiel |
|---|---|---|
| **Muss** | Pflicht; ohne sie wird das System nicht abgenommen | Slot buchen |
| **Soll** | wichtig, aber verhandelbar | Erinnerung 24 Std. vorher |
| **Kann** | optional, nur wenn Zeit da ist | Export in Outlook |

## 2 Ausgangslage & Ziele

### 2.1 Ist-Situation

Sprechstunden werden aktuell per E-Mail vereinbart. Das führt zu:

- Doppelbuchungen

- langen Antwortzeiten

- Unübersichtlichkeit

- hohem manuellem Aufwand (Terminabstimmung, Einladungen verschicken, weitere Personen in CC setzen)

### 2.2 Ziele

- Z1: Studierende buchen Sprechstundentermine selbst, ohne E-Mail-Verkehr.

- Z2: Bestätigungen, Erinnerungen und Absagen werden automatisch verschickt, sodass Lehrende keinen manuellen Aufwand mehr haben.

- Z3: Doppelbuchungen sind ausgeschlossen.

### 2.3 Abgrenzung

- Raumverwaltung und Prüfungstermine sind nicht Teil von Version 1.

## 3 Nutzer & Rollen

### 3.1 Nutzergruppen

- Studierende, Lehrende, Administratoren


### 3.2 Rechte je Rolle

| Objekt | Studierende | Lehrende | Admin |
|---|---|---|---|
| Slot | R | CRUD (eigene) | CRUD (alle) |
| Buchung | CRD (eigene) | R (zu eigenen Slots) | CRUD (alle) |

C = Create, R = Read, U = Update, D = Delete. Der Admin hat globale Rechte (CRUD) auf alle Daten.

## 4 Anwendungsfälle

### 4.1 Übersicht

```text
                +------------- System Terminplaner -------------+
 Studierende ---|--- ( UC-01 Slot buchen )                       |
             \--|--- ( UC-02 Buchung stornieren )                |
 Lehrende ------|--- ( UC-03 Slots anlegen )                     |
                +------------------------------------------------+
```

Akteure stehen links, die Anwendungsfälle als Ovale ( ) im Systemrahmen; Linien zeigen, wer welchen Anwendungsfall nutzt.

### 4.2 Beschreibung der Anwendungsfälle

| UC-01 | Slot buchen |
|---|---|
| Akteur | Studierende |
| Vorbedingung | Studierende sind eingeloggt, es gibt einen freien Slot |
| Ablauf | 1. Lehrende wählen → 2. freien Slot wählen → 3. Buchung bestätigen |
| Nachbedingung | Slot ist belegt, Bestätigung per E-Mail ist versendet |
| Alternative | Slot wurde inzwischen von jemand anderem gebucht → Hinweis „Slot nicht mehr verfügbar“ |

## 5 Funktionale Anforderungen

### 5.1 Termine verwalten

| ID | Anforderung | Begründung | Bezug | Prio |
|---|---|---|---|---|
| FA-01 | Lehrende müssen Slots mit Datum, Uhrzeit, Dauer und Ort anlegen können. | Grundlage für jede Buchung | UC-03 | Muss |

### 5.2 Buchen und Stornieren

| ID | Anforderung | Begründung | Bezug | Prio |
|---|---|---|---|---|
| FA-07 | Studierende müssen eine Buchung bis 24 Std. vor Beginn stornieren können. | Lehrende können den Slot neu vergeben | UC-02 | Muss |

### 5.3 Benachrichtigungen

| ID | Anforderung | Begründung | Bezug | Prio |
|---|---|---|---|---|
| FA-10 | Das System soll 24 Std. vor dem Termin eine Erinnerung per E-Mail senden. | Weniger vergessene Termine | Z2 | Soll |

### 5.4 Fehlerfälle

| ID | Anforderung | Begründung | Bezug | Prio |
|---|---|---|---|---|
| FA-12 | Kann eine Bestätigungs-Mail nicht versendet werden, muss die Buchung trotzdem gespeichert und der Fehler protokolliert werden. | Buchung darf nicht verloren gehen | UC-01 | Muss |

## 6 Daten & Regeln

### 6.1 Datenmodell

| Objekt | Attribut | Typ | Pflicht |
|---|---|---|---|
| Slot | Beginn | Datum + Uhrzeit | ja |
| Slot | Dauer | Minuten | ja |
| Buchung | Status | gebucht / storniert | ja |

Ein Lehrender bietet beliebig viele Slots an, ein Slot hat höchstens eine Buchung, Studierende können mehrere Buchungen haben.

### 6.2 Regeln

| ID | Regel (Wenn – Dann) | Begründung | Bezug |
|---|---|---|---|
| GR-02 | Wenn Studierende bereits 2 offene Buchungen bei denselben Lehrenden haben, dann wird jede weitere Buchung abgelehnt. | Slots sollen fair verteilt werden | UC-01 |

## 7 Benutzungsoberfläche

Skizze Wochenansicht (Bezug: UC-01):

```text
+------------------------------------------------+
| Prof. Müller – Sprechstunden    < KW 45 >      |
+--------+--------+--------+--------+------------+
|        |  Mo    |  Di    |  Mi    |  ...       |
| 10:00  | [frei] | [----] | [frei] |            |
| 10:15  | [----] | [frei] | [----] |            |
+--------+--------+--------+--------+------------+
```

[frei] = grün, klickbar → öffnet Dialog „Buchung bestätigen“; [----] = belegt, grau.

## 8 Schnittstellen

| ID | System | Zweck | Richtung | Bezug |
|---|---|---|---|---|
| IF-01 | THM-Login (SSO) | Anmeldung | lesend | UC-01 |
| IF-02 | E-Mail-Server | Bestätigungen und Erinnerungen versenden | schreibend | FA-10 |

## 9 Nicht-funktionale Anforderungen

### 9.1 Performance

| ID | Anforderung | Messgröße | Prio |
|---|---|---|---|
| NFA-01 | Eine Buchung ist schnell abgeschlossen. | ≤ 5 Sekunden bei 500 gleichzeitigen Nutzern | Muss |

### 9.2 Sicherheit und Datenschutz

| ID | Anforderung | Messgröße | Prio |
|---|---|---|---|
| NFA-03 | Personenbezogene Daten werden DSGVO-konform gespeichert. | Speicherung nur auf Servern der THM | Muss |

### 9.3 Usability und Barrierefreiheit

| ID | Anforderung | Messgröße | Prio |
|---|---|---|---|
| NFA-05 | Die Oberfläche ist barrierefrei bedienbar. | vollständig per Tastatur und Screenreader nutzbar | Soll |

## 10 Randbedingungen

| ID | Randbedingung | Begründung |
|---|---|---|
| RB-01 | Webanwendung, auch mobil nutzbar | Studierende buchen oft unterwegs |
| RB-02 | Oberfläche auf Deutsch und Englisch | internationale Studierende an der THM |

## 11 Abnahmekriterien

| ID | Gegeben | Wenn | Dann | Bezug |
|---|---|---|---|---|
| AK-01 | ein freier Slot | zwei Studierende ihn gleichzeitig buchen | erhält genau eine Person die Buchung | Z3 |

## 12 Offene Punkte & Ansprechpartner

| Nr. | Frage | Entscheidet | Bis |
|---|---|---|---|
| OP-1 | Dürfen Gasthörer buchen? | Fachbereich | KW 46 |