---
project_name: "Pi*Pixel Homepage"
report_date: "2026-05-22"
previous_report_date: "2026-05-18"
overall_status: "On Track"
priority: "Hoch"
phase: "Pre-Launch (statische Site fertig)"
progress: 65
next_tasks:
  - "Datenschutz-Placeholder durch echten DSGVO-Text ersetzen (e-recht24-Generator)"
  - "Impressum-Platzhalter (Name, Adresse, USt-ID) ausfuellen"
  - "Domain DNS auf Netlify schwenken und live schalten"
  - "Pre-Launch-Checkliste durchgehen"
---

# Projekt-Status-Report

## Zusammenfassung
Pi*Pixel Homepage ist die statische Marketing-/Brand-Site fuer `pi-x-pixel.com` — Single-Screen, kein Build-Step, kein JS-Framework. Site ist deploy-fertig, sobald Impressum + Datenschutz finalisiert sind. Keine inhaltliche Aktivitaet im Berichtszeitraum (nur eine untracked `.gitignore`).

## Seit letztem Report erledigt
_Keine_

## Naechste Schritte
- [ ] datenschutz.html: Placeholder durch generierten DSGVO-Text ersetzen (Netlify-Hosting + Google Fonts angeben) <!-- Status: Offen | Prio: Hoch | Typ: Doku -->
- [ ] impressum.html: Platzhalter ausfuellen (Name, Adresse, USt-ID/Steuernummer) <!-- Status: Offen | Prio: Hoch | Typ: Doku -->
- [ ] Netlify-Deploy via Drag&Drop oder Git-Link <!-- Status: Offen | Prio: Hoch | Typ: Setup -->
- [ ] Porkbun-DNS auf Netlify-A-Records umstellen <!-- Status: Offen | Prio: Hoch | Typ: Setup -->
- [ ] SSL-Provisionierung verifizieren (Let's Encrypt via Netlify) <!-- Status: Offen | Prio: Mittel | Typ: Test -->
- [ ] Pre-Launch-Checkliste (Smoke-Test alle Pages, Mobile-View, 404) <!-- Status: Offen | Prio: Mittel | Typ: Test -->

## Blocker & Risiken
- Datenschutz nur Placeholder — DSGVO-Compliance ohne Update nicht gegeben
- Impressum-Platzhalter blockiert ebenfalls Launch (§ 5 TMG)

## Offene Entscheidungen
- Deploy-Methode: Drag&Drop (schneller) vs. Git-Linked (bessere Iteration)?

## Notizen
Aus dem frueheren Projekt `website-generator` ausgegliedert (Pi*Pixel Branding). Synergie mit `pi-x-pixel-repo` (n8n-WhatsApp-Postgres-Memory-Connector — selbe Brand). Site enthaelt nur statische HTML-Files, kein Build noetig. Letzter Commit unveraendert: 6decd5b. Eine untracked `.gitignore` ist hinzugekommen, sonst keine Aenderung.
