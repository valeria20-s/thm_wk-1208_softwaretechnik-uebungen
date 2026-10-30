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

- **Kürzel statt Klarname.** Dieses Repository ist öffentlich. Wählen Sie ein
  Kürzel, das Sie selbst wiedererkennen, und behalten Sie es über alle
  Übungen bei. Es wird Teil von Datei- und Branchnamen: nur Kleinbuchstaben
  und Ziffern, keine Umlaute, keine Leerzeichen. Liegt unter
  `ue01/steckbriefe/` schon eine Datei mit Ihrem Kürzel, hängen Sie eine
  Ziffer an.
- **Öffentlich ist mehr als das Kürzel.** Am Pull Request steht Ihr
  GitHub-Benutzername, in jedem Commit stehen Name und E-Mail-Adresse aus
  Ihrer Git-Einrichtung. Wie Sie Ihre Adresse verbergen, steht in
  [Aufgabe 0 des Übungsblatts](https://carstenlucke.github.io/thm_wk-1208_softwaretechnik/ue01-git-github/#aufgabe-0--einrichten). Schreiben Sie auch in Ihre Dateien nichts, was nicht
  jeder lesen darf — keine Matrikelnummer, keine Anschrift.
- **Nur eigene Dateien.** Sie ändern ausschließlich, was Sie selbst angelegt
  haben; Vorlagen und die Dateien anderer bleiben unberührt. So kommen sich
  die Pull Requests nicht in die Quere.
- **Nicht auf `main` arbeiten.** `main` Ihres Forks folgt allein dem Stand
  dieses Repositorys; nur so lässt er sich später abgleichen.
- **Ein Anliegen je Pull Request**, mit einem Titel, der sagt, was sich
  ändert.
- **Aussagekräftige Commit-Nachrichten**, etwa `Steckbrief für mmus anlegen`.
