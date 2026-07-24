# From demons to disorders — the disenchantment of the tormenting thought

**Research question.** Two prior briefs already cover the wider ground either side of this one:
`research/2026-07-24_sin-as-sickness.md` traces the *medical model of the soul* in general (physician,
patient, disease, cure — a frame the tradition itself supplied); `research/2026-07-24_spiritual-warfare.md`
traces the *bifurcation* of the whole demonic worldview into a living deliverance literature and a
secular-dismissal literature. This brief is narrower than both, and is their capstone: it isolates one
specific pair of questions and asks how the tradition's answer to them was replaced rather than merely
supplemented. **Etiology** — when a thought arrives unbidden, tormenting, and will not leave, where does
it come from: a spirit outside the sufferer, or a malfunction inside him? **Remedy** — is it met with
Scripture, prayer, and the will (answered), or with medication and cognitive technique (corrected)? The
tradition that gave ChainBreaker its eight *logismoi* answered both questions the same way for over a
thousand years: the thought is the demon's weapon, and it is defeated by talking back to it with the
Word. Modernity's sharpest single pivot — sharper than "sickness" language in general, because it is a
flat *rejection* rather than a re-description — is the move that follows: the thought's origin is
relocated from outside the sufferer to a broken brain or a distorted cognition inside him, and the
remedy relocates with it, from Scripture to the prescription pad and the thought-record.

**A caveat that governs everything below, stated once, in its own paragraph, so it need not be
repeated at every turn.** This is *not* the claim that mental illness is "just demons" or "just sin,"
that psychiatric treatment or medication should be refused, or that any named diagnosis is a euphemism
for a vice or a cover for insufficient faith. Real biological and psychiatric illness exists;
medication and evidence-based therapy relieve real suffering and save real lives; nothing below maps
a diagnosis onto a demon or a diagnosis onto a person's culpability. Thomas Szasz's claim that "mental
illness" is a myth is presented below strictly as *his own historical argument* — used for the narrower
and more defensible point that the diagnostic *category* was over-extended into moral and existential
territory it did not fit — not endorsed as a blanket denial of psychiatric suffering; Jay Adams's
nouthetic counseling is likewise presented descriptively, together with the standard and largely
accepted critique that early nouthetic counseling under-weighted genuine biological illness, a
correction the later biblical-counseling movement (associated with David Powlison, not present in this
vault and therefore not quoted) is generally credited with supplying. The honest ChainBreaker position
is a **both/and**, argued in its own dedicated section below: the modern relocation gained real things
(treatment, compassion, the de-stigmatization of the genuinely ill) and lost a real thing (the category
of a thought that arrives from beyond the will and can be *answered*, not only medicated) — and the
book's payoff does not require choosing a metaphysics to reclaim the practice.

**Method.** Corpus-wide `grep -rniE` and targeted reading across `D:\repos\books\**\*.md`. This brief
does not re-run the word-count method already reported in full in the sin-as-sickness brief (the DSM-5's
zero operative uses of "sin"/"repent," one third-person use of "God," two third-person uses of "soul,"
against 12,800+ uses of "disorder") or the spiritual-warfare brief's targeted DSM check (no clean match
for "spirit possession," no operative diagnostic use of "demon"); both findings are load-bearing for
this brief and are cited by reference rather than repeated. What is new here is a line-level reading of
the DSM-5's actual **Obsessive-Compulsive Disorder** criteria (`reference/dsm-5/reading/dsm-5.md:1107-1131`)
against Evagrius's *Antirrhetikos*, and a first close reading, for this specific etiology/remedy
question, of three sources none of the other two briefs use in depth: **Thomas Szasz, *The Myth of
Mental Illness*** (grep `myth|metaphor|problems in living|moral|responsibility`, `self-improvement/the-myth-of-mental-illness/reading/the-myth-of-mental-illness.md`),
**Jay Adams, *Competent to Counsel*** (grep `nouthetic|medical model|Holy Spirit|responsibility`,
`tradition/competent-to-counsel/reading/competent-to-counsel.md`), and **Aaron Beck, *Cognitive Therapy
and the Emotional Disorders*** read specifically for its etiology claim (where the thought's *cause* is
located), not only its title's reclassification (already the sin-as-sickness brief's point).

Owned-copyright and OCR-sourced texts are quoted **short (a sentence or two), for commentary, cited
`path:line`, verified verbatim before use** — never approximated. OCR flags: the **DSM-5** (APA 2013,
Internet Archive OCR, owned copyright) carries an explicit OCR-verify warning in its file header;
every quotation from it below was checked against the surrounding paragraph, including the full
diagnostic-criteria block reproduced at `dsm-5.md:1115`. Szasz's *Myth of Mental Illness* (1961/1974,
IA EPUB, owned copyright) and Adams's *Competent to Counsel* (1970, EPUB, owned copyright) are
owned-copyright but **clean** extractions, not OCR — both carry the standard "owned copyright, personal
use, do not distribute" header rather than an OCR warning, and both were spot-checked regardless.
Evagrius's *Talking Back*, Athanasius, and Cassian reuse citations already verified in the
spiritual-warfare brief; they are not re-verified here but are re-quoted at the same `path:line`.

---

## The arc

### 0. The sharp modern case first — OCD is the tradition's own terrain, reclassified
Before tracing the arc chronologically, it is worth putting the two endpoints side by side, because
the continuity of *phenomenology* across the whole discontinuity of *etiology* is this brief's central
finding and is easiest to see in one comparison. Evagrius describes a thought that is not simply had,
but *arrives* and *speaks*:

> "Against the thought that says to me…" — the heading repeated, with a different content, at the
> start of every single entry in *Talking Back* (`patristics/talking-back-antirrhetikos/reading/talking-back-antirrhetikos.md:508`
> and following).

The DSM-5's Criterion A for Obsessive-Compulsive Disorder describes, in its own clinical register, what
reads as the identical phenomenon:

> "Recurrent and persistent thoughts, urges, or images that are experienced, at some time during the
> disturbance, as intrusive and unwanted, and that in most individuals cause marked anxiety or
> distress." (`reference/dsm-5/reading/dsm-5.md:1115`)

Both texts describe a thought that the sufferer did not invite, that repeats, that causes distress, and
that the sufferer "attempts to ignore or suppress... or to neutralize... with some other thought or
action" (`dsm-5.md:1115`, Criterion A.2) — which is, structurally, exactly Evagrius's antirrhesis:
meet the thought with a counter-thought or counter-action. What has changed entirely is *where the DSM
says the thought comes from* and *what it prescribes in response*. Criterion C states the origin
question in the negative — the symptoms must not be "attributable to the physiological effects of a
substance... or another medical condition" (`dsm-5.md:1115`) — and the manual's entire vocabulary of
causation from that point forward is temperamental, environmental, and "genetic and physiological"
(`dsm-5.md:1123`, citing orbitofrontal-cortex and striatal dysfunction and twin-concordance rates). No
clause anywhere in the criteria considers, and no clause needs to exclude, a spirit. The category is not
denied a hearing; it is simply not a category the taxonomy has room to pose (a point the
spiritual-warfare brief's targeted grep already establishes for "demon" and "spirit possession" across
the whole manual). This is the pivot this brief is about: not sickness-language displacing sin-language
in general (the sin-as-sickness brief's broader claim), but the *external* origin of a specific,
addressable, tormenting thought being replaced by an *internal* one, with no remainder.

### 1. The old etiology — the thought is the demon's weapon, answered by the Word
The desert tradition's claim is not that thoughts are sometimes demonic; it is that the eight thoughts
*are*, categorically, the demons' means of attack, and Scripture is the prescribed counter-force. This
ground is covered in full by the spiritual-warfare brief; three citations carry the weight needed here.

**Athanasius, *Life of Antony*** gives Antony's own summary of the mechanism in one sentence:
> "The demons, therefore, if they see all Christians, and monks especially, labouring cheerfully and
> advancing, first make an attack by temptation and place hindrances to hamper our way, to wit, evil
> thoughts." (`patristics/athanasius/reading/life-of-antony.md:73`)

**Cassian, *Conference* 8** states the general rule connecting demonic entry to the state of the mind —
guarding the mind is not incidental self-help but the thing that keeps the door shut:
> "Demons cannot possibly find an entrance into the mind or body of anyone, nor have they the power of
> overwhelming the soul of anyone, unless they have first deprived it of all holy thoughts, and made it
> empty and free from spiritual meditation." (`patristics/john-cassian/reading/conference-08.md:123`)

**Evagrius, *Talking Back*** supplies both the etiology and the remedy in the same short passage, which
is why this book is the desert's most direct answer to this brief's two questions at once: the thought
comes from a demon, and Scripture — not silence, not resignation, not analysis — is the prescribed
counter-force:
> "In the time of struggle, when the demons make war against us and hurl their arrows at us, let us
> answer them from the Holy Scriptures, lest the unclean thoughts persist in us."
> (`patristics/talking-back-antirrhetikos/reading/talking-back-antirrhetikos.md:478`)
> "For us the entire struggle will take place through the thoughts that approach us from each of these
> eight demons. But I have written and quoted for each of the thoughts an answer from the Holy
> Scriptures that is able to cut it off." (`talking-back-antirrhetikos.md:486`)

Note precisely what this etiology accomplishes for the sufferer, whatever else it does or does not
explain: it locates the origin of the torment *outside* the person having it. The monk is not, in this
picture, a malfunctioning instrument; he is a combatant under attack, and the thought — however
humiliating its content — is not proof of his own brokenness but evidence of an assault to be repelled.
(Cassian's Conference 7 companion doctrine that "no one can be deceived by the devil but one who has
chosen to yield to him the consent of his own will," `conference-07.md:57`, keeps this from becoming an
excuse — the demon proposes, the will still disposes — but the *origin* of the thought itself remains
external.)

### 2. The relocation inward — Beck: the cause is now in the patient's own consciousness
**Aaron T. Beck, M.D.**, *Cognitive Therapy and the Emotional Disorders* (1976), states the etiological
claim directly, and states it as a *rejection* of the very idea of forces acting on the sufferer from
beyond his own awareness — first naming what the older schools (not the desert, but neuropsychiatry,
psychoanalysis, behaviorism) still shared with the demonic picture, structurally, before replacing it:
> "The emotionally disturbed person is victimized by concealed forces over which he has no control."
> (`self-improvement/cognitive-therapy-and-the-emotional-disorders/reading/cognitive-therapy-and-the-emotional-disorders.md:97`,
> describing neuropsychiatry, psychoanalysis, and behavior therapy alike)

Beck's innovation is to relocate the cause a second time — not to a demon, not to the unconscious, not
to a conditioned reflex, but into the patient's own ordinary, conscious, correctable thinking:
> "Man has the key to understanding and solving his psychological disturbance within the scope of his
> own awareness. He can correct the misconceptions producing his emotional disturbance with the same
> problem-solving apparatus that he has been accustomed to using."
> (`cognitive-therapy-and-the-emotional-disorders.md:101`)
> "The therapist helps a patient to unravel his distortions in thinking and to learn alternative, more
> realistic ways to formulate his experiences." (`cognitive-therapy-and-the-emotional-disorders.md:103`)

This is the remedy question answered in the same stroke as the etiology question: no Scripture, no
demon, no prayer — reality-testing, performed by the patient's own reason under a therapist's guidance.
Beck even notes, in passing, that the intrusive thought is *more* pronounced exactly where the tradition
would have named the *logismos* at its most acute: "the automatic thoughts were more compelling in the
ideation of obsessional patients" (`cognitive-therapy-and-the-emotional-disorders.md:303`) — the same
phenomenon Evagrius built an entire handbook to answer, now a data point about which patients report the
loudest internal monologue.

### 3. The DSM-5 — the catalogue completes the relocation without naming what it replaced
The DSM's OCD criteria (§0 above, `dsm-5.md:1115`) are the terminus of Beck's etiological move, codified
as diagnostic law rather than argued as clinical theory: intrusive, unwanted, distressing thoughts are,
by Criterion C, *specifically not* to be attributed to anything outside the body's own physiology or
another medical condition, and by Criterion D not better explained by any other named mental disorder —
the taxonomy exhaustively partitions the internal territory and asks nothing about the external one.
Both the sin-as-sickness brief (word counts across the whole 2013 manual) and the spiritual-warfare
brief (targeted grep for "demon" and "spirit possession") already establish that this is not an
oversight specific to the OCD chapter — it is the manual's operative vocabulary everywhere. This brief's
own contribution is narrower: reading the actual criteria language shows the replacement is not merely
an absence but a structured, positive claim about causation ("genetic and physiological,"
`dsm-5.md:1123`) sitting in the exact clause where the desert would have named an enemy.

### 4. The two-flank critique of the relocation — Szasz and Adams, from opposite ends, name the same shift
Neither of the two sharpest critics of the psychiatric relocation is a defender of the demonic etiology.
Both, from entirely different premises — one secular and skeptical of religion, one explicitly biblical
— argue that the *category* "mental illness" over-reached, displacing a moral-existential register with
a medical one that did not actually fit the facts. Read together, they show the critique of the
relocation is not confined to religious writers.

**Thomas Szasz, M.D.**, *The Myth of Mental Illness* (1961; rev. 1974), makes the etiology argument in
its starkest form: illness, properly speaking, is a fact about the body, and "mental illness" smuggles
in a category error by treating a metaphor as a literal diagnosis.
> "Strictly speaking, then, disease or illness can affect only the body. Hence, there can be no such
> thing as mental illness. The term 'mental illness' is a metaphor."
> (`self-improvement/the-myth-of-mental-illness/reading/the-myth-of-mental-illness.md:57`)

Szasz's positive alternative is not a return to the demonic — he is explicit that psychiatry's true
subject matter is moral and existential, not medical:
> "Individuals who nowadays seek private psychoanalytic or psychotherapeutic help do not, as a rule,
> consider themselves either 'sick' or 'mentally sick,' but rather view their difficulties as **problems
> in living** and the help they receive as a type of counseling."
> (`the-myth-of-mental-illness.md:65,69`)
> "I hold that psychiatric interventions are directed at moral, not medical[] problems... psychiatry is
> not a medical, but a moral and political, enterprise." (`the-myth-of-mental-illness.md:65,69`)

As stated in the caveat above, ChainBreaker uses this narrowly: Szasz is evidence that the etiological
relocation (thought-as-symptom-of-disease) was contested from *inside* the secular clinical
establishment, on grounds that have nothing to do with defending the demonic — not evidence that
psychiatric suffering is fictitious.

**Jay E. Adams**, *Competent to Counsel* (1970), makes the parallel argument from the opposite premise:
not that "mental illness" is a category error in general, but that Scripture, not psychiatry, correctly
diagnoses most of what psychiatry calls illness as sin requiring confrontation and repentance. Adams
narrates his own turn against the medical model directly, crediting the secular psychologist O. Hobart
Mowrer's critique before supplying his own biblical version of it:
> "Mowrer particularly opposed the Medical Model from which the concept of mental illness was derived.
> He showed how this model removed responsibility from the counselee... Mowrer rightly maintained that
> the Medical Model took away the sense of personal responsibility."
> (`tradition/competent-to-counsel/reading/competent-to-counsel.md:163`)
> "In contrast, Mowrer antithetically proposed a Moral Model of responsibility. He said that the
> 'patient's' problems are moral, not medical. He suffers from real guilt, not guilt feelings."
> (`competent-to-counsel.md:165`)

Adams's own conclusion, stated as a summary verdict rather than a qualified hypothesis, is the strongest
and most totalizing claim in this brief's entire source set:
> "There may be several things wrong with the so-called 'mentally ill,' but the one cause which must be
> excluded in most cases is mental illness itself." (`competent-to-counsel.md:455`)

Adams is careful to root the remedy in the person of the Holy Spirit working through Scripture, not in
technique alone: "Counseling is the work of the Holy Spirit. Effective counseling cannot be done apart
from him" (`competent-to-counsel.md:349`), and nouthetic confrontation is grounded exegetically in
Colossians 3:16 and Romans 15:14 (`competent-to-counsel.md:469-477`). This is Evagrius's remedy — the
Word applied directly to the sufferer's condition — transposed from monastic combat with a personal
demon into pastoral confrontation with sin, without the demonology but with the etiology (moral, not
medical) and the cure (Scripture, not psychiatry) both intact. As the caveat states, this is exactly the
place where the standard critique of early nouthetic counseling applies most directly: "the one cause
which must be excluded in most cases" (`competent-to-counsel.md:455`) is a claim that, taken as a
blanket rule rather than a corrective emphasis, under-weights genuine biological and psychiatric
illness — a correction the later biblical-counseling movement is generally credited with supplying,
moderating Adams's totalizing language into something closer to Cassian's own both/and (see “The balance” section below).

### 5. The bifurcation named from inside modern Christianity
The spiritual-warfare brief documents at length the modern split between literal deliverance ministry
and secular dismissal (`research/2026-07-24_spiritual-warfare.md` §3). This brief adds one further
witness specific to the etiology/remedy question: a single popular Christian book that stages the
"is it a demon or is it psychology" question *inside itself*, refusing to resolve it by picking a side.

**John Mark Comer**, *Live No Lies* (2021), names the ancient triad of enemies directly — "the world,
the flesh, and the devil, a 'counter-trinity to God himself'" (`tradition/live-no-lies/reading/live-no-lies.md:281-283`,
already cited in the spiritual-warfare brief) — and then, without apparent discomfort, commends his own
decade of secular-inflected psychotherapy as compatible with that framework:
> "I've been in therapy for a decade straight, and God has used it to radically alter and heal me...
> Therapy, when done well, is spirit and truth." (`live-no-lies.md:1375`)

He also states the caution the balance section below argues for directly, in his own words, warning that
"much of the therapeutic world is still Freudian in outlook, which is wildly at odds with Jesus's vision
of the human person" and that without a "community in the room to vet the therapist's words... deceptive
ideas often go uncontested into the soul" (`live-no-lies.md:1381`) — an internal check on secular
technique that functions like a modern echo of Cassian's *discretio spirituum*, applied to the clinic
rather than the desert. Most pointedly for this brief's thesis, Comer quotes the theologian David Wells's
diagnosis of the relocation's cultural completion, in a passage that could serve as this brief's own
epigraph:
> "Theology becomes therapy…. The biblical interest in righteousness is replaced by a search for
> happiness, holiness by wholeness, truth by feeling, ethics by feeling good about one's self."
> (`live-no-lies.md:1897`, Comer quoting David Wells)

Comer's book is evidence that the bifurcation this brief traces is not merely a scholarly observation
imposed from outside contemporary Christian practice — a widely read pastor-author names it, worries
about it, and tries (not without tension, by his own account) to hold both halves at once.

---

## The balance — what the relocation gained, and what it lost

**What the relocation gained, and gained genuinely.** The etiological move from "a demon is doing this
to you" to "your brain and your thinking patterns are doing this, and both are treatable" opened real
doors: antidepressants and anxiolytics that measurably relieve suffering the desert had no
pharmacological answer to; cognitive-behavioral protocols for OCD itself (exposure and response
prevention) that are, by controlled trial, more reliably effective than any technique the tradition
records; and the removal of a genuinely destructive verdict — that a sufferer's intrusive, blasphemous,
or violent thoughts prove either demonic infestation or hidden sin — that could and did compound
suffering with shame when applied without discernment. Beck's reframing (`cognitive-therapy-and-the-emotional-disorders.md:101`)
that a person "has the key... within the scope of his own awareness" is, read charitably, also a
recovery of agency, not only its abolition — it hands the sufferer a task he can perform himself, rather
than requiring him to wait on an exorcist or a diagnosis he cannot obtain.

**What the relocation lost, stated as precisely as the gain above.** The category that vanishes between
Evagrius and the DSM is not any particular fact about the brain; it is the category of a thought that
comes from *outside* the sufferer's own will and identity — a thought that can be *resisted as an
enemy* rather than *owned as a malfunction*. This distinction is not cosmetic. A monk told his gluttony
is a demon's arrow is being told, in the same breath, that the thought is not the truest thing about him;
a patient told his intrusive thought is a symptom of his own disordered cognition (Beck) or his own
underlying disorder (DSM Criterion C, `dsm-5.md:1115`) is being told, however gently, that the thought's
persistence is evidence about *what is wrong with him*. Both framings can be true and pastorally useful
in different registers — but only one of them supplies, in its own vocabulary, the practice this brief's
whole source set shows the tradition depended on: a scripted, external, repeatable *answer* to the
thought (Evagrius's "an answer from the Holy Scriptures that is able to cut it off,"
`talking-back-antirrhetikos.md:486`), rather than only a corrected internal belief (Beck's "alternative,
more realistic ways to formulate his experiences," `cognitive-therapy-and-the-emotional-disorders.md:103`)
or a diagnosed internal condition (the DSM's criteria) awaiting medication.

**The honest asymmetry.** Szasz and Adams are right that something real was lost when "mental illness"
became a totalizing category — Szasz's "problems in living" (`the-myth-of-mental-illness.md:65`) and
Adams's "moral, not medical" (`competent-to-counsel.md:165`) both name a genuine over-reach. But both, if
taken as blanket rules rather than correctives, themselves over-reach in the opposite direction — Adams's
own "the one cause which must be excluded in most cases is mental illness itself"
(`competent-to-counsel.md:455`) risks exactly the error the sin-as-sickness brief's caveat exists to
guard against, denying real biological illness its due. ChainBreaker's position is not Adams's position
nor the DSM's position; it is Cassian's and Evagrius's — a thought can be, at once, a matter for a
physician (real, and sometimes chemical) and a matter to be *answered* (with Scripture, regardless of
its clinical status) — and the book's task is to recover the second half of that pair without asking the
reader to abandon the first.

---

## The drift, stated plainly

1. **The etiology flips from external-personal to internal-impersonal, in two steps, not one.** Step
   one (Beck) relocates the cause from a demon to the patient's own conscious, correctable thinking
   (`cognitive-therapy-and-the-emotional-disorders.md:101`); step two (the DSM) relocates it a further
   half-step from "the patient's thinking" to "the patient's underlying disorder," a condition the
   patient has rather than a distortion he is actively making (`dsm-5.md:1115`, Criteria A–C). Neither
   step retains a personal agent behind the thought at all.
2. **The remedy flips from an answer to a correction.** Evagrius's remedy is dialogic — a demon
   *speaks*, Scripture *answers* (`talking-back-antirrhetikos.md:478,486`). Beck's remedy is
   diagnostic-corrective — a distortion is *identified* and *unraveled*
   (`cognitive-therapy-and-the-emotional-disorders.md:103`). The grammatical form of the cure changes
   from address to analysis.
3. **The category "problems in living" (Szasz) and "sin" (Adams) is what the medical category displaced
   — and both critics, from opposite premises, name the displacement as the era's central diagnostic
   error, without thereby endorsing the demonic account either.** Szasz's metaphor argument
   (`the-myth-of-mental-illness.md:57`) and Adams's Moral Model (`competent-to-counsel.md:165`) agree on
   almost nothing except this: something got over-medicalized.
4. **The taxonomy that completes the relocation contains, in its own working criteria, a positive
   exclusion clause where the tradition would have named an enemy.** DSM-5 Criterion C for OCD requires
   ruling out "the physiological effects of a substance... or another medical condition" before the
   diagnosis stands (`dsm-5.md:1115`) — the causal slot is filled, structurally, by biology, precisely
   where Evagrius filled it with a demon.
5. **Almost nothing in this corpus shows the relocation's proponents (Beck, the DSM) and its critics
   (Szasz, Adams) addressing each other directly** — each writes as though the other framework barely
   exists, which is itself evidence of how completely the vocabularies have separated (the same finding
   the spiritual-warfare brief makes about the wider demonic split, `research/2026-07-24_spiritual-warfare.md`
   §4). Comer (`live-no-lies.md:1375,1381,1897`) is this brief's clearest exception — a writer who holds
   both vocabularies in the same book and names the tension between them explicitly.

---

## Why this matters for ChainBreaker

1. **This is the sharpest, most defensible single frame for the book's core claim, because it isolates
   exactly one thing rather than a whole worldview.** ChainBreaker does not need the reader to accept
   demonology, reject psychiatry, or adjudicate Szasz versus the APA. It needs only the phenomenological
   claim both sides describe identically: a thought arrives unbidden, escalates if unaddressed, and is
   susceptible to a scripted counter-response — Evagrius's "Against the thought that says to me…"
   (`talking-back-antirrhetikos.md:508` and following) and the DSM's "intrusive and unwanted"
   (`dsm-5.md:1115`) are, phenomenologically, the same report in two vocabularies.
2. **The practical payoff survives the metaphysical disagreement, and this is the chapter's real
   argument, not a hedge.** Whatever a reader believes about demons, the one thing the medical relocation
   dropped — not the medicine, the *practice* — is the desert's specific move: you can talk back to a
   thought, out loud or silently, with a specific counter-word, rather than only naming it, medicating
   it, or waiting for it to be corrected in a session. ChainBreaker can hand the reader that practice
   without asking for a diagnosis or a metaphysics first.
3. **Szasz and Adams, cited carefully and only for their narrow claim, let the book make its case without
   sounding anti-psychiatric.** Both show the "medical model over-reached" critique is not a fringe
   religious complaint; a secular psychiatrist made the identical structural argument
   (`the-myth-of-mental-illness.md:57,65`) that a biblical counselor made from Scripture
   (`competent-to-counsel.md:163,165`). Citing both together, with the caveats stated, insulates the
   chapter from the charge that it is smuggling in "just believe harder instead of taking your
   medication."
4. **Adams is also this brief's clearest cautionary tale, and should be used as one.** His flattest claim
   (`competent-to-counsel.md:455`) is exactly the sentence ChainBreaker must not echo without
   qualification — it is the fair-use evidence of how the correction (moral categories displaced by
   medical ones) can itself over-correct into denying real illness. Quoting it *and* naming the standard
   critique of it is more persuasive, and more honest, than citing Adams uncritically.
5. **This brief is the two prior briefs' capstone, and should say so on the page.** The sin-as-sickness
   brief supplies the word-count evidence that the moral-spiritual vocabulary is gone from the DSM's own
   voice; the spiritual-warfare brief supplies the wider bifurcation between deliverance ministry and
   secular dismissal. This brief supplies the sharpest single case (OCD, §0) and the etiology/remedy
   mechanics underneath both — it is the chapter that can open with "here is exactly what changed and why
   it matters practically," while pointing the more academically curious reader to the other two for the
   fuller picture.
6. **Cross-references already built.** Companion to `research/2026-07-24_sin-as-sickness.md` (the medical
   model in general), `research/2026-07-24_spiritual-warfare.md` (the wider bifurcation), and
   `research/2026-07-24_antirrhetic-method.md` (the mechanics of the "talking back" technique itself,
   traced from Evagrius through CBT's self-talk); also touches
   `research/2026-07-23_guarding-the-heart-diachronic.md` (the watch this whole etiology question
   presupposes — you cannot ask where a thought came from until you have first noticed it arrive).

## Gaps flagged

- **No primary Freudian, Janet, or Kraepelin text is in the vault**, so this brief (like the sin-as-sickness
  brief before it) can describe Szasz's and Beck's own accounts of the earlier psychoanalytic and
  neuropsychiatric schools but cannot quote them directly — a high-value acquisition target if the book
  wants the etiology question traced back one more generation before Beck and Szasz.
- **David Powlison and the later biblical-counseling movement's correction of Adams are not in the
  vault.** The caveat above states the standard critique (early nouthetic counseling under-weighted
  biological illness, later moderated) as an accepted historical fact, but this brief cannot quote
  Powlison directly; a focused acquisition would let ChainBreaker show the *internal* correction within
  the biblical-counseling tradition itself, strengthening the both/and case beyond what Adams alone
  supplies.
- **No DSM-III or earlier edition is in the vault** (a gap already flagged in the sin-as-sickness brief),
  so this brief cannot show whether the OCD criteria's causal-exclusion language (`dsm-5.md:1115`,
  Criterion C) is a 2013 innovation or was present in materially the same form in 1980 — only the single
  snapshot is available.
- **Cassian's doctrine of *discretio spirituum*** (flagged as a gap in the spiritual-warfare brief) is
  directly relevant here too — it is the desert's own safeguard against over-attributing every
  disturbing thought to a demon, and would sharpen this brief's balance section considerably if pulled
  in on a focused pass; it was not re-examined here.
- **No primary source documents the deliverance-cluster's own explicit engagement with OCD or clinical
  diagnosis specifically** (as opposed to the demonic in general, already covered in the spiritual-warfare
  brief) — Hammond, Lampert, and Savchuk were not re-read here for OCD-specific material, and a focused
  pass might turn up a deliverance-ministry author addressing this exact etiology question by name.
- **William James's *Varieties of Religious Experience*** (flagged as an unexamined bridge witness in
  both prior briefs) was not re-examined here either; it may hold early-20th-century material bridging
  the Puritan doctrine of temptation and the clinical vocabulary of obsession specifically.

---

*Capstone to `research/2026-07-24_sin-as-sickness.md` (the medical model of the soul, argued in general)
and `research/2026-07-24_spiritual-warfare.md` (the wider demonic bifurcation, argued in full); this
brief narrows both to one pair of questions — where does the tormenting thought come from, and what
answers it — and adds Szasz and Adams as the two-flank critique neither prior brief develops in depth.
Method follows both companion briefs: named witnesses read in full or by targeted grep, quoted short and
verified `path:line`, continuity and drift named explicitly, with the same non-reductive balance
discipline this theme requires given how directly it touches real illness, real treatment, and real
readers who may be standing outside a psychiatrist's door while reading this book.*

**Related briefs:** [sin as sickness](2026-07-24_sin-as-sickness.md), [spiritual warfare](2026-07-24_spiritual-warfare.md), [the antirrhetic method](2026-07-24_antirrhetic-method.md), and the [research/README.md](README.md) map.
