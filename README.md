# Sebyōshi – Releases

*Ready-made Mac builds of [Sebyōshi](https://github.com/gnqgpsr495-ui/sebyoshi) — your PDFs as a bookshelf.*
*Fertige Mac-Builds von [Sebyōshi](https://github.com/gnqgpsr495-ui/sebyoshi) – deine PDFs als Bücherregal.*

Source code, issues and build instructions live in the main repo: [github.com/gnqgpsr495-ui/sebyoshi](https://github.com/gnqgpsr495-ui/sebyoshi).

**What is here.** Each release carries `Sebyoshi-<version>.zip` (universal, arm64 + x86_64, ad hoc signed) and `Sebyoshi-<version>.zip.sig`, an Ed25519 signature over the bytes of the ZIP.

**Updater.** At launch the app queries `releases/latest` of this repo. “Update” downloads the ZIP and installs it only if the `.sig` matches the key built into the app, the app inside has the same bundle identifier and the announced version, and `codesign --verify` passes; a release without `.sig` is never installed. **Privacy:** this check is the app's only network connection; nothing about you or your books is sent. Switch it off in Settings — “Check for Updates …” still works.

**Install (Mac, macOS 15 or later).** Unzip, drag `Sebyoshi.app` to Applications, open it once. The app is not notarised (no paid developer account), so Gatekeeper blocks it on first launch: **System Settings → Privacy & Security → “Open Anyway”** (at the bottom), then confirm. Right-click → Open no longer works since macOS 15.

**iPad and iPhone** are not distributed here: build the app yourself with your own free Apple ID (see the main README), or use TestFlight if a build is offered there.

**Predecessor.** The app was called *Regal* up to version 0.2, and this repo was `regal-releases`; the Regal 0.2 release is still listed. Regal does not update itself to Sebyōshi — install Sebyōshi once by hand; on first launch it copies your settings and app folder over, nothing is deleted.

License: code MIT; artwork and docs CC BY-SA 4.0; the name and logo “Sebyoshi” are not licensed for forks. See LICENSE and NOTICE in the main repo.

---

## Deutsch

Quellcode, Issues und Bauanleitung liegen im Haupt-Repo: [github.com/gnqgpsr495-ui/sebyoshi](https://github.com/gnqgpsr495-ui/sebyoshi).

**Was hier liegt.** Jedes Release enthält `Sebyoshi-<version>.zip` (universell, arm64 + x86_64, ad hoc signiert) und `Sebyoshi-<version>.zip.sig`, eine Ed25519-Signatur über die Bytes des ZIPs.

**Updater.** Beim Start fragt die App `releases/latest` dieses Repos ab. „Aktualisieren“ lädt das ZIP und installiert es nur, wenn die `.sig` zum eingebauten Schlüssel passt, die App darin dieselbe Bundle-ID und die angekündigte Version trägt und `codesign --verify` besteht; ein Release ohne `.sig` wird nie installiert. **Datenschutz:** diese Abfrage ist die einzige Netzverbindung der App; es werden keine Daten über dich oder deine Bücher gesendet. Abschaltbar in den Einstellungen – „Nach Updates suchen …“ geht weiterhin.

**Installieren (Mac, ab macOS 15).** ZIP entpacken, `Sebyoshi.app` in den Programme-Ordner ziehen, einmal öffnen. Die App ist nicht bei Apple beglaubigt (kein bezahltes Entwicklerkonto), macOS blockiert sie deshalb beim ersten Start: **Systemeinstellungen → Datenschutz & Sicherheit → „Trotzdem öffnen“** (ganz unten), dann bestätigen. „Rechtsklick → Öffnen“ geht seit macOS 15 nicht mehr.

**iPad und iPhone** gibt es hier nicht: die App selbst bauen, mit der eigenen kostenlosen Apple-ID (siehe Haupt-README), oder TestFlight nutzen, falls dort ein Build angeboten wird.

**Vorgängerin.** Bis Version 0.2 hieß die App *Regal* und dieses Repo `regal-releases`; das Release Regal 0.2 ist hier weiterhin gelistet. Regal aktualisiert sich nicht auf Sebyōshi – Sebyōshi einmal von Hand installieren; beim ersten Start übernimmt es Einstellungen und App-Ordner per Kopie, gelöscht wird nichts.

Lizenz: Code MIT; Logo, Bilder und Doku CC BY-SA 4.0; Name und Logo „Sebyoshi“ sind nicht für Abwandlungen freigegeben. Einzelheiten in LICENSE und NOTICE im Haupt-Repo.
