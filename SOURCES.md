# Sources

Captured 2026-07-21; expanded 2026-07-22 (Phase A acquisition, Priorities 1-5).

> **Externalized scans (2026-07-23):** the large image-scan PDFs listed below (Philokalia
> 1782, Climacus PG 88, Budge vols 1-2, Brooks scans) were **moved out of this git repo** to
> keep it pure text. They now live at `D:\repos\scans\<same relative path>` — not in git,
> backed up by the Axcient BDR (local + cloud), integrity verifiable via
> `D:\repos\scans\CHECKSUMS.sha256`. The `raw/.../*.pdf` paths in the rows below describe the
> mirrored location under `D:\repos\scans`. All quotable material is the clean text captures.

| Collection | Source URL | Local material | Edition and reuse note |
|---|---|---|---|
| Cassian, *Institutes* I-V, VII-XII | https://www.newadvent.org/fathers/3507.htm | `patristics/john-cassian/raw/new-advent/` | C. S. Gibson, NPNF 2.11 (1894), public-domain translation. Saved page presentation belongs to its host. Book VI was omitted by the NPNF editors (captured separately via Dysinger, below). Books I-IV added 2026-07-22. |
| Cassian, *Conferences* I-XI, XIII-XXI, XXIII-XXIV | https://www.newadvent.org/fathers/3508.htm | `patristics/john-cassian/raw/new-advent/` | C. S. Gibson, NPNF 2.11 (1894), public-domain translation. Complete NPNF set. Conferences XII and XXII are **absent** from the NPNF/Gibson translation (verified 2026-07-22: `3508 12`/`3508 22` redirect to the New Advent home page); see the Latin *Collationes* row for those two. Conferences III, IV, VI-XI, XIII-XXI, XXIII-XXIV added 2026-07-22. |
| Cassian, complete Latin text | https://la.wikisource.org/wiki/De_coenobiorum_institutis | `patristics/john-cassian/raw/wikisource/` | Wikisource identifies Migne, PL 49 (1846), derived from Corpus Corporum TEI. Page content is CC BY-SA; underlying ancient/1846 text is public domain. |
| Cassian, *Institutes* VI | https://www.ldysinger.com/%40texts/0415_cassian/02_inst-06.htm | `patristics/john-cassian/raw/dysinger/` | Latin with a modern English reading text based on Kardong and Bertram. Use for research; verify reuse rights before quoting the modern wording. |
| Evagrius, *Praktikos* | https://evagriusponticus.net/cpg2430/cpg2430.eng.1990.dysinger.html | `patristics/evagrius-ponticus/raw/praktikos/` | Luke Dysinger English translation; source metadata calls the translation public domain and the TAN transcription CC BY 4.0. |
| Evagrius, *Antirrhetikos* parallel page | https://evagriusponticus.net/cpg2434/cpg2434-full-for-search.html | `patristics/evagrius-ponticus/raw/antirrhetikos/antirrhetikos-parallel.html` | Search convenience showing aligned witnesses. |
| Evagrius, *Antirrhetikos* Syriac | https://raw.githubusercontent.com/Arithmeticus/TAN-Evagrius/master/cpg2434/cpg2434.syr.1912.frankenberg.tei.xml | `patristics/evagrius-ponticus/raw/antirrhetikos/antirrhetikos-frankenberg-syriac.xml` | Frankenberg 1912 Syriac transcription; TAN metadata identifies CC BY 4.0. |
| Evagrius, *Antirrhetikos* Greek retroversion | https://raw.githubusercontent.com/Arithmeticus/TAN-Evagrius/master/cpg2434/cpg2434.grc.1912.frankenberg.tei.xml | `patristics/evagrius-ponticus/raw/antirrhetikos/antirrhetikos-frankenberg-greek-retroversion.xml` | Reconstruction from Syriac, not a surviving complete Greek original; TAN metadata identifies CC BY 4.0. |
| Evagrius, *Antirrhetikos* Serbian | http://evagriusponticus.net/tan/cpg2434/cpg2434.srp.2023.nesic.xml | `patristics/evagrius-ponticus/raw/antirrhetikos/antirrhetikos-nesic-serbian.xml` | Lazar Nesic modern Serbian translation; consult embedded TAN metadata and attribution requirements. |

## Added 2026-07-22 (Phase A)

| Collection | Source URL | Local material | Edition and reuse note |
|---|---|---|---|
| Cassian, complete Latin *Collationes* (Conferences I-XXIV, incl. XII & XXII, + 3 part-prefaces + index) | https://la.wikisource.org/wiki/Collationes | `patristics/john-cassian/raw/wikisource/collationes/` | Wikisource text of the Migne/Corpus Corporum Latin *Collationes*, one page per collatio. Page content is CC BY-SA; underlying ancient/Migne Latin is public domain. This is the **only** witness in the vault for Conferences XII and XXII (absent from the NPNF English). Raw-only; no reading copy generated this pass. |
| Evagrius, *Peri Logismon* / On Thoughts (CPG 2450) — critical & parallel witnesses | https://evagriusponticus.net/corpus.htm (cpg2450/) | `patristics/evagrius-ponticus/raw/peri-logismon/cpg2450*.html` | evagriusponticus.net (TAN) collated parallel editions plus Greek transcriptions (Géhin 1998; PG 1858/1863) and Nesic Serbian 2023. Consult embedded TAN/CC metadata per file. No English translation is hosted here. |
| Evagrius, *Peri Logismon* / On Thoughts — Dysinger English | http://www.ldysinger.com/Evagrius/04_Peri-Log/01_p-log_all.htm | `patristics/evagrius-ponticus/raw/peri-logismon/peri-logismon-dysinger-*.html` | Luke Dysinger O.S.B. English translation with parallel Greek (page notes the translation is partly based on Palmer/Kadloubovsky and the Greek on Migne/Philokalia/Muyldermans, superseded by Guillaumont's critical edition). Research use; **verify before print quotation**. Also captured: the SC Greek text page and a spiritual-direction cross-reference page. |
| Evagrius, *De oratione* / Chapters on Prayer (CPG 2452) — critical & parallel witnesses | https://evagriusponticus.net/corpus.htm (cpg2452/) | `patristics/evagrius-ponticus/raw/de-oratione/cpg2452*.html` | evagriusponticus.net (TAN) collated parallel editions plus Greek (Géhin 2017; PG 1863) and Latin (PG 1863) transcriptions and Nesic Serbian 2023. Consult embedded TAN/CC metadata per file. No English translation is hosted here. |
| Evagrius, *De oratione* / On Prayer — Dysinger English | http://www.ldysinger.com/Evagrius/03_Prayer/01_prayer_all.htm | `patristics/evagrius-ponticus/raw/de-oratione/de-oratione-dysinger-*.html` | Luke Dysinger O.S.B. English translation with parallel Greek; page states "translation in public domain" and the Greek is based on PG 79.1165-1200, the Philokalia, and Tugwell, updated per Géhin (SC 589). Research use; verify before print quotation. |
| Athanasius, *Life of Antony* | https://www.newadvent.org/fathers/2811.htm | `patristics/athanasius/raw/new-advent/life-of-antony.html` | Translated by H. Ellershaw, NPNF Second Series, Vol. 4 (1892), public domain. Saved page presentation belongs to its host. |
| Chrysostom, *No One Can Harm the Man Who Does Not Injure Himself* | https://www.newadvent.org/fathers/1902.htm | `patristics/john-chrysostom/raw/new-advent/no-one-can-harm.html` | Translated by W. R. W. Stephens, NPNF First Series, Vol. 9 (1889), public domain. |
| Chrysostom, *Homilies on the Statues* (complete: 21 homilies + index) | https://www.newadvent.org/fathers/1901.htm | `patristics/john-chrysostom/raw/new-advent/statues-homily-01..21.html`, `statues-index.html` | NPNF First Series, Vol. 9 (1889), public domain. Complete set captured (no editorial selection made). |
| James Allen, *As a Man Thinketh* (1903) | https://www.gutenberg.org/ebooks/4507 | `tradition/james-allen/raw/gutenberg/as-a-man-thinketh-allen-pg4507.txt` | Project Gutenberg eBook #4507; public domain. |
| Augustine, *Confessions* (Pusey translation) | https://www.gutenberg.org/ebooks/3296 | `patristics/augustine/raw/gutenberg/confessions-pusey-pg3296.txt` | Translated by E. B. Pusey; Project Gutenberg eBook #3296; public domain. |
| Thomas à Kempis, *The Imitation of Christ* | https://www.gutenberg.org/ebooks/1653 | `tradition/thomas-a-kempis/raw/gutenberg/imitation-of-christ-benham-pg1653.txt` | Translated by William Benham; Project Gutenberg eBook #1653; public domain. |
| John Owen, *The Mortification of Sin in Believers* (1656) | https://ccel.org/ccel/owen/mort/mort | `tradition/john-owen/raw/ccel/mortification-of-sin-ccel-mort.txt` | CCEL plain-text export; transcription print basis The Banner of Truth Trust, Edinburgh, 1967. Underlying 1656 text public domain; **verify wording before quoting** the modern typesetting. |
| John Owen, *Of Temptation* (1658) | https://ccel.org/ccel/owen/temptation/temptation | `tradition/john-owen/raw/ccel/of-temptation-ccel-temptation.txt` | CCEL plain-text export; underlying 1658 text public domain; verify wording before quoting. |
| Thomas Brooks, *Precious Remedies Against Satan's Devices* (1652) — original-edition scan | https://archive.org/details/preciousremedies00broo | `tradition/thomas-brooks/raw/archive-org/precious-remedies-against-satans-devices-1832-newhaven-archive.pdf` | Nathan Whiting, New Haven (1832) reprint of the public-domain 1652 text; authoritative scanned witness. |
| Thomas Brooks, *Precious Remedies* — modern typeset reading PDF | https://www.preachtheword.com/bookstore/remedies.pdf | `tradition/thomas-brooks/raw/preachtheword/precious-remedies-against-satans-devices-preachtheword.pdf` | Full modern typeset PDF (~160 pp), easier to read than the scan. Not on CCEL (listed "Wanted") or Gutenberg. Underlying 1652 text public domain; this typesetting is **verify-before-quoting** (check against the archive.org scan above). Raw-only (PDF). |
| Budge, *The Paradise (or Garden) of the Holy Fathers* (1907), vols. 1-2 | https://archive.org/details/ParadiseOfTheHolyFathersV1 , https://archive.org/details/ParadiseOfTheHolyFathersV2 | `patristics/apophthegmata/raw/archive-org/budge-paradise-of-the-holy-fathers-1907-vol1.pdf`, `...-vol2.pdf` | E. A. Wallis Budge, translated from the Syriac; London: Chatto & Windus, 1907; public domain. Searchable `_text.pdf` scans (OCR text layer over page images). Archive item identifiers: `ParadiseOfTheHolyFathersV1` / `V2`. Raw-only (PDF). |
| John Climacus, *Ladder of Divine Ascent* / *Scala Paradisi* — Greek base text | https://www.documentacatholicaomnia.eu/04z/z_0525-0606__Joannes_Climacus__Scala_Paradisi_(MPG_088_0631_1163)__GM.pdf.html | `patristics/john-climacus/raw/documenta-catholica-omnia/scala-paradisi-greek-migne-pg88-0631-1163.pdf` | Migne, Patrologia Graeca 88, cols 631-1163 (Rader's Greek, 1860), public domain. Captured as a **base text** because no public-domain English translation exists (Moore 1959 and Luibheid/Russell 1982 are copyrighted — English access is research-only). Raw-only (image PDF, ~70 MB). |
| The *Philokalia of the Neptic Fathers* (Φιλοκαλία τῶν ἱερῶν νηπτικῶν) — Greek base text, 1782 Venice first edition | https://commons.wikimedia.org/wiki/File:%CE%A6%CE%99%CE%9B%CE%9F%CE%9A%CE%91%CE%9B%CE%99%CE%91_%CE%A4%CE%A9%CE%9D_%CE%99%CE%95%CE%A1%CE%A9%CE%9D_%CE%9D%CE%97%CE%A0%CE%A4%CE%99%CE%9A%CE%A9%CE%9D.pdf | `patristics/philokalia/raw/wikimedia/philokalia-ton-hieron-neptikon-1782-venice-wikimedia.pdf` | The original Greek anthology compiled by Nikodimos the Hagiorite and Makarios of Corinth, Venice 1782; public domain. Full-resolution scan hosted on Wikimedia Commons. Captured as a **Greek base text**; the modern English (Palmer/Sherrard/Ware, Faber) is copyrighted and is NOT captured. Raw-only (image PDF, ~193 MB; stored via Git LFS). |

## Added 2026-07-23 (pre-Nicene / Nicene public-domain expansion)

Roots and parallels for the eight-thoughts / spiritual-combat tradition. All public
domain (ANF = Ante-Nicene Fathers, Roberts-Donaldson 1885; NPNF = Nicene and
Post-Nicene Fathers). New Advent page presentation belongs to its host.

| Collection | Source | Local material | Edition and reuse note |
|---|---|---|---|
| Apostolic Fathers — *Shepherd of Hermas* (Visions/Commands/Similitudes), *Didache*, *Epistle of Barnabas* | New Advent /fathers/02011-02013, 0714, 0124 | `patristics/apostolic-fathers/raw/new-advent/` + reading | ANF Vol. 1-2, public domain. Hermas = proto-discernment-of-thoughts. |
| Clement of Alexandria — *The Instructor (Paedagogus)*, Books I-III | New Advent /fathers/02091-02093 | `patristics/clement-of-alexandria/raw/new-advent/` + reading | Trans. William Wilson, ANF Vol. 2 (1885), public domain. On the bodily passions. |
| Tertullian — *Of Patience*, *On Repentance*, *On Prayer*, *On Fasting*, *On Modesty* | New Advent /fathers/0325, 0320, 0322, 0408, 0407 | `patristics/tertullian/raw/new-advent/` + reading | ANF Vol. 3-4, public domain. |
| Cyprian — *On the Lord's Prayer* (Tr. 4), *On Works and Alms* (Tr. 8), *On Jealousy and Envy* (Tr. 10) | New Advent /fathers/050704, 050708, 050710 | `patristics/cyprian/raw/new-advent/` + reading | ANF Vol. 5, public domain. |
| Lactantius — *On the Anger of God* | New Advent /fathers/0703 | `patristics/lactantius/raw/new-advent/` + reading | ANF Vol. 7, public domain. |
| Methodius — *The Banquet of the Ten Virgins* (Introduction + 11 Discourses) | New Advent /fathers/062300-062311 | `patristics/methodius/raw/new-advent/` + reading | ANF Vol. 6, public domain. On chastity. |
| Gregory of Nyssa — *On Virginity* | New Advent /fathers/2907 | `patristics/gregory-of-nyssa/raw/new-advent/` + reading | NPNF 2.5, public domain. |
| Ambrose — *Concerning Repentance*, Books I-II | New Advent /fathers/34061-34062 | `patristics/ambrose/raw/new-advent/` + reading | NPNF 2.10, public domain. |
| Origen — *On Prayer* | https://ccel.org/ccel/origen/prayer/prayer | `patristics/origen/raw/ccel/on-prayer-curtis-ccel.txt` + reading | Trans. William A. Curtis; CCEL plain-text; public domain. (On Prayer is not in ANF.) |
| Gregory the Great — *Moralia in Job* (Morals on the Book of Job), Books I-XXXV | https://www.lectionarycentral.com/gregorymoraliaindex.html | `patristics/gregory-the-great/raw/lectionarycentral/` | *Library of the Fathers* translation (Bliss/Marriott, Oxford, 1844-50), public domain. The bridge text from Cassian's eight thoughts to the Western seven deadly sins (Book XXXI). Raw-only this pass (Word-exported HTML; searchable; reading copies deferred). |

## Added 2026-07-23 (Jewish / Second-Temple world — "what did the Jews know")

All public-domain English text (no scans). Division: `jewish/`.

| Collection | Source | Local material | Edition / rights |
|---|---|---|---|
| Josephus — *Antiquities*, *Wars*, *Against Apion*, *Life* | Project Gutenberg #2848/2850/2849/2846 | `jewish/josephus/` | William Whiston translation (1737); public domain |
| Philo of Alexandria — *The Works of Philo Judaeus* | CCEL | `jewish/philo/` | C. D. Yonge translation (1854); public domain |
| The Apocrypha (Deuterocanon) | Project Gutenberg #124 | `jewish/apocrypha/` | KJV 1611; public domain |
| Alfred Edersheim — *Life and Times of Jesus the Messiah*, *Sketches of Jewish Social Life*, *The Temple* | CCEL | `jewish/edersheim/` | public domain (Edersheim d. 1889) |
| Pseudepigrapha — *The Book of Enoch*; Charles's *Apocrypha & Pseudepigrapha* vol. 2 | sacred-texts.com; archive.org (Charles, Oxford 1913) | `jewish/pseudepigrapha/` | public domain; the APOT vol. 2 file is archive.org **OCR — verify before quoting** |
| The Targums of Onkelos & Jonathan (Pentateuch) | archive.org (Etheridge 1862) | `jewish/targums/` | public domain; archive.org **OCR — verify before quoting** |

## Gaps and research-only (2026-07-22)

- **Chrysostom, *On Vainglory and the Right Way to Bring Up Children*** (Priority 5) — NOT captured. The work is *absent from Migne's Patrology*; its Greek survives only in the copyrighted Malingrey critical edition (Sources Chrétiennes 188), and the standard English (Laistner 1951) is copyrighted. No public-domain witness exists to capture. Recorded gap.
- **The Philokalia — English** (Priority 5) — the Palmer/Sherrard/Ware (Faber) English translation is copyrighted and is NOT captured; research-only. The public-domain **Greek** 1782 first edition WAS captured as a base text (see the Philokalia row above).
- **John Climacus, English translation** — no public-domain English exists; the Greek PG 88 base text was captured instead (above). English wording must come from a future working translation or a rights-checked source.
- **Jewish phase — deferred items** (2026-07-23): the **Rodkinson Babylonian Talmud** (public
  domain, but only as ~124 messy multi-edition archive.org OCR scans or the rate-limited
  sacred-texts text — needs a dedicated careful pass, not a quick grab); **Edersheim's *Bible
  History: Old Testament*** (not on CCEL; get from Gutenberg/archive later); **Schürer's
  *History of the Jewish People*** and the **Jewish Encyclopedia (1901–06)** (archive.org /
  jewishencyclopedia.com — the latter a large structured reference for a scoped pass). All PD.
- **Basil of Caesarea — homilies *Against Anger*, *On Envy*, *On Humility*, *On Fasting*** (2026-07-23) — NOT captured. These per-passion homilies survive in English only in copyrighted modern translations (Fathers of the Church, *Ascetical Works* / *On Social Justice*); NPNF 2.8 Basil contains the Hexaemeron, *On the Spirit*, and Letters, but not these homilies. No public-domain English witness found. Recorded gap.
