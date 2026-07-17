# KyPost Site

The landing page for the KyPost email ecosystem — a self-hosted mail server
paired with native, relay-only clients for Android, iOS, macOS, and Linux.

This repo is just the marketing site. The actual products live in their own
repos:

- [KyPost Server](https://github.com/Yoshiofthewire/KyPost-Server) — self-hosted IMAP/SMTP web client with local-AI keyword labeling
- [KyPost for Android](https://github.com/Yoshiofthewire/KyPost-for-Android)
- [KyPost for Mac & iOS](https://github.com/Yoshiofthewire/KyPost-for-Mac)
- [KyPost for Linux](https://github.com/Yoshiofthewire/KyPost-for-Linux)

## What's here

A single-page static site, no build step, no framework:

```
index.html       All page sections
css/styles.css   Layout, typography, @font-face, theme-wipe demo styling
js/main.js       Mobile nav toggle, scroll-spy nav highlighting, theme-wipe scroll mechanic
assets/          Logos, mascot art, self-hosted fonts (Space Grotesk, IBM Plex Mono),
                 and real KyPost web app screenshots used in the theme demo
```

The page covers the ecosystem overview, cross-platform reach, the PGP +
secure-pickup privacy model, the shared 15-theme customization system (with
a scroll-driven preview built from real app screenshots), and the current
status of each project.

## Running locally

Any static file server works, e.g.:

```sh
python3 -m http.server 8000
```

Then open `http://localhost:8000/`.

## Deploying

Zero-build static site — deploy the repo as-is to Cloudflare Pages, GitHub
Pages, Netlify, or any static host.

## License

AGPL-3.0 (this site). The KyPost client apps are licensed separately under
GPL-2.0 — see their individual repos.
