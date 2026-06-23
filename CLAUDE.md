# CLAUDE.md — Website / Portfolio
**Stand:** April 2026 | **Owner:** Ing. Richard Schöll (TecSavvy-Solutions)
**Zielrolle:** Digital Transformation & Innovation Lead (Focus: Tech Ops / MRO)

---

## Wer ist Richard? (Kurzkontext)

- **The Domain-Architect:** 20 Jahre B1.1/B2 Aviation-Expertise trifft auf skalierbare Software-Architektur
- **Value Proposition:** Moving MRO from physical troubleshooting at the engine to systemic troubleshooting via code
- **Mindset:** Ultra-Trail Running (100km+) — Relentless execution, no excuses. *"Start where others stop."*
- **Rollenverteilung:** Richard ist der Architekt — Claude ist der Programmierer

---

## Was ist das?

Richards persönliche Portfolio-Website. Dient als **digitale Visitenkarte und Proof of Transformation** — übersetzt tiefes technisches Architektur-Wissen in klaren MRO-Business-Value (Delay Resistance, Operational Efficiency) für Management und Recruiter.

Gehostet auf GitHub Pages unter `https://tecsavvy-solutions.github.io/`.
Kein Build-Step, kein Framework — reines HTML/CSS/JS mit Tailwind CDN und Chart.js CDN.

**Aktuelle Version:** `index.html` = V18 (Clean Architecture Edition)

---

## Strategischer Zweck

Die Website ist das Herzstück von Richards Portfolio-Strategie und dient als Beweis für die Transformation vom operativen Techniker zum Digital Transformation Lead. Zielgruppe: **MRO-Management, Aviation-HR und Tech-Recruiter**.

Jede Änderung an der Website muss gegen dieses Ziel bewertet werden:
> Stärkt es Richards Position als authoritative Digital Transformation Lead in Aviation/MRO?

---

## Kommunikationsstil / Tone of Voice

**Aktiv, direkt, keine Floskeln.**

| Verboten | Richtig |
|---|---|
| "Ich würde gerne..." | "Ich baue..." |
| "Ich versuche..." | "Ich transformiere..." |
| "Man könnte..." | "Ich execute..." |
| Corporate Buzzword-Salat | Klare, operative Sprache |

Stil: **relentless, candid, hochprofessionell, action-oriented.** Starke Verben. Keine Weichmacher.

---

## Datei-Struktur

```
Website\
├── html Codes\
│   ├── index.html          ← AKTIVE PRODUKTIONS-DATEI (aktuell V18)
│   ├── website_V1–V18.*    ← Versionsverlauf (txt = Notes, html = Code)
├── favicon.png
├── logo.png
├── dashboard.PNG           ← Screenshot für Tab-2 (Hybrid_Store)
├── print.PNG               ← Screenshot für Tab-3 (Precision_Print)
├── multi_device_test.JPG   ← Screenshot für Tab-4 (Responsive_Exec)
├── MRO_Ground_Plan_Visualizer_Presentation_EN_WS.pdf
├── Ground_Plan_DEMO_Video.mp4
└── CLAUDE.md               ← diese Datei
```

**Alle Assets (Bilder, PDF, Video) liegen im gleichen Ordner wie index.html** — relative Pfade ohne Subfolder.

---

## Design-System

| Element | Wert |
|---|---|
| Primärfarbe | Sky-Blue `#38bdf8` / `#0ea5e9` |
| Hintergrund | Slate-50 `#f8fafc` mit Grid-Pattern |
| Dark Sections | Slate-900 `#0f172a` |
| Fonts | Inter (Body), JetBrains Mono (Code/Badges) |
| Stil | Clean, Tech-ästhetik, Aviation-MRO-Sprache |

Tailwind-Klassen für Blau: `text-sky-400/500/600`, `bg-sky-500/600`, `border-sky-500`

---

## GPV — Technische Details (für korrektes Copywriting)

Das Flagship-Projekt, das auf der Website präsentiert wird:

| Parameter | Wert |
|---|---|
| Größe | ~1.750 LOC Full-Stack WebApp |
| Frontend | React 19.2 + Vite (SPA) |
| Backend | Flask (Python) + SQLite (Auto-Cleanup nach 48h) |
| API | REST via Axios Polling (60s Intervall) |
| Deployment | 5-Service Docker Compose Stack |
| Zugriff | Tailscale SSO — überall erreichbar |
| Versionierung | GitHub (TecSavvy-Solutions) |
| Print | `@media print` — A4 Landscape Handover Protokolle 1:1 skaliert |
| Kernlogik | Fuzzy_ID — bindet Daten an Flugereignis, Delays wandern automatisch mit |

---

## Sektionen

| ID | Nummer | Inhalt |
|---|---|---|
| `#intro` | 01 | Identity/Header — Name, Tagline, Registry-Panel |
| `#philosophy` | 02 | Philosophie — 4 Karten |
| `#poc` | 03 | Ground Plan Visualizer — Video/PDF Toggle, Strategy Tabs, Radar Chart |
| `#leadership` | 04 | Leadership Log — Deputy TL, AOG Recovery |
| `#logs` | 05 | Experience Timeline — Karriere-Verlauf |
| Footer | — | CTA LinkedIn, Copyright |

---

## JavaScript-Logik (index.html)

| Funktion | Beschreibung |
|---|---|
| `simulateDelay()` | Animation in Tab-1 — Bar springt nach rechts, rot |
| `playVideo()` | Custom Play-Button — zeigt native Controls nach erstem Klick |
| `switchMedia(type)` | Pill-Toggle zwischen Video und PDF |
| `switchTab(tabId, btn)` | Strategy Tab Wechsel — aktiver Tab dark, Dot animiert |
| Cursor-IIFE | Custom Blue Glow Cursor — nur auf Desktop (`pointer: fine`) |
| `new Chart(...)` | Radar Chart mit Chart.js |

---

## Custom Cursor (hinzugefügt V18+)

- **Typ:** Kleiner blauer Glow-Punkt (10px, `#38bdf8`)
- **Nur Desktop:** Media Query `(pointer: fine)` — Touch-Geräte behalten Standard-Cursor
- **Hover-Effekt:** Auf Links/Buttons wird der Punkt größer (scale 1.8) und heller
- **Performance:** `requestAnimationFrame` + `will-change: left, top`
- **CSS-Klassen:** `#cursor-dot`, `.cursor-hover`, `.cursor-hidden`

---

## Deployment

Website liegt auf GitHub Pages — Repository: `TecSavvy-Solutions/tecsavvy-solutions.github.io`

**Deploy-Workflow:**
1. `index.html` + alle Assets in den Repo-Root pushen
2. GitHub Pages baut automatisch aus `main` Branch
3. Keine npm, kein Build — direktes HTML

**Lokaler Test:** Datei direkt im Browser öffnen oder mit Live Server in VS Code.

---

## Erweitertes Profil (relevant für zukünftige Website-Sektionen)

Falls die Website um weitere Kompetenzen ergänzt wird:

- **AI Integration:** Chief AI Academy Background — Graph RAG und Model Context Protocol (MCP) für autonome, vernetzte Knowledge-Systeme
- **Systemic Logic:** Creator der "TRIADE" Trading Strategy (Pine Script) — beweist Fähigkeit zur Architektur antifragiler Systeme außerhalb Aviation
- **Stack-Präferenz:** Python / React / Docker-basierte Lösungen

---

## AI-Anweisungen für Website-Arbeit

1. **Kontext-Alignment:** Jede Feature-Anfrage, Code-Änderung oder Text-Anpassung gegen das Ziel der Portfolio-Optimierung und Richards Positionierung als Digital Transformation Lead evaluieren
2. **Tone:** Starke, aktive Verben. Kein Corporate Fluff. Objektiv, scharf, autoritativ
3. **Tech-Alignment:** Python/React/Docker-Lösungen bevorzugen. Operative Resilienz priorisieren
4. **Zielgruppe im Kopf behalten:** Texte müssen für MRO-Management und Recruiter verständlich sein — nicht nur für Entwickler

---

## Kritische Regeln

- **Kein Build-Step** — alle CDN-Links (Tailwind, Chart.js, FontAwesome) bleiben extern
- **Asset-Pfade relativ** — niemals absolute Pfade oder `http://`
- **Versionen** — neue Version als `website_VXX.html` sichern, dann `index.html` überschreiben
- **Mobile first** — alle Änderungen auf Handys testen (Samsung S24, iPads)
- `cursor: none` gilt nur für `@media (pointer: fine)` — Touch-Geräte NICHT anfassen
