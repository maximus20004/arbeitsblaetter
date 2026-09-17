# Arbeitsblätter veröffentlichen – Kurzanleitung

Dieser Ordner ist so aufgebaut, dass er direkt als GitHub-Pages-Seite läuft.

```
index.html               Übersichtsseite (die Adresse, die du in Teams postest)
jgst10-wiederholung.html Arbeitsblatt Jgst. 10
```

## 1. Einmalig: Repository anlegen und Pages einschalten

1. Auf GitHub ein neues Repository anlegen, z. B. `arbeitsblaetter`. **Sichtbarkeit: Public**
   (GitHub Pages ist für private Repositories kostenpflichtig).
2. Den Inhalt dieses Ordners hochladen – entweder per Drag-and-drop auf
   *Add file → Upload files*, oder per Git:

   ```
   git init
   git add .
   git commit -m "Arbeitsblätter"
   git branch -M main
   git remote add origin https://github.com/<DEIN-NAME>/arbeitsblaetter.git
   git push -u origin main
   ```

3. Im Repository auf **Settings → Pages** gehen.
   Bei *Source* **Deploy from a branch** wählen, Branch `main`, Ordner `/ (root)`, speichern.
4. Nach ein bis zwei Minuten ist die Seite erreichbar unter:

   ```
   https://<DEIN-NAME>.github.io/arbeitsblaetter/
   ```

Diese eine Adresse ist ab jetzt dein Verteil-Link. Sie ändert sich nie, auch wenn
du später Blätter ergänzt.

## 2. Ein neues Arbeitsblatt ergänzen

1. Im Baukasten das Blatt mit **⭳ Arbeitsblatt (HTML)** exportieren.
   Häkchen **„Schlanke Fassung exportieren"** setzen – 151 statt 700 KB.
2. Datei in diesen Ordner legen, Name klein und ohne Umlaute
   (z. B. `jgst7-bruchrechnen.html`).
3. In `index.html` den vorhandenen `<a class="blatt">`-Block kopieren und
   Adresse, Titel und Untertitel anpassen. Die Kommentarzeile im Quelltext
   zeigt die Stelle.
4. Hochladen bzw. `git add . && git commit -m "..." && git push`.

## 3. Wichtig: Lösungsblätter gehören NICHT hierher

Das Repository ist öffentlich – alles darin kann jeder lesen, der die Adresse
errät. Lösungsblätter also **nicht** hochladen. Die brauchst du ohnehin nur
selbst: im Baukasten auf *Lösungsblatt* umschalten und über **⭳ PDF** ausgeben.

## 4. Verteilen über Teams

Ab jetzt **nur noch den Link posten, nie die Datei anhängen.**

Der bisherige Weg scheiterte daran, dass Teams-Anhänge in SharePoint liegen und
SharePoint HTML-Dateien grundsätzlich nicht anzeigt, sondern nur zum Download
durchreicht. Auf dem iPad landet die Datei dann im Text-Betrachter – das war das
„nur Code". Ein Link umgeht das komplett.

**So geht es:**

- **In einem Kanal oder Chat:** Adresse einfach in die Nachricht schreiben.
  Teams macht daraus eine anklickbare Vorschaukarte.
- **In einer Aufgabe (Assignment):** *Ressourcen hinzufügen → Link* und die
  Adresse einfügen. Schüler öffnen sie direkt aus der Aufgabe.
- **Als feste Registerkarte:** Im Kanal oben auf **+**, Kachel **Website**
  wählen, Namen und Adresse eintragen. Dann liegt die Übersicht dauerhaft als
  Reiter im Kanal – ein Tipp, kein Suchen in alten Nachrichten.

**Ein Hinweis für die Klasse:** Tippt man den Link in Teams an, öffnet sich der
eingebaute Browser von Teams. Das Arbeitsblatt funktioniert dort vollständig.
Nur wenn jemand sein ausgefülltes Blatt **als PDF sichern** will, sollte er
vorher über das **⋯**-Menü auf **„In Safari öffnen"** gehen – eingebaute Browser
tun sich mit Downloads schwer.

## 5. Wenn kein GitHub sein soll

Jeder Ort, der HTML-Dateien als Webseite ausliefert, funktioniert genauso:
mebis/Moodle (Datei-Material mit Anzeige „Einbetten" bzw. „Öffnen"), die
Schulhomepage oder ein anderer Webspace. Entscheidend ist nur, dass am Ende
eine **Adresse** herauskommt und keine Datei zum Herunterladen.
