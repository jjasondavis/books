# Capture Plan — text-first public-domain acquisition (punch list)

Execution layer under `COLLECTION-ROADMAP.md`. This file is what the capture agents follow.

## Operating policy

- **Text-first. Skip image-only scans.** Capture clean transcriptions (Gutenberg, CCEL,
  Wikisource, Standard Ebooks, New Advent). Do NOT capture image-only PDFs expecting to OCR
  them for quotation. The existing Greek scans (Philokalia 1782, Climacus PG 88) stay as
  reference *witnesses* only — never OCR-quote them.
- **No binaries in the repo — ever.** This repo is text-only. Any scanned PDF, image, e-book
  binary, audio/video, or archive belongs in `D:\repos\scans` (Axcient-backed, off-repo),
  mirroring its sub-path, NOT here. A `.gitignore` blocks these extensions as a safety net;
  if a capture agent lands a binary in the repo tree, relocate it to `D:\repos\scans` and
  record it in `D:\repos\scans\CHECKSUMS.sha256`.
- **Model policy (cost).** Bulk fetching runs on **Sonnet** subagents (reliable for site
  structure). **Haiku** may run pure known-URL fetch loops. **Opus** (the orchestrator) does
  planning, tricky source-hunting, and QC only. The download itself is tool calls, so the
  cheap model is doing cheap orchestration, not expensive reasoning.
- **Every capture writes:** raw text in `raw/<source>/`, a cleaned reading copy in `reading/`
  when the raw isn't already clean prose, one row in `SOURCES.md`, one row in `CATALOG.tsv`
  (below), and a `CHECKSUMS.sha256` entry.
- **Verify each item is truly public domain** (see the copyright rule in the roadmap). ⚠ items
  need a per-edition/translation check before capture; when unclear, skip and log.

## Research metadata — `CATALOG.tsv` (the diachronic substrate)

Maintain one tab-separated row per work so the corpus is queryable across centuries. Columns:

`id  author  author_birth  author_death  title  composed_circa  translator  translation_year  tradition  language  topics  source  source_url  local_path  license`

- `tradition` ∈ {apostolic, patristic-greek, patristic-latin, desert, byzantine, medieval,
  reformation, puritan, catholic-devotional, orthodox, evangelical, stoic, new-thought,
  business, scripture, reference, jewish, world-religions, classical, medieval}
- `topics` = semicolon list from a controlled vocab: repentance; prayer; anger; sorrow;
  acedia; vainglory; pride; gluttony; lust; avarice; humility; watchfulness; discernment;
  temptation; spiritual-warfare; contentment; suffering; wealth; work; leadership; character;
  self-discipline; providence; grace; sanctification; envy; wisdom; apologetics; scripture.
- `composed_circa` uses the *authorship* era (for ancient works), `translation_year` the PD
  English edition. Both matter: trend analysis keys on `composed_circa`, quote-checking on the
  translation.

This index is what later research passes (trend/diachronic analysis, concordance, theme
tracing) run against. Build it as we go.

## Source recipes (so cheap agents don't flail)

- **Project Gutenberg:** find id via Gutendex — `https://gutendex.com/books?search=<title author>` →
  read `results[].id` and confirm the author/translator; then fetch UTF-8 text
  `https://www.gutenberg.org/cache/epub/<id>/pg<id>.txt`. Reading copy = strip the
  `*** START/END ... ***` boilerplate (see `scratchpad/convert-text.ps1 -Kind gutenberg`).
- **CCEL:** author page `https://ccel.org/ccel/<author>`; work landing `.../<work>/<work>`;
  plain text `https://ccel.org/ccel/<L>/<author>/<work>/cache/<work>.txt` (note the single
  letter directory). Reading copy via `convert-text.ps1 -Kind ccel`.
- **New Advent (ANF/NPNF):** `https://www.newadvent.org/fathers/<nnnn>.htm`; multi-part works
  have an index page linking sub-pages. Reading copy via `convert-newadvent.ps1` (auto-detects
  translator/volume from the "About this page" block).
- **Wikisource:** article HTML; content lives in `mw-parser-output`, ends at `printfooter`.
- **Standard Ebooks:** per-book page → download the plain-text or EPUB (CC0).
- Prefer the source that yields **clean UTF-8 text**; fall back CCEL→Gutenberg→Wikisource.

---

## Punch list by phase

Format: `author — work (≈date) → source`. Agents resolve exact URLs via the recipes. Target
path: `<division>/<author-slug>/raw/<source>/…` and matching `reading/`.

### Phase 1 — Reformation & Puritan core  ★ (run first)
- Calvin — *Institutes of the Christian Religion* (Beveridge tr.) → CCEL
- Calvin — *Commentaries* (start with Genesis, Psalms, Romans) → CCEL
- Luther — *Bondage of the Will*; *Commentary on Galatians*; *Table Talk* → CCEL/Gutenberg
- John Owen — *Mortification of Sin* [HAVE]; *Of Temptation* [HAVE]; *Of the Dominion of Sin
  and Grace*; *Indwelling Sin*; *Communion with God*; *The Glory of Christ* → CCEL
- Richard Baxter — *The Reformed Pastor*; *The Saints' Everlasting Rest*; *A Call to the
  Unconverted* → CCEL/Gutenberg
- John Bunyan — *The Pilgrim's Progress*; *The Holy War*; *Grace Abounding* → Gutenberg
- Jonathan Edwards — *Religious Affections*; *The Freedom of the Will*; *Sinners in the Hands
  of an Angry God*; *A Treatise Concerning Religious Affections* → CCEL
- Thomas Watson — *A Body of Divinity*; *The Doctrine of Repentance*; *The Art of Divine
  Contentment*; *All Things for Good* → CCEL/Gutenberg
- Thomas Brooks — *Precious Remedies* [HAVE, add clean text]; *The Mute Christian Under the
  Smarting Rod*; *Heaven on Earth* → CCEL/Gutenberg
- Richard Sibbes — *The Bruised Reed and Smoking Flax* → CCEL/Gutenberg
- Stephen Charnock — *The Existence and Attributes of God* → CCEL
- Jeremiah Burroughs — *The Rare Jewel of Christian Contentment* → CCEL/Gutenberg
- William Gurnall — *The Christian in Complete Armour* → CCEL
- John Flavel — *Keeping the Heart*; *The Mystery of Providence* → CCEL/Gutenberg
- Walter Marshall — *The Gospel Mystery of Sanctification* → CCEL
- Confessional: Westminster Confession + Larger/Shorter Catechisms; Heidelberg; Canons of
  Dort; 1689 Baptist Confession → CCEL/Gutenberg
- John Foxe — *Book of Martyrs* → Gutenberg

### Phase 2 — Evangelical & revival (18th–19th c.)
- Spurgeon — *Morning and Evening*; *All of Grace*; *Lectures to My Students*; *The Treasury
  of David*; *John Ploughman's Talk*; selected *Metropolitan Tabernacle Pulpit* sermons → CCEL/Gutenberg
- J. C. Ryle — *Holiness*; *Practical Religion*; *Expository Thoughts* → CCEL/Gutenberg
- Andrew Murray — *Humility*; *Abide in Christ*; *With Christ in the School of Prayer* → CCEL/Gutenberg
- E. M. Bounds — *Power Through Prayer* (+ prayer series) → CCEL/Gutenberg
- Wesley — *Sermons*; *A Plain Account of Christian Perfection*; *Journal* → CCEL
- Whitefield — *Sermons* → CCEL/Gutenberg
- Hannah Whitall Smith — *The Christian's Secret of a Happy Life* → Gutenberg
- George MacDonald — *Unspoken Sermons*; *Diary of an Old Soul* → Gutenberg
- Finney — *Lectures on Revivals of Religion* → CCEL/Gutenberg
- Horatius Bonar; Octavius Winslow; Robert Murray M'Cheyne → CCEL/Gutenberg

### Phase 3 — Bibles & reference
- PD English Bibles: KJV, ASV 1901, RV 1885, Douay-Rheims (Challoner), Young's Literal,
  Darby, Geneva 1599, Webster, Brenton LXX → eBible / Gutenberg / archive text
- Reference: Matthew Henry *Commentary*; John Gill *Exposition*; Adam Clarke *Commentary*;
  Jamieson-Fausset-Brown; Barnes' *Notes*; Strong's & Thayer's & BDB (PD eds.); Cruden's
  Concordance; Josephus (Whiston); Eusebius *Church History*; Schaff *History of the
  Christian Church* → CCEL/Gutenberg
- Original-language texts (text, not scans): TR (Scrivener), Westcott-Hort, Nestle 1904,
  Clementine Vulgate, Swete LXX, Westminster Leningrad Hebrew → SWORD/STEPBible

### Phase 4 — Catholic & Orthodox devotional
- Francis de Sales — *Introduction to the Devout Life*; *Treatise on the Love of God* → CCEL/Gutenberg
- Teresa of Ávila — *The Interior Castle*; *The Way of Perfection*; *Life* ⚠(PD tr.) → CCEL/Gutenberg
- John of the Cross — *Dark Night*; *Ascent of Mount Carmel* ⚠(Lewis 1864) → CCEL/archive text
- Ignatius of Loyola — *Spiritual Exercises* ⚠(PD tr.) → Gutenberg
- Brother Lawrence — *The Practice of the Presence of God* → CCEL/Gutenberg
- Scupoli — *The Spiritual Combat* → Gutenberg
- de Caussade — *Abandonment to Divine Providence* → Gutenberg
- Augustine — *City of God*; *Enchiridion*; *On the Trinity* → CCEL/New Advent
- Aquinas — *Summa Theologica* (Dominican tr.) → CCEL/Gutenberg
- Thomas à Kempis — *Imitation* [HAVE]
- *The Way of a Pilgrim* ⚠(verify tr. date) → archive text/Gutenberg
- Chesterton — *Orthodoxy* (1908); *The Everlasting Man* (1925) → Gutenberg

### Phase 5 — Self-improvement / character
- James Allen — *As a Man Thinketh* [HAVE]; *Eight Pillars of Prosperity*; *From Poverty to
  Power*; *The Mastery of Destiny*; *Above Life's Turmoil*; *The Way of Peace* → Gutenberg
- Wallace Wattles — *The Science of Getting Rich*; *…Being Great*; *…Being Well* → Gutenberg
- Orison Swett Marden — *Pushing to the Front* → Gutenberg
- Charles Haanel — *The Master Key System* (1912) → Gutenberg
- Napoleon Hill — *The Law of Success* (1928) ✓; ⚠ *Think and Grow Rich* (1937) NOT free → Gutenberg/archive
- Florence Scovel Shinn — *The Game of Life* (1925) → Gutenberg
- *The Kybalion* (1908); Russell Conwell — *Acres of Diamonds*; Elbert Hubbard — *A Message to
  Garcia*; Ralph Waldo Trine — *In Tune with the Infinite* → Gutenberg
- Samuel Smiles — *Self-Help*; *Character*; *Thrift*; *Duty* → Gutenberg
- Emerson — *Essays* (First & Second Series) → Gutenberg
- Franklin — *Autobiography*; *The Way to Wealth* → Gutenberg
- William James — *The Varieties of Religious Experience* → Gutenberg
- Stoics: Marcus Aurelius *Meditations* (Long); Epictetus *Enchiridion* & *Discourses*;
  Seneca *Letters* & *On the Shortness of Life* → Gutenberg

### Phase 6 — Business, economics & strategy
- Adam Smith — *The Wealth of Nations*; *The Theory of Moral Sentiments* → Gutenberg
- Carnegie — *The Gospel of Wealth*; *Autobiography* → Gutenberg
- P. T. Barnum — *The Art of Money-Getting* → Gutenberg
- Sun Tzu — *The Art of War* (Giles 1910) → Gutenberg
- Machiavelli — *The Prince* → Gutenberg
- J. S. Mill — *Principles of Political Economy*; *On Liberty* → Gutenberg
- Ricardo — *Principles of Political Economy and Taxation* → Gutenberg
- Marshall — *Principles of Economics* (1890) → Gutenberg
- Veblen — *The Theory of the Leisure Class* → Gutenberg

### Phase 7 — Complete the patristic set + medieval/mystical
- Remaining ANF/NPNF volumes (Augustine corpus, Basil, the Gregories, Jerome, Irenaeus,
  John of Damascus, Eusebius) → CCEL/New Advent
- Anselm; Bernard; Bonaventure; *The Cloud of Unknowing* ⚠; Julian of Norwich ⚠; Dante → Gutenberg/CCEL

### Phase 8 — Classical antiquity (Greeks & Romans)
- Plato — complete dialogues (Jowett tr.) → Gutenberg
- Aristotle — *Nicomachean Ethics*; *Politics*; *Rhetoric* → Gutenberg
- Plutarch — *Lives* (Dryden/Clough); *Moralia* → Gutenberg
- Xenophon — *Memorabilia*; *Cyropaedia*; *Anabasis* → Gutenberg
- Cicero — *On Duties (De Officiis)*; *On Friendship*; *On Old Age*; *Tusculan Disputations* → Gutenberg
- Diogenes Laertius — *Lives of the Eminent Philosophers* → Gutenberg
- (Stoics — Marcus Aurelius, Epictetus, Seneca — already in Phase 5)
- Herodotus; Thucydides; Homer — history/epic (optional, literary) → Gutenberg
- Aesop — *Fables* → Gutenberg

### Phase 9 — Jewish history & the Second-Temple world  ★ (run right after Phase 1)
The "what did the Jews know" angle: primary Jewish history + the cultural/daily-life,
customary, and idiomatic background a 2026 reader lacks. All public domain (text only).
- ★ **Josephus** — *Complete Works* (William Whiston tr., 1737): *Antiquities of the Jews*,
  *The Wars of the Jews*, *Against Apion*, *The Life of Flavius Josephus* → Gutenberg
- **Philo of Alexandria** — *The Works of Philo* (C. D. Yonge tr., 1854) → Gutenberg/earlychristianwritings
- ★ **Alfred Edersheim** — *The Life and Times of Jesus the Messiah*; *Sketches of Jewish
  Social Life*; *The Temple: Its Ministry and Services*; *Bible History: Old Testament* → CCEL/Gutenberg
- **Emil Schürer** — *A History of the Jewish People in the Time of Jesus Christ* (PD English tr.) → archive text
- **R. H. Charles** — *The Apocrypha and Pseudepigrapha of the Old Testament* (1913, 2 vols) → archive text/sacred-texts
- **The Apocrypha / Deuterocanon** (KJV 1611; RV 1895) → Gutenberg
- **Babylonian Talmud** — Rodkinson tr. (1903, PD; ⚠ Soncino is copyrighted) → sacred-texts
- **The Targums** — J. W. Etheridge tr. (1862) → sacred-texts
- **The Mishnah** — ⚠ Danby 1933 is copyrighted; use only a confirmed PD older partial (e.g., Barclay 1878) or skip
- **George Foot Moore** — *Judaism in the First Centuries of the Christian Era* (1927, PD) → archive text
- **The Jewish Encyclopedia (1901–1906)** — massive PD reference on Jewish law, custom, daily
  life, idiom; ideal for the "cultural references someone in 2026 won't know" goal → jewishencyclopedia.com / archive text

### Phase 10 — World religions & comparative texts (apologetics reference)
For apologetics / comparative work. Text only, English, public domain. The monumental
umbrella source is **Max Müller's *Sacred Books of the East* (SBE)**, 50 vols, Oxford
1879–1910 (all PD); plus **sacred-texts.com** and Gutenberg.
- **Islam:** The Qur'an — PD English: George Sale (1734); J. M. Rodwell (1861); E. H. Palmer
  (SBE 6 & 9, 1880); Muhammad Ali (1917). ⚠ Pickthall (1930) is now US-PD as of 2026;
  Yusuf Ali (1934) is NOT PD. ⚠ Major hadith collections (Bukhari, Muslim) survive mostly in
  copyrighted modern translations — capture only if a confirmed PD English exists.
- **Hinduism:** *Bhagavad Gita* (Edwin Arnold, *The Song Celestial*, 1885; Telang, SBE 8);
  *The Upanishads* (Müller, SBE 1 & 15; R. E. Hume, *Thirteen Principal Upanishads*, 1921);
  *Rig Veda* (Griffith, 1896); *Ramayana* (Griffith); *Mahabharata* (Ganguli/Roy, complete,
  1883–96); *The Laws of Manu* (Bühler, SBE 25); *Vishnu Purana* (H. H. Wilson, 1840);
  *Yoga Sutras / Raja Yoga* (Vivekananda, 1896).
- **Buddhism:** *The Dhammapada* (Müller, SBE 10); *Buddhist Suttas* (Rhys Davids, SBE 11);
  *The Jataka* (Cowell, 1895–1907); *The Questions of King Milinda* (Rhys Davids, SBE 35–36);
  *Lotus Sutra / Saddharma-Pundarika* (Kern, SBE 21); *Buddhism in Translations* (H. C. Warren,
  1896); *The Gospel of Buddha* (Paul Carus, 1894); *Buddhacarita / Life of Buddha* (Cowell,
  SBE 49); *The Tibetan Book of the Dead* (Evans-Wentz, 1927, now US-PD).
- **Cheap breadth from the same PD sources:** Confucian *Analects*, *Mencius*, *Doctrine of the
  Mean*, and the *Tao Te Ching* (James Legge, SBE); the Zoroastrian *Avesta* (SBE); the
  *Book of Mormon* (1830).

Store under a new top-level division `world-religions/<tradition>/<author-or-work>/`. Primary
sources: sacred-texts.com and archive.org (text), Gutenberg, and the SBE set.

## Run order & mandate

- **Mandate:** capture aggressively — local storage is abundant and cheap relative to the value
  of the material and of time; token costs may rise, so build the corpus now. **Text only**
  (no image scans). Keep going phase to phase without stopping for confirmation between phases.
- **Run order:** Phase 1 (Puritan/Reformed) → **Phase 9 (Jewish/Second-Temple, elevated)** →
  Phase 2 → 3 → 4 → 5 → 6 → 8 → 7 → **Phase 10 (world religions, apologetics)**. Adjust as
  sources dictate; log deviations.
- **Execution:** Sonnet worker agents per author-cluster write only their own author
  directories and return a manifest; the orchestrator (Opus) consolidates `SOURCES.md`,
  `CHECKSUMS.sha256`, and `CATALOG.tsv`, spot-checks, and commits per phase.

---

## Research agenda this corpus enables (the *why*)

Once `CATALOG.tsv` is populated, these become tractable — the kind of multi-century synthesis
that would take a human years:

1. **Diachronic theme-tracing** — follow one passion (e.g., anger, acedia, vainglory) from the
   desert eight thoughts → Cassian → Gregory's seven → the Puritans → Spurgeon → the New
   Thought writers; chart continuity and drift.
2. **Cross-tradition comparison** — how Orthodox *watchfulness*, Puritan *mortification*, and
   New-Thought *right thinking* describe the same inner mechanics in different vocabularies.
3. **Concept concordance** — every treatment of "guarding the heart / thoughts" across 1,800
   years, with citations, to source and stress-test a chapter's claims.
4. **Vocabulary/idiom shift** — how the language of the interior life changed by era, useful
   for pitching ancient ideas to a modern reader.
5. **Claim verification** — for each manuscript assertion, pull every primary witness that
   supports or complicates it, verified against the local text.

These run as later passes (their own plans), reading `CATALOG.tsv` + the captured text.
