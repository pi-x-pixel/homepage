---
project_name: "Pi*Pixel Homepage"
report_date: "2026-08-10"
previous_report_date: "2026-07-02"
overall_status: "Paused"
priority: "Hoch"
phase: "Pre-Launch (statische Site fertig)"
progress: 65
next_tasks:
  - "datenschutz.html: Placeholder durch generierten DSGVO-Text ersetzen (Netlify-Hosting + Google Fonts angeben)"
  - "impressum.html: Platzhalter ausfuellen (Name, Adresse, USt-ID/Steuernummer)"
  - "Netlify-Deploy via Drag&Drop oder Git-Link"
  - "Porkbun-DNS auf Netlify-A-Records umstellen"
  - "Pre-Launch-Checkliste (Smoke-Test alle Pages, Mobile-View, 404)"
---

# Projekt-Status-Report

## Zusammenfassung

Pi*Pixel Homepage ist die statische Marketing- und Brand-Site fuer `pi-x-pixel.com` — Single-Screen, kein Build-Step, kein JS-Framework. Die Site ist technisch deploy-fertig und wartet ausschliesslich darauf, dass die beiden Rechtstext-Platzhalter gefuellt werden. Im Berichtszeitraum fand keine Commit-Aktivitaet statt.

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

- Datenschutzseite enthaelt weiterhin nur Platzhaltertext — ohne echten DSGVO-Text ist ein Livegang nicht zulaessig.
- Impressum-Platzhalter blockiert den Launch zusaetzlich (Paragraf 5 TMG).
- Der Launch haengt seit rund drei Monaten an zwei Textseiten, die in wenigen Stunden erledigt waeren. Bei Prioritaet "Hoch" ist diese Diskrepanz zwischen Aufwand und Stillstand selbst das eigentliche Risiko.

## Offene Entscheidungen

- Deploy-Methode: Drag&Drop (schneller) vs. Git-Linked (bessere Iteration)?

## Notizen

Status von On Track auf Paused geaendert. Begruendung: Seit dem Initial-Commit hat sich inhaltlich nichts bewegt, im Berichtsfenster 2026-07-02 bis 2026-08-10 gibt es keinen einzigen inhaltlichen Commit. Der einzige Commit (c8747f2, 2026-07-18) ist ein automatischer Backup-Lauf, der nur diese PROJECT_STATUS.md versioniert hat. Ein Projekt, das seit drei Monaten unveraendert vor derselben Huerde steht, ist nicht "On Track".

Working Tree ist sauber, es liegt keine unkommittierte Arbeit herum. Progress bleibt unveraendert bei 65 Prozent. Nicht mit `pi-x-pixel-repo` verwechseln — das ist ein getrenntes Projekt derselben Firma.
