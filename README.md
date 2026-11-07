# Jedes Leben ein Licht · Every Life a Light

Alle 8,3 Milliarden Menschen und alle Tiere der Erde als Lichter auf einem 3D-Globus, zum Hineinzoomen bis zum einzelnen Menschen.
Every person and animal on Earth as lights on a 3D globe.

Die Seite ist komplett statisch: `index.html`, Schriften, three.js und 156 Bildkacheln mit Bevölkerungsdaten. Sie braucht keinen Server-Code, keine Datenbank und lädt nichts von fremden Servern.

## Auf GitHub Pages veröffentlichen (kostenlos)

1. Auf github.com oben rechts **+ → New repository**. Name zum Beispiel `every-life-a-light`, **Public** auswählen, **Create repository**.
2. Dateien hochladen. Am einfachsten mit **GitHub Desktop** (desktop.github.com): Repository klonen, den ganzen Inhalt dieses Ordners hineinkopieren, „Commit to main“, dann „Push origin“.
   Im Browser geht es auch („uploading an existing file“). Dort sind aber höchstens 100 Dateien pro Upload möglich: zuerst alles außer dem Ordner `detail` hochladen, dann die Kacheln aus `detail` in zwei Portionen (die Datei-Namen müssen im Ordner `detail/` landen).
   Die versteckte Datei `.nojekyll` sorgt dafür, dass GitHub die Dateien unverändert ausliefert.
3. Im Repository **Settings → Pages**: bei „Build and deployment“ **Deploy from a branch**, Branch **main**, Ordner **/ (root)**, **Save**.
4. Nach ein bis zwei Minuten ist die Seite unter `https://martin01248.github.io/every-life-a-light/` erreichbar.

Damit die Vorschau beim Teilen (WhatsApp, LinkedIn …) überall erscheint: in `index.html` die Zeile mit `og:image` auf die volle Adresse ändern, also `content="https://martin01248.github.io/every-life-a-light/og.png"`.

GitHub Pages ist für öffentliche Repositories kostenlos (bis 1 GB Größe und etwa 100 GB Datenverkehr pro Monat; diese Seite ist rund 50 MB groß).

## Hinweis

Mit Hilfe von KI (Claude von Anthropic) erstellt. Eine Annäherung, ohne Gewähr für Richtigkeit und Vollständigkeit. Alle Quellen und Lizenzen stehen auf der Seite unter „Quellen & Lizenzen“.

## Lizenzen der verwendeten Daten und Software (Kurzfassung)

- Bevölkerung: GHSL GHS-POP (© Europäische Union, JRC, CC BY 4.0); Google Data Arts WebGL Globe (Apache 2.0, nach SEDAC/CIESIN GPW); Our World in Data (CC BY 4.0); Gapminder (CC BY 4.0); UN World Population Prospects (CC BY 3.0 IGO)
- Karten: Natural Earth (gemeinfrei), world-atlas (ISC), IANA-Zeitzonen (gemeinfrei)
- Tiere und Pflanzen: FAOSTAT (CC BY 4.0), CHIRPS (gemeinfrei), NASA MODIS über NOAA ERDDAP, van den Hoogen et al. 2019, weitere Studien wie auf der Seite angegeben; Statistik Austria
- Himmel: Yale Bright Star Catalogue über d3-celestial (BSD-3-Clause); NASA JPL Bahnelemente
- Software: three.js (MIT); Schriften Instrument Serif, Hanken Grotesk, JetBrains Mono (SIL Open Font License 1.1)
