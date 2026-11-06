# Sherlock Holmes, Band I
Arthur Conan Doyle.

Source: `Sources/The Complete Sherlock Holmes Vol. I - Sir Arthur Conan Doyle.epub` (English, 1887–1902, public domain). It contains five works: «A Study in Scarlet», «The Sign of Four», «The Adventures of Sherlock Holmes», «The Memoirs of Sherlock Holmes» and «The Hound of the Baskervilles». Only Doyle's text is used: the Barnes & Noble introductions, notes, footnotes and questions are excluded.
Extraction: `.venv/bin/python scripts/epub_extract.py sherlock-holmes` → `source/chNN.txt` (64 units; an extra `PART:` line marks the first unit of each work).

## Level progression (by source word count, at work/story boundaries)

| Units | Work | Stage | Narration tense |
|---|---|---|---|
| 1–14 | Eine Studie in Scharlachrot | A2 | Präsens |
| 15–26 | Das Zeichen der Vier | A2 (upper) | Präsens |
| 27–35 | Die Abenteuer, stories 1–9 | A2 → B1 bridge | Präteritum |
| 36–49 | Die Abenteuer, stories 10–12, and Die Memoiren | B1 | Präteritum |
| 50–64 | Der Hund der Baskervilles | B2 | Präteritum |

Watson narrates in the first person. In the A2 stages his narration is in the Präsens («Ich treffe Holmes zum ersten Mal …»); in dialogue, the Perfekt is used for the past.

## Format
- `PART: <title>` in the source becomes a `# ` heading with the German title of the work (see `GLOSSAR.md`). Text that follows it on the part page (e.g. the dedication of the «Hound», or the subtitle «Being a reprint from the reminiscences of John H. Watson, M.D.») goes in italics under that heading.
- Novel chapters: `## Kapitel N: <German title>`, with N counting within the work, as in the source. Stories: `## <German title>`.
- The images (the torn note in «The Reigate Puzzle», the plan in «The Naval Treaty») keep their place. Explain any English writing in them in the surrounding text.
