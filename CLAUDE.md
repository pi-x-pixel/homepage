# Project: Pi*Pixel Homepage

## Description

Statische Single-Screen-Brand-/Marketing-Site für `pi-x-pixel.com` — reines HTML ohne Build-Step und ohne JS-Framework (index, impressum, datenschutz, 404, robots.txt, netlify.toml). Deploy-Ziel ist Netlify mit Custom Domain via Porkbun-DNS. Die Site ist deploy-fertig, sobald Impressum und Datenschutz finalisiert sind.

## Tech Stack

* Statisches HTML/CSS (kein Build-Step, kein JS-Framework)
* Netlify (Hosting; Security-Headers + www-Redirect via `netlify.toml`, SSL via Let's Encrypt)
* Porkbun (Domain/DNS)
* Google Fonts

## Current Status

* Phase: Pre-Launch (statische Site fertig) — On Track, Priorität: Hoch, Progress 65 %
* Last updated: 2026-06-12
* Details: siehe PROJECT_STATUS.md

## Conventions

* Language: DE (Site-Inhalte + Rechtstexte; README EN)

## Key Decisions

* Aus dem früheren Projekt `website-generator` ausgegliedert (Pi*Pixel-Branding); Schwester-Projekt: `pi-x-pixel-repo` (selbe Brand)
* Offen: Deploy-Methode — Drag&Drop (schneller) vs. Git-Linked (bessere Iteration)

## Current Goals

* [ ] `datenschutz.html`: Placeholder durch echten DSGVO-Text ersetzen (e-recht24-Generator; Netlify-Hosting + Google Fonts angeben)
* [ ] `impressum.html`: Platzhalter ausfüllen (Name, Adresse, USt-ID/Steuernummer)
* [ ] Netlify-Deploy + Porkbun-DNS auf Netlify schwenken, SSL-Provisionierung verifizieren
* [ ] Pre-Launch-Checkliste (Smoke-Test alle Pages, Mobile-View, 404)
