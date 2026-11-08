# S3VL05-Frontend
Repo zu S3 VL05: Frontend in verteilten Systemen

# Vorbereitung

- GitHub Codepace für `DHBW-VS-Vert-Sys/S3VL05-Frontend` erstellen.

- nginx Docker image runterladen:
```shell
docker pull nginx:latest
```

# Aufgabe 1: HTML Hosten

## HTML erzeugen

Erzeuge im Ordner `nginx-content` eine HTML Datei namens `index.html` und fülle sie mit Inhalt.

## nginx starten

Im Terminal des Codespaces im Repository-Verzeichnis ausführen:

```shell
docker compose up -d
```

Im Reiter **Ports** den weitergeleiteten Port **8080** öffnen. 

Zum Stoppen:

```shell
docker compose down
```

# Aufgabe 2: Stylesheets

## CSS

### Inline

Ändert eure vorhandenen HTML Elemente durch inline CSS Attribute. Nach einem Refresh der gehosteten Seite könnt ihr die Änderungen live beobachten.

### Externes Stylesheet

Verschiebt nun eure CSS Änderungen in ein dediziertes Stylesheet und bindet es in die HTML Seite ein. Erzeugt hierfür eine neue Datei im Ordner `nginx-content` namens `style.css`. Im HTML verlinkt ihr das Stylesheet mit der Zeile ` <link rel="stylesheet" href="style.css">`. Achtet darauf, dass das externe Stylesheet genaue Selektoren braucht, um die Styles auf die einzelnen Elemente anwenden zu können.

# Aufgabe 3: Javascript

Erzeugt eine Datei namens `script.js` im `nginx-content` Directory. Befüllt die Datei mit dem Inhalt aus dem Foliensatz. Auch die HTML muss angepasst, bzw. erweitert werden. Bindet die Skriptdatei ins HTML ein: `<script src="script.js"></script>`
Ladet die gehostete Seite neu und schaut, welchen Effekt wir per Javascript erzielen können.