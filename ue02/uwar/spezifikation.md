# Spezifikation Terminplaner — Gliederungsentwurf

**Mitgearbeitet (GitHub-Benutzernamen):** Umerwarraich99, Mazm96

---

## 1 Ziel und Abgrenzung

*Ohne Zielbild gewichtet das Team jede Einzelanforderung falsch. Die Abgrenzung gehört an den Anfang, nicht ans Ende — sonst baut jemand zwei Wochen lang etwas, das wir gar nicht wollen.*

**Beispiel** — nummerierte Liste, damit spätere Abschnitte darauf verweisen können:

- `/M10/` Studierende buchen Sprechstundentermine selbstständig online, ohne E-Mail-Verkehr.
- `/W20/` Gebuchte Termine lassen sich als `.ics` in den eigenen Kalender übernehmen.
- `/A30/` Nicht im Umfang: Raumverwaltung. Der Raum ist Freitext am Termin, Raumkollisionen prüft das System nicht.

---

## 2 Begriffe

*Ab hier steht fest, was „Slot", „Termin" und „Buchung" bedeuten. Jeder folgende Abschnitt benutzt diese Wörter, also muss die Definition davor stehen.*

**Beispiel** — Tabelle, im ganzen Dokument verbindlich:

| Begriff | Bedeutung |
|---|---|
| Slot | Freigegebenes Zeitfenster fester Länge (Standard 15 min), noch ohne Buchung. |
| Buchung | Verbindliche Zuordnung genau einer studierenden Person zu genau einem Slot. |
| Termin | Oberbegriff für Slot + zugehörige Buchung. Wird allein nie als Zustand verwendet. |

---

## 3 Rollen, Rechte und Anmeldung

*Fast jede spätere Anforderung lautet „Rolle X darf Y". Die Anmeldung steht direkt dahinter, weil sie klärt, woher die Rollen technisch kommen.*

### 3.1 Rollen und Sichtbarkeit
### 3.2 Herkunft der Identität

**Beispiel** — Tabelle, Sehen und Ändern getrennt:

| Rolle | Sieht | Ändert |
|---|---|---|
| Studierende/r | freie Slots, eigene Buchungen | eigene Buchung (stornieren) |
| Lehrende/r | eigene Slots inkl. Namen und Anliegen der Buchenden | eigene Slots und deren Buchungen |
| Sekretariat | Slots der vertretenen Lehrenden, ohne Anliegen-Text | Slots im Auftrag anlegen |
| Admin | Stammdaten, keine Anliegen-Texte | Rollen und Vertretungen |

Zu 3.2: Anmeldung über den THM-Account (CAS/Shibboleth). Der Terminplaner prüft kein Passwort und führt keine eigene Benutzerverwaltung; die Rolle ergibt sich aus dem gelieferten Status.

---

## 4 Daten und Lebensdauer

*Die Löschregeln hängen direkt an den Feldern, deshalb stehen sie hier statt in einem eigenen Datenschutzabschnitt.*

### 4.1 Datenmodell
### 4.2 Aufbewahrung und Löschung

**Beispiel** — beschriebene Skizze mit Kardinalitäten:

> **Person** (id, kennung, name, mail, rolle) — eine lehrende Person erzeugt `0..*` **Slot**
> (id, beginn, dauer_min, raum, status ∈ {frei, gebucht, abgesagt}). Ein Slot trägt `0..1`
> **Buchung** (id, erstellt_am, anliegen, quelle ∈ {web, agent}), eine Buchung gehört zu genau
> `1` studierenden Person. Stornieren setzt den Status, es löscht nichts.

Zu 4.2: Der Anliegen-Text wird 30 Tage nach Slot-Ende gelöscht, der Termin selbst nach 6 Monaten. Bei Exmatrikulation wird die Person anonymisiert, die Buchung bleibt als Zählwert erhalten.

---

## 5 Funktionen

*Der Kern. Nutzt die Rollen aus 3 und die Objekte aus 4.*

### 5.1 Übersicht
### 5.2 Anwendungsfälle im Detail

**Beispiel** — Kurzschablone je Anwendungsfall:

> **UC-03 Termin buchen** · *Akteur:* Studierende/r · *Vorbedingung:* angemeldet, Slot ist frei.
> *Ablauf:* Lehrende/n wählen → freie Slots der nächsten 14 Tage → Slot + Anliegen (max. 500 Zeichen) → System bestätigt, Mail an beide.
> *Ausnahme:* Slot inzwischen belegt → Meldung, Rücksprung, keine Buchung.

---

## 6 Regeln und Randfälle

*Diese Regeln gelten quer über mehrere Funktionen aus 5. Würde ich sie dort verstreuen, vergisst das Team sie beim Verschieben — deshalb stehen sie einmal zentral.*

**Beispiel** — nummerierte Liste, jede Regel einzeln testbar:

- `GR-1` Ein Slot trägt höchstens eine bestätigte Buchung. Bei gleichzeitigem Zugriff gewinnt die erste bestätigte Transaktion, die zweite wird abgelehnt.
- `GR-2` Stornieren bis 24 h vor Beginn; danach nur durch die/den Lehrende/n.
- `GR-3` Sagt ein/e Lehrende/r ab, werden alle Buchungen der Sprechstunde storniert und alle Betroffenen benachrichtigt.

---

## 7 Schnittstellen

*iCal und Agenten-API sind derselbe Zugang wie die Oberfläche, nur ohne Mensch davor.*

### 7.1 iCal-Export
### 7.2 API für KI-Agenten

**Beispiel** — Liste, je Schnittstelle die bindenden Festlegungen:

- **iCal** nach RFC 5545, Abo-Link je Person; UID bleibt über Änderungen stabil, Zeitzone `Europe/Berlin`, Absage als `STATUS:CANCELLED` statt Löschen.
- **Agenten-API:** lesen und buchen erlaubt, stornieren nur durch den Menschen. Der Agent handelt im Namen einer Person, die Buchung wird mit `quelle = agent` gekennzeichnet, max. 10 Anfragen/Minute.

---

## 8 Qualitätsanforderungen

*„Wie gut" setzt voraus, dass „was" feststeht.*

**Beispiel** — Tabelle; jede Anforderung mit Messvorschrift, sonst nicht prüfbar:

| Nr. | Anforderung | Messung |
|---|---|---|
| `NFR-1` | Wochenansicht lädt in < 2 s | 200 gleichzeitige Sitzungen, 95 %-Quantil |
| `NFR-2` | Bedienbar ab 360 px Breite | Firefox, Chrome, Safari in aktueller Version |
| `NFR-3` | Studierende sehen nie fremde Namen oder Anliegen | Rollentest gegen alle Views und API-Endpunkte |

---

## 9 Weitere Abschnitte ohne Beispiel

Aus Zeitgründen nur benannt:

- Oberfläche
- Abnahme und Testfälle
- Offene Punkte und Annahmen

Die offenen Punkte würde ich in der echten Spezifikation zuerst füllen — sie zeigen dem Team, was es aus diesem Dokument nicht entscheiden kann.