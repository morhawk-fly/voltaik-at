# voltaik-at

Voltaik – PV-Großprojekte (voltaik.at). Eine statische Seite (`index.html`), veröffentlicht über GitHub Pages.

## Fotos tauschen (ohne Programmieren)

Alle Fotos liegen im Ordner **`bilder/`** und haben **feste Namen**. Die Seite zeigt ein Foto automatisch,
sobald eine Datei mit genau diesem Namen dort liegt; fehlt sie, steht an der Stelle „Foto folgt · bilder/…“.

1. Auf GitHub den Ordner `bilder` öffnen → **Add file → Upload files**.
2. Foto hineinziehen. **Der Dateiname muss genau stimmen** (klein geschrieben, Endung `.jpg`).
   Vorher am PC umbenennen. Gleicher Name wie ein vorhandenes Foto = ersetzt es.
3. Unten **Commit changes**. Nach 1–2 Minuten ist es auf der Seite.

| Datei | Wo auf der Seite | Format (Richtwert) |
|---|---|---|
| `titel.jpg` | Kopfbereich rechts (fehlt es: Dach-Skizze) | Querformat, 1600 × 1000 px |
| `montage.jpg` | Breites Foto unter „Warum Voltaik“ | sehr breit, 2100 × 800 px |
| `referenz-1.jpg`, `referenz-2.jpg`, … | Referenzkarten | Querformat 4:3, 1200 × 900 px |
| `franz.jpg`, `willi.jpg` | Ansprechpartner (rund) | quadratisch, 400 × 400 px |

Tipps: JPG, unter 500 KB je Foto. Nur Fotos verwenden, für die wir die Rechte haben, bei Kundenprojekten mit
Zustimmung des Kunden.

## Referenztexte ändern

Datei **`referenzen.js`** öffnen → Stift-Symbol → Titel/Details ändern → **Commit changes**.
Anleitung steht oben in der Datei. Für ein neues Projekt einen Block kopieren und `referenz-4.jpg` hochladen.

## Veröffentlichen (einmalig, wenn fertig)

Noch **nicht** eingeschaltet. Ablauf: Repo-Settings → Pages → Branch `main` / root → Save; Datei `CNAME` mit
`voltaik.at` anlegen; DNS bei IONOS umstellen. Die Domain ist bei GitHub bereits verifiziert.
