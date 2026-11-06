# Kinder- und Hausmärchen
Brüder Grimm.

Source: the 7th edition of 1857 ("Ausgabe letzter Hand", public domain), from German Wikisource. Fetched with `python3 scripts/grimm_fetch.py` → `source/chNNN.txt`, one tale per file in KHM order; line 2 of each file gives the KHM number. The illustrations come from the Russian fb2 edition in `Sources/` (19th-century engravings, some with Russian captions printed on them by the 2017 publisher; personal use only) and are placed with `python3 scripts/grimm_images.py`.

## This book is different: German → easier German
The source is already German, but 19th-century German. The task is an **adaptation**, not a translation:
- Retell each tale in modern German at the stage's level, with modern spelling (*dass*, not *daß*; *fing*, not *fieng*; *Tür*, not *Thür*).
- Keep the plot, every motif, the repetitions (the threefold tasks, the refrains), the formulaic openings and endings (*Es war einmal …*, *Und wenn sie nicht gestorben sind, so leben sie noch heute*), and the dry humour of the comic tales.
- Rhymes and spells (*Spieglein, Spieglein an der Wand …*, *Rapunzel, Rapunzel, lass dein Haar herunter*) are part of German culture. Keep them in their well-known wording, modernised in spelling only, and mark the hard words.
- Tales in Low German or other dialect (e.g. *Von dem Fischer un syner Fru*, *Von dem Machandelboom*) are retold in standard German. Keep one refrain line in dialect, followed by the standard-German version in the text.
- **No content changes, ever.** Characters, their names and roles («der Jude», «die Stiefmutter»), their way of speaking, the violence, the punishments and the morals stay exactly as in 1857. Only the *language* is simplified to the stage. Old words that the reader needs to recognise the original are kept and glossed, not replaced by modern euphemisms.
- At the B2 stage, stay close to the original's wording and rhythm, but modernise grammar and words that a reader today would not understand.

## Level progression (by source word count, at tale boundaries; 211 units ≈ 261,000 words)

| Units | Content | Stage | Narration tense |
|---|---|---|---|
| 1–29 | KHM 1–29 (Froschkönig … Teufel mit den drei goldenen Haaren) | A2 | Präsens |
| 30–58 | KHM 30–58 | A2 (upper) | Präsens |
| 59–90 | KHM 59–90 | A2 → B1 bridge | Präteritum |
| 91–135 | KHM 91–135 | B1 | Präteritum |
| 136–211 | KHM 136–200 (incl. 151*) and the ten Kinderlegenden | B2 | Präteritum |

Unit numbers differ from KHM numbers after 151, because the 1857 edition has an extra tale 151* («Die zwölf faulen Knechte», unit 152). Units 202–211 are the «Kinderlegenden». The first of them (unit 202) opens with the part heading `# Kinderlegenden`.

**A2 and the fairy-tale past tense:** in the A2 stages the tales are told in the Präsens, like the other books. The famous opening stays as it is («Es war einmal …»), and the closing formula «Und wenn sie nicht gestorben sind, dann leben sie noch heute» too. These are fixed formulas, not narration.

## Format
- Every tale is one unit: `## <title in modern spelling>`, no "Kapitel N".
- Use `— ` dashes for dialogue, as in the other books, even though the 1857 text uses quotation marks.
- Each `[[IMG:i_NNN.jpg]]` marker becomes `![](img/i_NNN.jpg)` on its own line, in the same place.
