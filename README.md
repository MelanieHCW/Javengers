//* # Mein Projekt

Mein erstes Git-Repository.

---

## So arbeitest du mit diesem Repository

### Einmalig: Einrichten

1. GitHub-Konto anlegen und die Einladung zum Repository annehmen (kommt per E-Mail).
2. Git installieren: https://git-scm.com
3. Name und E-Mail für Commits festlegen:

   ```bash
   git config --global user.name "Dein Name"
   git config --global user.email "deine@email.de"
   ```

4. Repository auf den eigenen Computer herunterladen:

   ```bash
   git clone https://github.com/DEIN-NAME/mein-projekt.git
   cd mein-projekt
   ```

### Für jede neue Aufgabe

```bash
# 1. Neuesten Stand holen
git checkout main
git pull

# 2. Eigenen Branch anlegen (Name beschreibt die Aufgabe)
git checkout -b mein-branch-name

# 3. Dateien bearbeiten, dann Änderungen speichern
git status
git add .
git commit -m "Kurze Beschreibung der Änderung"

# 4. Branch zu GitHub hochladen
git push -u origin mein-branch-name
```

5. Auf GitHub auf **„Compare & pull request“** klicken, kurz beschreiben, was du gemacht hast, und eine Person aus dem Team als **Reviewer** auswählen.
6. Nach der Prüfung wird der Pull Request mit **„Merge pull request“** in `main` übernommen.

### Regeln

- **Nie direkt auf `main` arbeiten.** Immer einen eigenen Branch anlegen.
- **Vor dem Arbeiten immer `git pull`**, dann gibt es weniger Konflikte.
- **Kleine, häufige Commits** mit verständlichen Nachrichten.
- Bei einem **Merge-Konflikt**: In der Datei die Stellen zwischen `<<<<<<<` und `>>>>>>>` bereinigen, speichern, dann `git add .` und `git commit`.

### Wichtige Befehle auf einen Blick

| Befehl | Was er macht |
|---|---|
| `git status` | Zeigt, was sich geändert hat |
| `git pull` | Holt die Änderungen der anderen |
| `git checkout -b name` | Neuen Branch anlegen und wechseln |
| `git checkout name` | Zu einem Branch wechseln |
| `git add .` | Alle Änderungen für den Commit auswählen |
| `git commit -m "…"` | Änderungen speichern |
| `git push` | Eigene Commits zu GitHub hochladen |
| `git log --oneline` | Versionsgeschichte anzeigen |
