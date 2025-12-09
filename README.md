# JPEZ
Tool to simulate determinism in Japanese pronunciation for learners

## What is this?

In Japanese, many words are written using kanji.  
A single kanji can have multiple readings, and the correct pronunciation of a word is often **not directly predictable** from its written form.  
Learning Japanese vocabulary therefore usually means memorizing the specific reading of each word individually.

JPEZ explores a different angle: it tries to **simulate determinism** in pronunciation by providing pronunciation-oriented filtering options over a large Japanese vocabulary dataset.

In practice, learners can:

- filter out all words where a given kanji is **not** pronounced in a user-selected way  
- select exactly one reading per kanji and obtain a subset of words whose pronunciation is then locally *deterministic* for that learner

The idea: if every kanji in your active vocabulary has only one active reading, the resulting words become easier to read, recall and internalize.

## Initial scope

Current (initial) scope of JPEZ:

- Filtering by **word length** (e.g. 1–2 kanji compounds)
- Filtering by **pronunciation** (per kanji reading)
- Filtering to **words consisting of Jōyō kanji only**

The goal is not to cover every aspect of Japanese proficiency, but to target the **time-consuming problem of learning kanji-based vocabulary** by making pronunciation more predictable within a controlled subset of words.

## Data sources

JPEZ is built on top of existing open dictionary projects:

- **JMDict** – core Japanese lexicon
- **JmdictFurigana** (by Doublevil) – furigana segmentation and per-word readings
- **nihongo** (by sph-mn) – Jōyō kanji lists and readings

As of now, **JMnedict** (names, places, etc.) is intentionally excluded from the scope.
