# Bonusmodul: Kollaboratives Arbeiten mit GitHub III

- **Kurs:** rstatsZH - Data Science mit R (rstatszh-k012)
- **Datum:** Dienstag, 21. Juli 2026
- **Dauer:** 60 Minuten
- **Format:** Übungsblock, vier Teilnehmende (drei Lernende plus Lars)
- **Folien:** [bonus-github-iii.html](https://rstatszh-k012.github.io/website/folien/bonus-github-iii.html)
- **Modulseite:** [bonus-github-iii.html](https://rstatszh-k012.github.io/website/module/bonus-github-iii.html)

## Lernziele

- Die Lernenden können eine Branch erstellen, darauf committen und einen Pull Request gegen `main` öffnen.
- Die Lernenden können einen Pull Request einer anderen Person reviewen (durchsehen) und mit mindestens einem Kommentar kommentieren.
- Die Lernenden können erklären, wann ein Merge-Konflikt entsteht, und einen Konflikt in einer gemeinsam bearbeiteten Datei auflösen.

## Aufbau

- Alle vier Personen sind in einer GitHub-Organisation und haben Schreibrecht auf ein gemeinsames Repository.
- Ein gemeinsamer Bericht (`bericht.qmd`): Titelblock oben, darunter vier Abschnitte, einer pro Person.
- Vier Issues, eines pro Person, klar zugewiesen.
- Das Team-Repository (`team-lila`) wird zu Beginn gemeinsam von GitHub nach Posit Cloud geklont (New Project from Git Repository).
- Branch-Namenskonvention: `issue-N-<slug>` (ein Slug ist ein einzelnes Wort, das das Issue beschreibt, zum Beispiel `methoden`).
- Branch-Schutz auf `main`: ein Pull Request und mindestens eine Review sind nötig.

## Rollen

- Lars ist Admin und merged die Pull Requests.
- Jeder Pull Request wird von einer anderen Person reviewt, nie der eigene.
- Bei jedem Schritt wechseln wir zwischen "Ich bin dran" (Lars zeigt es vor) und "Ihr seid dran" (die Lernenden machen es selbst mit einem Countdown).

## Ablauf (60 Minuten)

- **0 bis 10 Min - Einstieg und Repository klonen**
    - Organisation und Bericht zeigen.
    - Wir sind dran (gemeinsam): auf GitHub das Team-Repository `team-lila` öffnen, Code-URL kopieren, in Posit Cloud New Project, New Project from Git Repository, URL einfügen, bis `bericht.qmd` sichtbar ist.
    - Das eigene Issue gemeinsam suchen (Reiter Issues, das zugewiesene Issue finden, den Abschnitt lesen).
- **10 bis 20 Min - Branch erstellen**
    - 5 Min: Lars zeigt es vor.
    - 5 Min: Lernende erstellen eine Branch `issue-N-<slug>` und wechseln darauf (lokal oder auf posit.cloud).
- **20 bis 30 Min - Quiet Mode**
    - 10 Min: Lernende schreiben den eigenen Abschnitt in `bericht.qmd` und committen auf die eigene Branch.
- **30 bis 40 Min - Pull Request öffnen**
    - 5 Min: Lars zeigt es vor.
    - 5 Min: Lernende öffnen einen Pull Request gegen `main`, markieren eine andere Person als Reviewer und verlinken das Issue (zum Beispiel `Closes #N`).
- **40 bis 50 Min - Review**
    - 5 Min: Lars zeigt eine Review vor.
    - 5 Min: Lernende öffnen den zugewiesenen Pull Request, lesen die Änderungen (Files changed), hinterlassen mindestens einen Kommentar und geben die Review frei.
- **50 bis 55 Min - Live-Merge**
    - Lars merged die Pull Requests der Reihe nach gemeinsam mit der Gruppe.
    - Falls ein Merge-Konflikt entsteht, lösen wir ihn gemeinsam auf.
- **55 bis 60 Min - Fragerunde**
    - Offene Fragen klären.

## Merge-Konflikte (Backup-Erklärung)

- Ein Konflikt entsteht, wenn zwei Branches dieselbe Stelle einer Datei unterschiedlich ändern. Git kann nicht selbst entscheiden und bittet uns um die Entscheidung.
- Git fügt drei Markierungen ein: `<<<<<<<`, `=======` und `>>>>>>>`.
- Auflösen: die Markierungszeilen löschen, die gewünschte Version behalten (oder beide Einträge), speichern, committen und den Merge abschliessen.

## Reflexion

- Wozu dienen Branches, wenn mehrere Personen am selben Repository arbeiten?
- Wie hilft eine Review dabei, Probleme früh zu erkennen?
- Wann kann ein Merge-Konflikt entstehen, und was bedeutet er?

## Vorbereitung durch Lars

- Gemeinsames Repository mit `bericht.qmd` (Titelblock plus vier Abschnitte) aufsetzen.
- Vier Issues erstellen und je einer Person zuweisen.
- Branch-Schutz auf `main` aktivieren (Pull Request plus mindestens eine Review nötig).
- Alle Teilnehmenden mit Schreibrecht in die Organisation einladen.
