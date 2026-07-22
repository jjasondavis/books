# Books Source Library

Reusable primary-text and historical-source archive for book projects.

This repository keeps two layers:

- `raw/` files are untouched downloads used to audit wording, metadata, and provenance.
- `reading/` and `index/` files are mechanically derived conveniences. They are not
  independent editions and must always point back to the raw witness and source URL.

## Current collections

Captured 2026-07-21, expanded 2026-07-22 (Phase A acquisition). See `SOURCES.md` for
per-item URLs, editions, and reuse notes.

- **John Cassian** — *Institutes* I-V and VII-XII and the complete *Conferences*
  (I-XI, XIII-XXI, XXIII-XXIV) in the public-domain C. S. Gibson / NPNF translation;
  a Latin/English reading page for the NPNF-omitted *Institutes* VI; the complete Latin
  *De coenobiorum institutis*; and the complete Latin *Collationes* (all 24 conferences,
  including XII and XXII, which are absent from the NPNF English).
- **Evagrius Ponticus** — the complete *Praktikos* (Dysinger English); the *Antirrhetikos*
  in Syriac, Greek retroversion, and Serbian with a parallel index; *Peri Logismon*
  (On Thoughts) and *De oratione* (On Prayer) in Dysinger's English plus the
  evagriusponticus.net critical/parallel Greek, Latin, and Serbian witnesses.
- **Athanasius** — the *Life of Antony* (NPNF, Ellershaw).
- **John Chrysostom** — *No One Can Harm the Man Who Does Not Injure Himself* and the
  complete *Homilies on the Statues* (21 homilies), NPNF First Series Vol. 9.
- **John Climacus** — the Greek *Scala Paradisi* (Migne PG 88) as a base text; no
  public-domain English translation exists.
- **Apophthegmata** — Budge, *The Paradise of the Holy Fathers* (1907, Chatto & Windus),
  vols. 1-2, searchable scans.
- **Augustine** — *Confessions* (Pusey translation, Project Gutenberg).
- **The mind-cleansing tradition** (`tradition/`) — James Allen, *As a Man Thinketh*;
  John Owen, *The Mortification of Sin* and *Of Temptation*; Thomas Brooks, *Precious
  Remedies Against Satan's Devices* (original-edition scan + modern typeset PDF);
  Thomas à Kempis, *The Imitation of Christ* (Benham).

## Textual cautions

- The complete *Antirrhetikos* does not survive in its original Greek. The file labeled
  `greek-retroversion` is Frankenberg's reconstruction from Syriac, not Evagrius's
  surviving Greek original.
- The Syriac file is a transcription of the principal complete witness used here.
- A fresh English working translation for a manuscript must identify its textual base
  and must not be presented as a copyrighted modern translator's wording.
- The NPNF editors omitted Cassian's *Institutes* Book VI. Use the Latin text and the
  separate Dysinger/Kardong-Bertram reading page; do not imply that Gibson translated it.
- Cassian *Conferences* XII and XXII are absent from the NPNF English; the only witness
  here is the Latin *Collationes*. A quotation from either must come from that Latin (or a
  rights-checked modern translation), never from the NPNF set.
- Evagrius' *Peri Logismon* and *De oratione* English pages are Luke Dysinger's research
  translations shown with parallel Greek; verify wording before any print quotation.
- No public-domain English *Ladder of Divine Ascent* exists; the captured PG 88 Greek is a
  base text only. Chrysostom's *On Vainglory* and the English *Philokalia* were not
  captured (no public-domain witness / copyrighted); see `SOURCES.md` gaps.
- Modern typeset PDFs (the preachtheword Brooks) and OCR text layers (Budge, Climacus) are
  research aids; verify against the page images or an original edition where a disputed
  reading matters.
- Source pages and derived reading copies are research aids, not substitutes for a
  critical edition where a disputed reading matters.

See `SOURCES.md` for URLs, edition status, reuse notes, and recorded gaps.
`CHECKSUMS.sha256` records every raw file.
