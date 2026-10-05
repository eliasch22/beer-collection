# Beers – persönliches Bier-Tagebuch (PWA)

Installierbare Web-App: läuft offline, Daten bleiben auf dem Gerät.

## Installation über GitHub Pages

1. Auf https://github.com ein Konto erstellen (kostenlos).
2. Oben rechts **+** → **New repository**
   - Name: `beers`
   - Sichtbarkeit: **Public** (GitHub Pages ist im Gratis-Konto nur für öffentliche Repositories verfügbar. Öffentlich ist nur der Programmcode, deine Biere und Fotos bleiben auf deinem Handy.)
   - **Create repository**
3. Im neuen Repository: **uploading an existing file** (bzw. **Add file → Upload files**).
   Den **Inhalt** dieses Ordners (nicht den Ordner selbst) ins Fenster ziehen, inkl. `vendor`, `icons` und `.nojekyll`.
   → **Commit changes**
4. **Settings → Pages**: Source **Deploy from a branch**, Branch **main**, Ordner **/ (root)** → **Save**.
5. Nach 1–2 Minuten ist die App erreichbar unter
   `https://<dein-benutzername>.github.io/beers/`
6. Auf dem Handy in **Chrome** öffnen → Menü ⋮ → **App installieren** (oder «Zum Startbildschirm hinzufügen»).

## Daten aus der Claude-Version übernehmen

1. In der Claude-Version: Einstellungen → **Backup mit Fotos (ZIP)** → Datei speichern.
2. In der installierten App: Einstellungen → **Importieren (ZIP oder JSON)** → ZIP-Datei wählen.

## Updates

Geänderte Dateien im Repository ersetzen (Add file → Upload files). Die App lädt die neue Version beim nächsten Öffnen mit Internetverbindung.
Bei Änderungen an `sw.js` die Versionsnummer `VERSION` erhöhen.

## Backup

Die Daten liegen im Speicher von Chrome auf dem Gerät. Wer die Browserdaten löscht oder die App deinstalliert, löscht auch die Sammlung.
Darum regelmässig: Einstellungen → **Backup teilen** → z. B. in Google Drive ablegen. Die App erinnert nach 30 Tagen.

## Enthaltene Bibliotheken

- Tesseract.js 5.1.1 (Apache-2.0) und Sprachdaten tessdata_fast eng/deu (Apache-2.0) – lokale Texterkennung
- ZXing 0.21.3 (Apache-2.0) – Barcode-Erkennung
- JSZip 3.10.1 (MIT) – Backup als ZIP
- Weltkarte: Natural Earth via world-atlas (Public Domain)
