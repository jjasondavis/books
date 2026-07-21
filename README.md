# Books Source Library

Reusable primary-text and historical-source archive for book projects.

This repository keeps two layers:

- `raw/` files are untouched downloads used to audit wording, metadata, and provenance.
- `reading/` and `index/` files are mechanically derived conveniences. They are not
  independent editions and must always point back to the raw witness and source URL.

## Current collections

- John Cassian: *Institutes* V and VII-XII in the public-domain C. S. Gibson/NPNF
  translation, Conferences I, II, and V, a full Latin text, and a Latin/English
  reading page for the omitted NPNF Book VI.
- Evagrius Ponticus: the complete *Praktikos* in Luke Dysinger's English translation;
  the *Antirrhetikos* in Frankenberg's Syriac transcription, Frankenberg's Greek
  retroversion, and Lazar Nesic's Serbian translation; plus a parallel TSV index.

## Textual cautions

- The complete *Antirrhetikos* does not survive in its original Greek. The file labeled
  `greek-retroversion` is Frankenberg's reconstruction from Syriac, not Evagrius's
  surviving Greek original.
- The Syriac file is a transcription of the principal complete witness used here.
- A fresh English working translation for a manuscript must identify its textual base
  and must not be presented as David Brakke's copyrighted wording.
- The NPNF editors omitted Cassian's *Institutes* Book VI. Use the Latin text and the
  separate Dysinger/Kardong-Bertram reading page; do not imply that Gibson translated it.
- Source pages and derived reading copies are research aids, not substitutes for a
  critical edition where a disputed reading matters.

See `SOURCES.md` for URLs, edition status, and reuse notes. `CHECKSUMS.sha256` records
the raw files captured on 2026-07-21.
