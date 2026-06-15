# VascuMagic2
# VascuMAGIC+ — Aortic Graft Infection Decision Support

Clinical decision support extension for VascuMAGIC. Covers management, antibiotic duration, PET/CT guidance, and follow-up scheduling for aortic vascular graft and endograft infection (VGEI).

## Evidence base

| Paper | Key contribution |
|---|---|
| Lyons et al., EJVES 2026 | MAGIC follow-up: 59% suspected → infected within 2y; CRP sensitivity; 2-year minimum follow-up |
| Husmann et al., EJNMMI 2018 | PET/CT stop/continue/escalate thresholds (VASGRA cohort, n=68, 266 scans) |
| Kouijzer et al., CMI 2025 | Delphi consensus: empiric therapy, antibiotic duration (6/12wk/6mo rules), follow-up schedule |

## Modules

- **M0** — VascuMAGIC result entry + CRP/WBC interpretation
- **M1** — Emergency triage (6 binary questions → stable vs emergency pathway)
- **M2** — Stable pathway (surgical fitness, organism, graft removal extent)
- **M3** — Antibiotic duration engine (6w / 12w / 6mo / lifelong SAT rules)
- **M4** — PET/CT stop/continue/escalate engine with timing gate
- **M5** — Follow-up schedule generator (suspected vs infected, dated timeline)

## Important disclaimer

This tool is for clinical decision support only. It does not replace multidisciplinary team (MDT) judgement. All major treatment decisions require MDT sign-off. This tool has not been independently validated for autonomous clinical decision-making.

## Offline use

Because this is a single self-contained HTML file with no external dependencies, it can also be:
- Saved locally and opened directly in any browser (File → Open)
- Distributed as an email attachment
- Hosted on any web server or intranet

## Structure

```
vascumagic/
└── index.html    # Complete app — all HTML, CSS, and JavaScript in one file
└── README.md     # This file
```
