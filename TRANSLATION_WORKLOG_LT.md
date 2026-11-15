# Lithuanian translation work log

This file is the durable handoff for continuing Lithuanian PhotoCraft localization across conversations. The GitHub translation catalog remains the source of truth for actual UI strings; this file records terminology decisions and unresolved work so they are not lost between chats.

## Working rules
- Apply every explicitly agreed translation to the relevant catalog in the same work session.
- Search the whole catalog for the same source term and related variants before editing.
- Batch related edits into as few commits as practical.
- After writing, fetch the file again and verify the exact rows.
- Never report a change as saved unless the GitHub write succeeded and the row was verified.
- Do not invent source keys. If a discussed term is absent, locate the exact source key in the application or another source catalog first.

## Agreed terminology
| Source | Lithuanian | Notes |
|---|---|---|
| Basic | Pagrindinis | UI section/category |
| Basic Adjustments | Pagrindiniai koregavimai | Use when this exact source key exists |
| Light | Šviesa | Photo adjustment section, not font weight |
| fontWeight / Light | Plonas | Font weight only |
| Noise Reduction | Triukšmo slopinimas | Approved wording |
| Noise Reduction Strength | Triukšmo slopinimo stiprumas | Approved wording |
| Color Noise Reduction | Spalvinio triukšmo slopinimas | Approved wording |
| Tint | Atspalvis | Approved wording |
| Spot Color | Baltos spalvos balanso pipetė | Approved wording |
| Filter by | Atrankos kriterijai | Approved wording |
| Same folder as original photos | Originalios nuotraukos aplankas | Approved wording |
| Red Eye Removal | Raudonų akių koregavimas | Approved wording |
| Auto Tone | Automatinis tono koregavimas | Approved wording |
| Toning | Tonavimas | Approved wording |
| RAW Develop | RAW dorojimas | Approved wording |
| RAW Develop Filter | RAW dorojimo priemonės | Approved wording; do not translate as „filtras“ |
| Pixel Art Preview | Pikselinio meno peržiūra | Approved on 2026-11-15; exact catalog source key still needs locating |
| Print Size | Spaudinio dydis | Applied to catalog |
| Warming Filter (85) | Šiltų tonų filtras (85) | Applied to catalog |
| Warming Filter (LBA) | Šiltų tonų filtras (LBA) | Applied to catalog |
| Warming Filter (81) | Šiltų tonų filtras (81) | Applied to catalog |
| Cooling Filter (80) | Šaltų tonų filtras (80) | Applied to catalog |
| Cooling Filter (LBB) | Šaltų tonų filtras (LBB) | Applied to catalog |
| Cooling Filter (82) | Šaltų tonų filtras (82) | Applied to catalog |
| Export Preferences… | Eksportuoti parenkant nuostatas... | Applied to catalog |
| Filter | Filtrai | Applied to catalog |

## Current catalog details
- PhotoCraft translation catalog PR: https://github.com/storytold/craft-i18n/pull/295
- Fork: rytumb-cmyk/craft-i18n-lt
- Catalog path: locales/lt/photocraft.tsv
- PR branch: add-lithuanian-photocraft-catalog
- The catalog contains Basic = Pagrindinis; Light = Šviesa; fontWeight Light = Plonas; cameraRaw Light = Šviesa.
- The screenshot-confirmed warming/cooling filter preset rows have been added to the catalog.

## Outstanding checks
- Locate the exact source key for Pixel Art Preview in the application/source catalog and add „Pikselinio meno peržiūra“ to the actual translation TSV; do not invent a key.
- Locate exact source keys for RAW Develop / RAW Develop Filter in the application source or source catalogs; these keys were not found in the current PhotoCraft TSV at the last check.
- Audit remaining mismatches and untranslated UI labels against the approved terminology above.
- Check consistency of Red Eye entries: current catalog has Red Eye Tool / Red Eye as „Raudonų akių šalinimas“, while the approved general term is „Raudonų akių koregavimas“; decide/apply consistently after checking context.
- Current catalog has Reds = „Raudoni atspalviai“ and Yellows = „Geltoni atspalviai“; retain unless the user explicitly changes these decisions.
- Select Data Points currently appears as „Pasirinkti duomenų taškus“; do not change without explicit confirmation.
