# Jennas Cozy Chapters

Cozy Bücherzimmer-App für Jenna. Vollständiges GitHub-Pages-Projekt, ohne Build, Server oder API-Schlüssel.

## Hochladen & veröffentlichen

1. ZIP herunterladen und **entpacken**.
2. Auf GitHub ein neues **öffentliches Repository** erstellen, z. B. `jennas-cozy-chapters`.
3. **Add file → Upload files** auswählen. Den **Inhalt** des entpackten Ordners hochladen, nicht die ZIP und nicht den äußeren Ordner. `index.html` muss direkt auf der obersten Ebene stehen. Auch den gesamten `icons`-Ordner hochladen.
4. **Commit changes** wählen.
5. **Settings → Pages → Build and deployment → Source → Deploy from a branch**.
6. Branch **main**, Ordner **/ (root)** auswählen und **Save** klicken.
7. Nach der Bereitstellung steht unter **Settings → Pages → Visit site** der öffentliche Link. Es kann einige Minuten dauern.

Beispielformat (noch kein veröffentlichter Link): `https://DEIN-GITHUB-NAME.github.io/jennas-cozy-chapters/`

Die Punktdateien `.nojekyll` und `.gitignore` sind ebenfalls enthalten. Manche Dateimanager blenden sie aus. Ein eigener Actions-Workflow ist für diese Variante nicht erforderlich. Es gibt keine Installation und keinen Build-Schritt.

## Bisherige Daten mitnehmen

In der bisherigen App unter **Einstellungen & Sicherung → Datensicherung herunterladen** exportieren. Auf der neuen GitHub-Pages-Adresse die JSON-Datei über **Einstellungen & Sicherung** wiederherstellen. Deine bisherigen Daten wechseln nicht automatisch zwischen Internetadressen.

Persönliche Sicherungen **nicht in das öffentliche GitHub-Repository hochladen**. Nur in der App wiederherstellen. Das Paket enthält keine persönlichen Bücher, Journale oder Testdaten.

## Enthalten

- Vollständige Bibliothek, ISBN-Suche, unterstützter Kamera-Scan und Buchjournale.
- Fokus-Timer, Leseziele, Challenges, Lesetaler und Einrichtung.
- Vier Zimmerwelten: Meer, Wald, Kleinstadt-Café, Wohnzimmer am Park.
- 26 Möbel und Dekostücke inklusive Mond-, Whimsy- und Jahreszeitendeko.
- Lichtstimmungen, abschaltbare Animationen, synthetische Geräusche und Spotify-Playlist.
- Cozy Icon mit Buch, Mond und Pflanzen: Originalbild und Größen 32, 180, 192 und 512 Pixel.
- Web-App-Manifest und Apple-Touch-Icon für die Startbildschirm-Verknüpfung.

## Dateien

`index.html`, `app.js`, `cozy.js`, `style.css`, `manifest.webmanifest`, `icons/`, `.nojekyll`, `.gitignore` und diese Anleitung.

## Name und Begrüßung

Der vorläufige App-Name ist **Jennas Cozy Chapters**. Die Standardbegrüßung lautet „Jenna“. Jede Person kann ihren Namen in den Einstellungen ändern. Eine importierte Sicherung behält den dort gespeicherten Namen.

Weitere Namensideen:
- Jennas Lesestübchen – persönlich und gemütlich
- Cozy with Jenna – kurz und einladend
- Jenna’s Book Nook – wie eine kleine Leseecke
- Jennas Cozy Tales – märchenhaft und weich

Den App-Namen bei Bedarf in `index.html` und `manifest.webmanifest` ändern. Der interne Speicherschlüssel `leseliebe-v1` bleibt absichtlich unverändert, damit bestehende Sicherungen kompatibel sind.

## Speicher und Grenzen

Alle Bücher, Journale und Fortschritte liegen lokal im Browser, ohne Konto oder geräteübergreifende Synchronisation. Regelmäßig sichern. Browserdaten löschen entfernt auch App-Daten. Verschiedene Projekte auf derselben GitHub-Pages-Domain teilen den lokalen Speicher; für getrennte Installationen müsste der Speicherschlüssel angepasst werden.

Der Timer reagiert auf vom Browser gemeldete Sichtbarkeitswechsel. Er kann keine anderen Apps sperren. Kamera-Scan und Bildschirm-Wachhalten hängen vom Browser ab. Falls der Scan fehlt, ISBN eintippen. GitHub Pages stellt HTTPS bereit.

Open Library liefert Buchdaten und Cover; Google Fonts liefert Schriften; Spotify liefert die eingebettete Playlist. Diese Verbindungen brauchen Internet. Spotify-Wiedergabe hängt von Konto und Browser ab. Empfehlungen sind thematische Vorschläge anhand von Bewertungen, keine KI-Inhaltsanalyse. Geräusche werden lokal synthetisch erzeugt.

Das Manifest unterstützt die Darstellung als Startbildschirm-Verknüpfung. Kein vollständiger Offline-Modus und kein Service Worker enthalten.

## Lokal testen

Im Ordner `python3 -m http.server 8080` starten und `http://localhost:8080` öffnen. Für die normale Nutzung GitHub Pages verwenden. Direkte `file://`-Aufrufe sind für Kamera und Speicher nicht zuverlässig.

## Aktualisieren

Dateien im selben Repository ersetzen und committen. GitHub Pages veröffentlicht erneut. Vorher Datensicherung erstellen, den Speicherschlüssel beibehalten und danach die Seite neu laden.

## Icon

Das handgemalte Buch-Mond-Motiv wurde für dieses Projekt mit der integrierten Bildgenerierung erstellt. Briefing: offenes elfenbeinfarbenes Buch, goldener Sichelmond, Pflanzen und kleine Lichtpunkte auf moosgrünem Hintergrund; warmer Gouache-Stil ohne Schrift. Die PNG-Varianten sind Größenexporte desselben Motivs.

## Offizielle GitHub-Anleitung

https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
