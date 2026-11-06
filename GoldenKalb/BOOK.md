# Das Goldene Kalb
Ilja Ilf, Jewgeni Petrow.

Source: `Sources/Ilf, Petrov, 12 Stuliev.pdf`, PDF pages 328–641: «Золотой теленок» (Russian, 1931/1933; the authors died in 1937 and 1942, so the work is public domain in Germany/EU). Unit 1 is the authors' preface «От авторов»; units 2–37 are chapters 1–36. The edition's 2020 footnotes are not part of the work and are not translated.
Extraction: `.venv/bin/python scripts/extract_images.py goldenes-kalb` and `python3 scripts/ilf_petrov_pdf.py goldenes-kalb` → `source/chNN.txt`.

## Level progression (by source word count, at chapter boundaries)

| Units | Content | Stage | Narration tense |
|---|---|---|---|
| 1–6 | preface, Part 1 ch. 1–5 | A2 | Präsens |
| 7–10 | Part 1 ch. 6–9 | A2 (upper) | Präsens |
| 11–17 | Part 2 ch. 10–16 | A2 → B1 bridge | Präteritum |
| 18–26 | Part 2 ch. 17–25 | B1 | Präteritum |
| 27–37 | Part 3 ch. 26–36 | B2 | Präteritum |

## Format
- Unit 1: `## Von den Autoren` (no "Kapitel").
- Units 2–37: `## Kapitel N: <German title>`, where N is the chapter number 1–36 (unit number minus 1).
- A `ЧАСТЬ …` line opens a part: a `# ` heading (see `GLOSSAR.md`). An `ЭПИГРАФ:` line becomes an italic epigraph under it, with the line breaks given by « / ».
- Signs, posters and documents that the source sets in capitals or as separate lines (e.g. «РОГА И КОПЫТА», the jubilee kit in ch. 27) stay as separate lines.

## Relation to «Zwölf Stühle»
This is the sequel. Ostap Bender's catchphrases and recurring terms must match `books/zwoelf-stuehle/GLOSSAR.md`. The overlapping rows are copied into this book's `GLOSSAR.md`.
