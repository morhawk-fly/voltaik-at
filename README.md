# voltaik-at

Voltaik – PV-Großprojekte (voltaik.at). Eine statische Seite (`index.html`), veröffentlicht über GitHub Pages
(Datei `CNAME` = voltaik.at, `.nojekyll`).

## Dateien

| Datei | Inhalt |
|---|---|
| `index.html` | Seite mit Texten (Montage, Team, Leistungen, Shop, Referenzen, Versprechen, FAQ, Kontakt) |
| `produkte.js` | Produktkarten (Titel, Bild, Link auf voltaik.shop, kein Preis) und Produktzahl des Shops. **Nicht von Hand ändern** – erzeugt im Ops-Repo mit `python3 python-scripts/voltaik_at_produkte.py --ziel <ordner>` |
| `referenzen.js` | Referenzprojekte (siehe unten) |
| `bilder/` | Fotos, je WebP + JPG, ≤ 300 KB (Porträts ≤ 150 KB) |

## Fotos

| Datei | Wo | Herkunft |
|---|---|---|
| `titel.*` | Kopfbereich | KI-Bild, als „Symbolbild“ gekennzeichnet |
| `montage-fassade.*` | Abschnitt Montage | echtes Foto: Max Ennsgraber bei der Montage |
| `max-ennsgrabner.*` | Team, Max | Ausschnitt aus dem echten Montagefoto |
| `franz-holzner.*` | Team, Franz | Ausschnitt aus KI-Bild (Franz einverstanden, Willi 01.10.2026) |
| `grossdach.*`, `planung.*` | Leistungen, Ablauf | KI-Bilder, als „Symbolbild“ gekennzeichnet |
| `referenz-1.jpg`, `referenz-2.jpg`, … | Referenzkarten | fehlt die Datei, zeigt die Karte das `ersatzbild` bzw. „Foto folgt“ |

KI-Bilder werden ersetzt, sobald echte Fotos da sind. Neue Fotos im Ops-Repo verkleinern
(`python-scripts/voltaik_at_bilder.py`), oder auf GitHub unter `bilder/` hochladen (gleicher Name ersetzt das alte Foto,
dann beide Endungen `.webp` und `.jpg`).

## Referenztexte ändern

Datei **`referenzen.js`** öffnen → Stift-Symbol → Titel/Details ändern → **Commit changes**.
Anleitung steht oben in der Datei. Neues Projekt nur mit echten Angaben und Foto (`bilder/referenz-2.jpg`).

## Anfrage

GitHub Pages kann nichts serverseitig senden. „Zum Anfrageformular“ führt auf das Shopify-Kontaktformular
(`voltaik.shop/pages/contact?betreff=Grossprojekt`), daneben Telefon und `office@voltaik.shop`.

## Veröffentlichen

Repo-Settings → Pages → Branch `main` / root. DNS bei IONOS (macht Willi): 4 × A 185.199.108.153 – 185.199.111.153,
AAAA 2606:50c0:8000::153 – 2606:50c0:8003::153, CNAME `www` → `morhawk-fly.github.io`; vorher die Domain voltaik.at
in Shopify entfernen. Die Domain ist bei GitHub bereits verifiziert.
