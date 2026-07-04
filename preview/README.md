# DARMbalance

Website für Christine Lohmüller — Diplomierte Prävention & Gesundheitstrainerin.
Ganzheitliche Impulse für eine bewusste Darmbalance.

## Local starten

Die Seite ist statisches HTML/CSS/JS — du brauchst nur einen lokalen Webserver.

### Python (auf macOS vorinstalliert)

```bash
cd darmbalance
python3 -m http.server 8000
```

Dann im Browser öffnen: **http://localhost:8000**

Mit `Ctrl+C` beenden.

### Alternative: npx

```bash
cd darmbalance
npx serve .
```

## Projektstruktur

```
darmbalance/
├── index.html          # Hauptseite
├── disclaimer.html     # Rechtlicher Hinweis / Coaching-Disclaimer
├── style.css           # Stylesheet
├── data/
│   └── site.json       # Inhalte (per CMS editierbar)
├── admin/
│   ├── index.html      # Decap CMS Login
│   └── config.yml      # CMS-Konfiguration
├── Bild1.jpeg          # Hero-Bild
├── Bild2.jpeg          # Labor-Banner-Bild
└── Uebermich.jpeg      # Portrait Christine
```

## CMS

Die Inhalte der Seite werden aus `data/site.json` geladen und können über das Decap CMS unter `/admin/` bearbeitet werden.

**Live-URL:** https://garytimeless.github.io/darmbalance/admin/

Voraussetzung: GitHub-Collaborator im Repo `GaryTimeless/darmbalance` sein.

## Deployment

Gehostet auf GitHub Pages (Branch `gh-pages`). Nach CMS-Publish dauert es ~30 Sekunden, bis Änderungen live sind.
