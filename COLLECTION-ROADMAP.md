# Collection Roadmap — a personal, searchable, quotable public-domain library

**Purpose.** Build and *own* a durable local archive of out-of-copyright works useful for
Christian spiritual life, self-improvement, and business — searchable, quotable, and
checksummed — so that link-rot or paywalls on today's free sites (Gutenberg, CCEL,
archive.org, New Advent) can never take the material away. Everything here is public
domain; the vault stores a raw witness + (where clean) a reading copy, with provenance in
`SOURCES.md` and integrity in `CHECKSUMS.sha256`. Large scans go in Git LFS.

**Note on the "Puritan Hard Drive."** That product (Still Waters Revival Books) bundles
public-domain Puritan/Reformed works behind proprietary *software and compilation*. The
underlying texts are free; we acquire them directly from public-domain sources rather than
copying that product. This roadmap reproduces (and exceeds) its scope from open sources.

## Copyright rule of thumb (so we only capture what's truly free)

- **US:** works first published **in 1930 or earlier are public domain** (as of 2026); the
  wall advances one year every January 1. Sound recordings and some foreign works differ.
- **Life + 70:** unpublished works, and most countries outside the US, key off the
  *author's* (or *translator's*) death + 70 years. A modern *translation* of an ancient
  free text carries its own fresh copyright — always check the translator's dates.
- **Borderline items flagged below** with ⚠ — verify the specific edition/translation
  before capture. Examples: Napoleon Hill *Think and Grow Rich* (1937 — NOT free until
  2033) vs. *The Law of Success* (1928 — free); Dale Carnegie *How to Win Friends* (1936 —
  not free until 2032).

## Sourcing strategy (durable, public-domain-safe)

- **Project Gutenberg** (+ the Gutendex API for bulk lists) — clean UTF-8 text; best for
  self-improvement/business/literature.
- **CCEL** (Christian Classics Ethereal Library) — structured Christian classics; plain-text
  export at `/ccel/<L>/<author>/<work>/cache/<work>.txt`.
- **Internet Archive** — page scans (+ OCR `_text.pdf`); best authoritative witness for
  Puritan/Reformed folios and anything not cleanly transcribed. (Reach via DNS 8.8.8.8 if
  the local network blocks it.)
- **Wikisource** — transcribed texts (Latin, Greek, English), CC BY-SA presentation over PD text.
- **Standard Ebooks** — beautifully typeset PD works (CC0); great reading copies.
- **Post-Reformation Digital Library (PRDL)** — bibliographic index to Reformation/Puritan scans.
- **Bible / original languages:** eBible.org, the SWORD Project / CrossWire modules, STEPBible
  (open-licensed Hebrew/Greek), Unbound Bible.

**Format policy:** capture *text* (searchable/quotable) wherever a clean transcription
exists; capture *page scans* (PDF, LFS) where only images exist or the wording is disputed;
record both when available.

---

## The catalog

Legend: **[HAVE]** already in the vault · ⚠ verify edition/translation date · ★ high priority.

### A. Scripture & original-language base texts
- **English (PD):** KJV; American Standard Version 1901; Revised Version 1885; Douay-Rheims
  (Challoner); Young's Literal; Darby; Webster; Geneva Bible (1599); Tyndale; Wycliffe;
  Brenton's English Septuagint (1851). *Sources: eBible, Gutenberg, archive.org, SWORD.*
- **Original languages (PD):** Textus Receptus (Scrivener 1894); Westcott-Hort GNT (1881);
  Nestle 1904 GNT; Tischendorf; Clementine Vulgate; Swete's Septuagint (PD; ⚠ Rahlfs LXX is
  copyrighted); Leningrad/Westminster Hebrew (open license). *Sources: SWORD, STEPBible, archive.org.*

### B. Patristic (the great PD translation corpus)
- ★ **Ante-Nicene Fathers** (10 vols) + **Nicene & Post-Nicene Fathers** Series 1 (14) &
  Series 2 (14) — the whole 38-volume Schaff set, all PD. *Source: CCEL/New Advent.* Much of
  the on-theme material is **[HAVE]** already (Cassian, Evagrius, Athanasius, Chrysostom,
  Ambrose, Gregory of Nyssa, the Apostolic Fathers, Clement, Tertullian, Cyprian, Lactantius,
  Methodius, Origen). Completing the set gives Augustine's *City of God*, Basil, the Gregories,
  John of Damascus, Jerome, Irenaeus, etc.
- ★ **Gregory the Great, *Moralia in Job*** — **[HAVE]** (Library of the Fathers).
- **Schaff, *History of the Christian Church*** (8 vols) — reference. *CCEL.*
- **The Philokalia — Greek 1782** — **[HAVE]** (base text; English is copyrighted).

### C. Medieval & mystical
- ★ **Aquinas** — *Summa Theologica* (English Dominican Province, 1911-25, PD); *Catena Aurea*.
- **Anselm** — *Cur Deus Homo*, *Proslogion*. **Bernard of Clairvaux** — *On Loving God*,
  *On the Song of Songs*. **Bonaventure** — *The Journey of the Mind to God*.
- **Thomas à Kempis, *Imitation of Christ*** — **[HAVE]**.
- *The Cloud of Unknowing* (⚠ use a PD translation, e.g. Underhill 1912); **Julian of Norwich**
  *Revelations* (⚠ older PD translation); **Walter Hilton** *Scale of Perfection*.
- **Dante**, *Divine Comedy* (Longfellow / Cary, PD).

### D. Reformation & Puritan  ★ (the heart of the "Puritan library")
- **Calvin** — *Institutes* (Beveridge, 1845); the **Calvin Translation Society Commentaries**
  (45 vols, 1840s-50s). *CCEL/archive.org.*
- **Luther** — *Bondage of the Will*; *Commentary on Galatians*; *Table Talk*; *Ninety-Five
  Theses*; ⚠ (the modern 55-vol *Luther's Works* is copyrighted — use PD older translations).
- **John Owen** — *Works* (Goold ed., 16 vols) incl. *Mortification of Sin* **[HAVE]**,
  *Of Temptation* **[HAVE]**, *Indwelling Sin*, *Communion with God*, *The Glory of Christ*,
  the 7-vol *Hebrews*.
- **Richard Baxter** — *The Reformed Pastor*; *The Saints' Everlasting Rest*; *A Christian Directory*.
- **John Bunyan** — *Pilgrim's Progress*; *The Holy War*; *Grace Abounding*; *Works*.
- **Jonathan Edwards** — *Works* (PD eds.); *Religious Affections*; *Freedom of the Will*;
  *The End for Which God Created the World*; sermons.
- **Thomas Watson** — *A Body of Divinity*; *The Doctrine of Repentance*; *The Art of Divine
  Contentment*; *All Things for Good*.
- **Thomas Brooks** — *Precious Remedies Against Satan's Devices* **[HAVE]**; *The Mute
  Christian Under the Smarting Rod*; *Heaven on Earth*.
- **Richard Sibbes** — *The Bruised Reed*; **Stephen Charnock** — *Existence and Attributes of
  God*; **Jeremiah Burroughs** — *The Rare Jewel of Christian Contentment*; **William Gurnall**
  — *The Christian in Complete Armour*; **John Flavel** — *Works* / *Keeping the Heart*;
  **Thomas Goodwin** — *Works*; **Samuel Rutherford** — *Letters*; **John Bunyan**; **William
  Perkins**; **David Clarkson**; **Walter Marshall** — *The Gospel Mystery of Sanctification*.
- **Confessional / catechetical:** Westminster Confession & Larger/Shorter Catechisms;
  Heidelberg Catechism; Canons of Dort; Belgic Confession; 1689 London Baptist Confession.
- **Foxe, *Book of Martyrs*.** *Sources: CCEL, Gutenberg, Monergism, PRDL, archive.org.*

### E. Catholic devotional & mystical (PD)
- **Augustine** — *Confessions* (Pusey) **[HAVE]**; *City of God*; *Enchiridion*; *On the
  Trinity* (NPNF).
- **Francis de Sales** — *Introduction to the Devout Life*; *Treatise on the Love of God*.
- **Teresa of Ávila** — *The Interior Castle*; *The Way of Perfection*; *Life* (⚠ David
  Lewis / Stanbrook PD translations).
- **John of the Cross** — *Dark Night of the Soul*; *Ascent of Mount Carmel* (⚠ David Lewis 1864).
- **Ignatius of Loyola** — *Spiritual Exercises* (⚠ PD translation).
- **Brother Lawrence** — *The Practice of the Presence of God*.
- **Lorenzo Scupoli** — *The Spiritual Combat*.
- **Jean-Pierre de Caussade** — *Abandonment to Divine Providence*.
- **Butler**, *Lives of the Saints*; **Catholic Encyclopedia (1913)** — reference (PD);
  **G. K. Chesterton** — *Orthodoxy* (1908), *The Everlasting Man* (1925), *St. Francis* ⚠(post-1930 titles not yet US-PD).

### F. Orthodox (PD)
- **NPNF Series 2** covers Athanasius, Basil, the Gregories, Chrysostom, John of Damascus (PD).
- **The Philokalia — Greek 1782** — **[HAVE]**.
- ***The Way of a Pilgrim*** (⚠ verify translation; R. M. French 1930-ish).
- **Dostoevsky** — *The Brothers Karamazov*, etc. (Constance Garnett translations, PD).

### G. Evangelical & revival (18th–19th c., all PD)
- **John Wesley** — *Works*, *Sermons*, *Journal*, *A Plain Account of Christian Perfection*.
- **George Whitefield** — *Sermons*, *Journals*. **Charles Wesley** — hymns.
- ★ **Charles Spurgeon** — *The Metropolitan Tabernacle Pulpit* (thousands of sermons);
  *The Treasury of David*; *Morning and Evening*; *Lectures to My Students*; *All of Grace*;
  *John Ploughman's Talk*.
- **J. C. Ryle** — *Holiness*; *Expository Thoughts on the Gospels*; *Practical Religion*.
- **Andrew Murray** — *Abide in Christ*, *Humility*, *With Christ in the School of Prayer*.
- **E. M. Bounds** — *Power Through Prayer* and the prayer series.
- **Charles Finney** — *Lectures on Revivals*; **D. L. Moody**; **A. B. Simpson**; **Horatius
  Bonar**; **Robert Murray M'Cheyne**; **Octavius Winslow**; **Hannah Whitall Smith** —
  *The Christian's Secret of a Happy Life*.
- **George MacDonald** — *Unspoken Sermons*; *Diary of an Old Soul*.

### H. Commentaries & reference (PD)
- **Matthew Henry**, *Complete Commentary*; **John Gill**, *Exposition*; **Adam Clarke**,
  *Commentary*; **Matthew Poole**, *Annotations*; **Jamieson-Fausset-Brown**; **Barnes' Notes**;
  **Calvin's Commentaries** (above); **Strong's** & **Thayer's**/**BDB** lexicons (PD eds.);
  **Cruden's Concordance**; **Smith's / Easton's Bible Dictionary**; **Josephus** (Whiston);
  **Eusebius**, *Church History*.

### I. Self-improvement / character / "success" (mostly 1890–1930, PD)
- **James Allen** — *As a Man Thinketh* **[HAVE]**; *Eight Pillars of Prosperity*; *From
  Poverty to Power*; *The Mastery of Destiny*; *Above Life's Turmoil*; *The Way of Peace*.
- **Wallace D. Wattles** — *The Science of Getting Rich* (1910); *Science of Being Great*;
  *Science of Being Well*.
- **Orison Swett Marden** — *Pushing to the Front*; *He Can Who Thinks He Can*.
- **Charles F. Haanel** — *The Master Key System* (1912).
- **Napoleon Hill** — *The Law of Success* (1928, PD). ⚠ *Think and Grow Rich* (1937) is NOT
  yet PD (US: 2033).
- **Florence Scovel Shinn** — *The Game of Life* (1925). **"Three Initiates"** — *The Kybalion*
  (1908). **Russell Conwell** — *Acres of Diamonds*. **Elbert Hubbard** — *A Message to Garcia*.
  **Ralph Waldo Trine** — *In Tune with the Infinite*.
- **Samuel Smiles** — *Self-Help*; *Character*; *Thrift*; *Duty*.
- **Ralph Waldo Emerson** — *Essays* (*Self-Reliance*, *Compensation*).
- **Benjamin Franklin** — *Autobiography*; *The Way to Wealth*.
- **William James** — *The Varieties of Religious Experience*; *The Principles of Psychology*.
- **Stoics:** Marcus Aurelius, *Meditations* (Long/Farquharson PD); Epictetus, *Enchiridion* &
  *Discourses* (Long); Seneca, *Letters* & *On the Shortness of Life*.

### J. Business, economics & strategy (PD)
- **Adam Smith** — *The Wealth of Nations*; *The Theory of Moral Sentiments*.
- **Andrew Carnegie** — *The Gospel of Wealth*; *Autobiography*. **P. T. Barnum** — *The Art
  of Money-Getting*. **Napoleon Hill** — *The Law of Success* (1928).
- **Sun Tzu** — *The Art of War* (Lionel Giles, 1910). **Machiavelli** — *The Prince* (PD).
- **John Stuart Mill** — *Principles of Political Economy*; *On Liberty*. **David Ricardo** —
  *Principles of Political Economy and Taxation*. **Alfred Marshall** — *Principles of
  Economics* (1890). **Thorstein Veblen** — *The Theory of the Leisure Class*.
- **Benjamin Franklin** — *Poor Richard's Almanack*. **Aesop** — *Fables* (leadership/wisdom).

---

### K. World religions & comparative texts (apologetics, PD)
For comparative/apologetics work — English public-domain primary texts, chiefly from **Max
Müller's *Sacred Books of the East*** (50 vols, 1879–1910) via sacred-texts.com / archive.org.
- **Islam:** Qur'an — Sale (1734), Rodwell (1861), Palmer (1880, SBE), Muhammad Ali (1917);
  ⚠ Pickthall 1930 now US-PD, Yusuf Ali 1934 not PD; hadith mostly copyrighted.
- **Hinduism:** *Bhagavad Gita* (Arnold; Telang), *Upanishads* (Müller; Hume 1921), *Rig Veda*
  (Griffith), *Ramayana* (Griffith), *Mahabharata* (Ganguli/Roy), *Laws of Manu* (Bühler),
  *Vishnu Purana* (Wilson), *Yoga Sutras / Raja Yoga* (Vivekananda).
- **Buddhism:** *Dhammapada* (Müller), *Buddhist Suttas* (Rhys Davids), *Jataka* (Cowell),
  *Questions of King Milinda*, *Lotus Sutra* (Kern), *Buddhism in Translations* (Warren),
  *Gospel of Buddha* (Carus), *Life of Buddha* (Cowell), *Tibetan Book of the Dead* (1927).
- **Breadth:** Confucian *Analects*/*Mencius* & *Tao Te Ching* (Legge); Zoroastrian *Avesta*;
  *Book of Mormon* (1830). Captured under `world-religions/<tradition>/`.

## Proposed phased capture (each phase = its own commit + SOURCES/CHECKSUMS update)

1. **Christian core, Puritan/Reformed** ★ — Owen, Baxter, Bunyan, Watson, Sibbes, Charnock,
   Burroughs, Gurnall, Flavel, Brooks (complete), Calvin *Institutes*, Westminster standards,
   Foxe. (Mostly CCEL/Gutenberg text — fast.)
2. **Evangelical/revival** — Spurgeon (sermons + *Treasury of David*), Ryle, Murray, Bounds,
   MacDonald, Wesley, Whitefield. (Spurgeon is large — likely LFS for sermon corpora.)
3. **Bibles & reference** — PD English Bibles + original-language texts; Matthew Henry, Gill,
   Clarke, Strong's, Josephus, Eusebius, Schaff history.
4. **Catholic & Orthodox devotional** — de Sales, Teresa, John of the Cross, Scupoli,
   Caussade, Brother Lawrence, à Kempis (have), *Way of a Pilgrim*; Catholic Encyclopedia 1913.
5. **Self-improvement** — Allen (complete), Wattles, Marden, Haanel, Hill *Law of Success*,
   Shinn, Conwell, Smiles, Emerson, Franklin, James, the Stoics.
6. **Business/economics** — Smith, Carnegie, Barnum, Sun Tzu, Machiavelli, Mill, Ricardo,
   Marshall, Veblen.
7. **Complete the ANF/NPNF set** and remaining medieval/mystical.

**Scale/storage:** text-first keeps most of this small and grep-able; only large scan sets
(Spurgeon's collected sermons, Calvin's 45-vol commentaries as scans, folio Puritan works)
need Git LFS. A reasonable full build is on the order of a few GB — trivial for local disk,
and the whole point is that it lives on *your* drive, checksummed, forever.

---

_This roadmap is a living document. As phases are captured, their rows move into `SOURCES.md`
and their files into `CHECKSUMS.sha256`._
