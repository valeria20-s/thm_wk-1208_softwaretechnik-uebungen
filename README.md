# Softwaretechnik — Übungsrepository

Dieses Repository gehört zu den Übungen der Veranstaltung **Softwaretechnik**
(THM, Campus Friedberg, Fachbereich MND). Hier reichen Sie ein, was in den
Übungen entsteht — auf dem Weg, auf dem in Softwareprojekten gearbeitet wird:
über einen eigenen Fork, einen Branch und einen Pull Request.

## Aufbau

Jede Übung hat ein eigenes Verzeichnis mit einer eigenen `README.md`, die
sagt, was dort einzureichen ist.

| Verzeichnis | Übung |
|---|---|
| [`ue01/`](ue01/) | Erste Schritte mit Git und GitHub |
| [`ue02/`](ue02/) | Das Projektmodell am Fall |
| [`ue03/`](ue03/) | Anforderungen an den Terminplaner |
| [`ue04/`](ue04/) | Einen Coding Agent einrichten |

## So reichen Sie etwas ein

1. Legen Sie einmalig einen **Fork** dieses Repositorys an und **klonen** Sie
   ihn auf Ihren Rechner.
2. Legen Sie für jedes Vorhaben einen eigenen **Branch** an.
3. Halten Sie Ihre Änderungen als **Commits** fest und übertragen Sie sie per
   **Push** in Ihren Fork.
4. Stellen Sie einen **Pull Request** an dieses Repository.

Den Weg Schritt für Schritt beschreibt das
[Übungsblatt zur Übung 1](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/).

## Vor jeder weiteren Übung

Dieses Repository wächst mit jeder Übung. Bringen Sie vorher Ihren Fork und
Ihren Rechner auf den neuen Stand:

1. Klicken Sie auf der Startseite Ihres Forks auf **Sync fork → Update
   branch**.
2. Holen Sie den neuen Stand aus dem Fork auf Ihren Rechner:

   ```console
   $ git switch main
   $ git pull
   ```

Den Branch für die neue Übung zweigen Sie erst danach ab.

## Spielregeln

- **Ihr GitHub-Benutzername als Kennung.** Ihre Datei- und Verzeichnisnamen
  sowie Ihre Branches tragen Ihren GitHub-Benutzernamen, und zwar in
  Kleinbuchstaben: Aus `MMustermann` wird `mmustermann`. Anders als ein
  selbst gewähltes Kürzel ist er eindeutig, und er steht ohnehin an jedem
  Pull Request. Ihren Benutzernamen sehen Sie auf GitHub, wenn Sie oben
  rechts auf Ihr Profilbild klicken.
- **Öffentlich ist mehr als der Benutzername.** In jedem Commit stehen Name
  und E-Mail-Adresse aus Ihrer Git-Einrichtung. Wie Sie Ihre Adresse
  verbergen, steht in
  [Aufgabe 0 des Übungsblatts](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/#aufgabe-0--einrichten).
  Schreiben Sie auch in Ihre Dateien nichts, was nicht jeder lesen darf —
  keine Matrikelnummer, keine Anschrift.
- **Nur eigene Dateien.** Sie ändern ausschließlich, was Sie selbst angelegt
  haben; Vorlagen und die Dateien anderer bleiben unberührt. So kommen sich
  die Pull Requests nicht in die Quere.
- **Nicht auf `main` arbeiten.** `main` Ihres Forks folgt allein dem Stand
  dieses Repositorys; nur so lässt er sich später abgleichen.
- **Ein Anliegen je Pull Request**, mit einem Titel, der sagt, was sich
  ändert.
- **Aussagekräftige Commit-Nachrichten**, etwa `Steckbrief für mmustermann anlegen`.

Arbeiten Sie mit einem KI-Agenten, gelten die Spielregeln auch für ihn. Die
Datei [`AGENTS.md`](AGENTS.md) fasst sie für Agenten zusammen; opencode und
andere Coding Agents lesen sie, wenn sie in diesem Repository gestartet
werden.
