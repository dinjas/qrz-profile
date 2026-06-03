# K7BPM QRZ Profile — Project Context

## What this is
A hand-crafted HTML/CSS snippet for Jason's (K7BPM) QRZ.com profile page. The file `profile.html` is pasted directly into QRZ's profile editor — it is not a standalone page.

## ⚠️ Content editing policy
**Do not reword, rewrite, restructure, or editorialize any of the written content without explicit permission and review from Jason.** This includes the bio/story section, volunteer descriptions, and any other prose. He is particular about his voice and phrasing. CSS and structural/layout changes are generally fine; touching the words is not.

## File structure
- `profile.html` — the profile snippet (paste into QRZ editor)
- `old-profile.html` — previous version, kept for reference
- `preview.html` — browser preview wrapper (loads profile.html via fetch)
- `.context/` — project notes for AI assistants

## Local preview
```bash
python3 -m http.server 8000
```
Open http://localhost:8000/preview.html in a browser.

## Design notes
- Max width is controlled by QRZ's container; `.profile` has no `max-width` set
- Responsive breakpoint at 520px collapses the two-column layout to one column
- Color palette is intentionally muted/neutral — light backgrounds, dark-ish text
- All grays should be readable: avoid anything lighter than ~#555 for body text, ~#444 for labels
- `.past-item` uses `opacity: 0.85` to visually de-emphasize past roles without making them unreadable
- Section labels (`.section-label`) are monospace, uppercase, bold, `#444`
- QRZ links follow the pattern: `https://www.qrz.com/db/CALLSIGN`

## QSL info
- Uploads to LoTW and QRZ within a day of QSO
- Paper QSLs accepted via the 7th Area Incoming QSL Bureau
