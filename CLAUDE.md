# CLAUDE.md — working conventions for the `books` text-library

This repo is a personal, durable, **searchable and quotable** public-domain (+ owned) text library that
backs several book projects — chiefly **ChainBreaker** (the eight thoughts / *logismoi*, spiritual
warfare, guarding the mind). It is a **private** GitHub repo (`github.com/jjasondavis/books`).

## ⭐ Quoting policy (fair use) — READ FIRST

This library mixes **public-domain** texts and **owned-copyright** texts (the owner's purchased ebooks
and copyrighted translations). Both are here for **personal research use**, and both may be **quoted
briefly**:

> **Short, cited quotation is allowed from ANY text in this repo — public-domain or owned-copyright.**
> Under U.S. fair use (17 U.S.C. §107), a **sentence or two, at most a short paragraph**, used for
> commentary/criticism/scholarship, **with attribution (local file path + line)**, and not reproducing
> the "heart" of a short work, is a strong fair-use posture — exactly what the research briefs do.

Rules of thumb:
- **Do NOT tag owned-copyright works as "can't quote."** Quote them **short and cited**; paraphrase
  anything longer. The Philokalia, the *Ladder*, *Talking Back*, *Glittering Vices*, the acedia cluster,
  etc. are all quotable in the briefs this way — not merely paraphrasable.
- **Longer excerpts, whole poems, or the core of a short work** need a genuinely public-domain source or
  permission. For anything you might quote at length, prefer a PD text (zero-risk).
- The **private repo itself** (personal use) is unaffected by any of this — the policy matters at
  *publication* (the briefs, and ultimately the manuscript).
- This is a **working convention, not legal advice.** The final published manuscript should get a real
  IP review; when in doubt on a long or central quote, get permission.

Every quotation in a brief must be **verified verbatim** against the source file and cited as
`path/to/file.md:line`. Never invent or approximate a quote. (See also the root project rule: no
unverified facts in outward-facing writing.)

## Repo layout

- **Divisions** (top-level folders): `patristics/`, `tradition/`, `jewish/`, `scripture/`, `reference/`,
  `classical/`, `business/`, `self-improvement/`, `world-religions/`, `owned-library/`.
- **Per work:** either author-grouped (`<division>/<author-slug>/reading/<work>.md`, older pattern) or
  per-work (`<division>/<slug>/reading/<slug>.md`, used for bulk imports). Raw source kept under
  `.../raw/<source>/` alongside `reading/`.
- **Reading copy header** (3–4 lines): an HTML comment describing provenance, a `Source URL:` or
  `Source file:` line, and a `Title/Edition:` line ending in the license (`public domain.` or
  `owned copyright — personal use, do not distribute.`). OCR sources say `OCR-verify`.
- `CATALOG.tsv` — the research index, **15 tab-separated columns**:
  `id, author, author_birth, author_death, title, composed_circa, translator, translation_year,
  tradition, language, topics, source, source_url, local_path, license`. One row per `reading/*.md`.
  Invariants: exactly 15 fields per row, no duplicate `id`, every `local_path` resolves.
- `SOURCES.md` — dated provenance ledger. `CAPTURE-PLAN.md` — schema + controlled vocab + punch-list.
  `COLLECTION-ROADMAP.md` — PD works to own. `books_to_purchase.md` — the ebooks.com buy list.
- `research/` — diachronic **briefs** (e.g. the eight-thoughts + guarding-the-heart studies). Method:
  pick a theme → corpus-wide grep of `**/reading/**/*.md` → cite a local witness per era → name the
  continuity and the drift. Enrichments are added as dated `— Update YYYY-MM-DD —` blocks that
  **preserve** existing content.

## License tagging

- **Public domain:** US works published ≤ 1930 (advancing yearly), or Gutenberg `copyright:false`.
  Translations carry their **own** copyright from the translation date — a PD original in a modern
  translation is `owned-copyright` (the translation), even though the underlying text is ancient.
- **owned-copyright:** the owner's purchased ebooks and copyrighted translations. Segregated where
  practical, but the `license` column in `CATALOG.tsv` is the authoritative PD-vs-owned filter (so the
  repo can be filtered/excluded by license if ever needed, regardless of folder).

## Hard rules

- **TEXT ONLY.** No binaries in this repo — scans, page-image PDFs, images, ebooks (`*.pdf, *.epub,
  *.mobi, *.azw*, images, audio, archives`) are blocked by `.gitignore`. Scanned/image material goes to
  **`D:\repos\scans`** (Axcient-backed, off-repo). Extract text into `reading/` here; keep the binary there.
- **Every reading copy needs a header** and **every catalog row needs 15 fields + a unique id.**
- Commit trailer: `Co-Authored-By: Claude Opus 4.8 <noreply@anthropic.com>`.
  Push remote (username in URL to avoid prompts):
  `git push https://jjasondavis@github.com/jjasondavis/books.git main`. LF→CRLF warnings are harmless.

## Ingestion workflow (`books_to_process`)

Source files are dropped in **`D:\repos\books_to_process`** (not on OneDrive). To ingest: extract text
(EPUB via the spine-ordered XHTML extractor `scratchpad/epub2txt.py`; PDF via `pdftotext`), write a
`raw/` copy + a headered `reading/*.md`, add a `CATALOG.tsv` row, place by division, then run a
**completeness audit** (every source file vs ingested `Source file:` headers) so nothing is missed, and
**skip duplicates** (`_nodrm_1`/`_1` re-downloads, titles already present). Kindle **Topaz** `.azw1` and
files whose key is in the newest `.kinf2024` cannot be de-DRMed by current open tools.

## Network note

`archive.org` and `ccel.org` are blocked/interfered-with from this machine (DNS / TLS-SNI). Reach
archive.org via `scratchpad/dnsfetch.ps1` (resolves hosts via DNS 8.8.8.8, keeps SNI + cert validation).
CCEL fails even through that (SNI reset) — use archive.org or another mirror. **Subagents cannot reach
archive.org** — recover archive-only items in the main session.
