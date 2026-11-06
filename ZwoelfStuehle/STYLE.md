# Übersetzungsrichtlinien / Translation style guide

Source: Ilf & Petrov, «Двенадцать стульев» (1928 first-edition text, public domain), PDF pages 14–325. Translate directly from the Russian chapter files in `work/ru/`. Do not use or imitate published German translations, and do not translate the 2020 edition's editorial footnotes.

The reader is a German learner who reads Russian. The book is meant both as reading pleasure and as a vocabulary course, so the difficulty rises gradually through the book.

## Level progression (by Russian word count, at chapter boundaries)

| Chapters | Level | Narration tense | Notes |
|---|---|---|---|
| 1–7 | A2 | Präsens | strict A2 |
| 8–14 | A2 (upper) | Präsens | more relative clauses; Präteritum of frequent verbs in flashbacks |
| 15–21 (Part 2 up to «Экзекуция») | A2 → B1 bridge | **Präteritum** | Präteritum narration starts with Part 2; first *obwohl*, *damit*, *um … zu* |
| 22–31 (to «В театре Колумба») | B1 | Präteritum | |
| 32–41 (Part 3) | B2 | Präteritum | close to the original's register |

## A2 rules (chapters 1–14)
- Narration in **Präsens**. Use the Perfekt in dialogue and for earlier events. Use the Präteritum only for *sein*, *haben*, the modal verbs and *es gab*; from chapter 8 it is also allowed for frequent verbs in flashbacks.
- Short sentences, ideally ≤ 12–15 words. Allowed connectors: und, aber, oder, denn, deshalb, dann, trotzdem; subordinate clauses with weil, dass, wenn, als, ob, w-words. Simple relative clauses (Nominativ/Akkusativ) are allowed, used more often from chapter 8.
- No Konjunktiv II except *würde gern*, *möchte*, *hätte gern*. No passive. No Genitiv (use *von* + Dativ), except in fixed names.
- Cut descriptive clutter that adds no humour. Long Russian period sentences become 2–4 short sentences. Never cut a joke; simplify its wording instead.

## Bridge (chapters 15–21)
- Narration in **Präteritum**.
- Introduce B1 grammar one feature at a time: obwohl, damit, um … zu, während, nachdem; the Konjunktiv II *wäre/hätte/könnte*; an occasional simple passive.
- Sentences up to about 18 words.

## B1 rules (chapters 22–31)
- Präteritum. Subordinate clauses with obwohl, damit, während, bevor, nachdem, seit, um … zu. Full relative clauses. Simple passive (Präsens/Präteritum). Konjunktiv II for wishes, irreality and polite requests. Genitiv in common phrases.
- Common idioms are welcome when they carry humour. Sentences up to about 20 words.

## B2 rules (chapters 32–41)
- Close to the original's register: Präteritum, Plusquamperfekt, Konjunktiv I in reported speech (newspaper style, official papers), Konjunktiv II Vergangenheit, Passiv with modal verbs, Partizipialattribute, nominal style for bureaucratic parody.
- Keep Ilf & Petrov's long ironic sentences, though they may be split once if a sentence gets very long.

## Vocabulary (the educational part)
- **Deliberately enrich vocabulary.** Don't reduce everything to the 1,000 most common words. Each chapter should introduce plenty of new words at roughly the current level or one step above. Chapter 1 has about 240 marked words; later chapters will repeat many of them and add new ones, so aim for well over 100 marked words per chapter and mark generously. Prefer the precise, natural German word over a vague paraphrase when the word is useful (*flüstern*, not *leise sprechen*; *geizig*, not *will kein Geld geben*). Reuse words already introduced so they get repeated.
- **Mark every word a learner at the current level might not know** with `{{Wortform|Lemma|русский перевод}}`:
  - `Wortform` is the form exactly as it appears in the sentence.
  - `Lemma` is the dictionary form: nouns with article and plural (`der Sarg, die Särge`), verbs in the infinitive with separable prefix and, for strong verbs, the Präteritum and Perfekt forms (`verbieten (verbot, hat verboten)`), reflexive verbs with *sich*, and adjectives in their base form.
  - The translation is a short Russian equivalent that fits the context.
  - Mark idioms and fixed phrases as a whole: `{{zum Kuckuck noch mal|zum Kuckuck noch mal!|чёрт побери!}}`.
  - In chapters 1–21, the threshold is "a fresh A2 learner probably does not know it" (so *Beerdigungsbüro*, *geizig*, *Schnurrbart* get marked, but *Haus*, *gehen*, *schön* do not). In B1 chapters, mark B1+ words; in B2 chapters, mark B2+ words.
  - Don't worry whether a word was already marked in an earlier chapter. Mark it whenever it would be new to the reader; the build script keeps only the first occurrence in the whole book. Within a chapter, mark the word at least on its first occurrence (marking it more often is harmless).
  - Do not mark proper names. Do not put markup inside headings.

## Humour
- Every joke, ironic aside, catchphrase and absurd detail survives. At lower levels, rephrase it in simpler words; do not drop it.
- Russian wordplay with no German equivalent at that level: replace it with a German joke that has the same function and target. Do not explain it.
- Soviet realia: keep them when they are funny. Otherwise add a short neutral gloss in the text («das Standesamt», «die Kreismiliz»), not a footnote.
- Running gags must stay identical every time they appear. See `GLOSSAR.md`.

## Draft format (`drafts/kapitel-NN.md`)
- If the chapter opens a part (chapters 1, 15, 32), start with `# Erster Teil: Der Löwe von Stargorod` (or the equivalent for the other parts; see `GLOSSAR.md`).
- Then the chapter heading `## Kapitel N: <German title>`, followed by the text. Dialogue uses `— ` dashes as in the original.
- Every `[[IMG:pNNN.jpg]]` marker in the Russian file becomes `![](img/pNNN.jpg)` on its own line, at the same place in the text (between the same paragraphs).
- No word list at the end; `scripts/build.py` generates it.
- Build the reader edition with `python3 scripts/build.py`, which writes `de/`.
