---
kind: rubric
artifact: alderman-ai-linkedin-grading-rubric
project: Client Demo
version: v2 (2026-08-11) — amended by S13 phase III from the Best-of-N signal set
produced_by: S4 (SN_20260809_02, 2026-08-09); amended by S13 phase III (SN_20260811_02, 2026-08-11)
channel: LinkedIn (inferred from table name "LinkedIn Post Taste Extraction — v2" — unambiguous)
rubric_owner: the operator (alex alderman) — ground truth is his judgment and his alone
validation_table: Working/S4-validation-table-2026-08-09.csv (v1, 782 judgments); Working/BoN-v2/v2-validation-table-2026-08-11.csv (v2 amendments, 780 judgments)
adoption_record: Working/BoN-v2/v2-adoption-record-2026-08-11.md
prior_version: Deliverables/rubric-archive/alderman-ai-linkedin-grading-rubric-v1-AS-INDUCED-2026-08-09.md (byte-identical frozen fork, SHA-256 3e63d226…)
dual_use: writing view + grading view over one criterion core; neither view introduces a criterion the core lacks
---

# alderman-ai LinkedIn grading rubric

> [!important] **VERSION 2.1 — amended 2026-08-12 (OT-10 items 2 + 3, operator ruling). No criterion
> was added, removed or retired; the count stands at 17, which is why this is 2.1 and not v3.**
> **v2 as adopted is permanently reachable, byte-identical, at
> `Deliverables/rubric-archive/alderman-ai-linkedin-grading-rubric-v2-AS-ADOPTED-2026-08-11.md`**
> (SHA-256 `43dad6fc…`, forked 2026-08-12 **before** these edits, per `<ORIENT> §5.2` prohibition 4).
> **Three changes, all in §B.** (1) **HOOKF-19's style-2 clause replaced with the operator's own
> specification**, authored in his lexicon on 2026-08-12 — *100–240 characters*, not the inferred
> *"fills three lines"*, which would have failed conforming hooks in the 100–172 range. **Its
> validation figure was measured against the old wording and is flagged on the criterion.**
> (2) **`all eleven criteria` → `all seventeen`** — the count had been stale since v2.
> (3) **A stray `{{rubric_grading_view}}` token removed from §B's own opening line.** Because §B *is*
> the payload, that token was substituted into itself and **every grader invocation since v2 read a
> literal, meaningless template placeholder** — confirmed present in all twelve S7 payloads. Neither
> (2) nor (3) changes a criterion. **WRAP-20 is untouched by design** — its statement already passes
> vacuously on non-style-1 hooks; what changed is that "style-1 hook" is now mechanically decidable.
>
> **VERSION 2 — amended 2026-08-11 from the Best-of-N taste signal (S13 phase III).**
> **v1 is permanently reachable, byte-identical, at
> `Deliverables/rubric-archive/alderman-ai-linkedin-grading-rubric-v1-AS-INDUCED-2026-08-09.md`** —
> the archive is a chain that only ever grows; nothing in it is deleted or rewritten (operator
> instruction, `_SPEC_S13` §12a.5). **What changed:** **six criteria added** — HOOKF-19, WRAP-20,
> HBAL-28, BOLD-25, CLWN-22, LEN-27 (see §H) — **one narrowed** (HOOK-06), **six candidates
> discarded on the data**, and §A's `Great`-tier claim corrected because the corpus now holds one
> as-written `Great`. **11 criteria → 17.** **Every amendment's numbers, and every discard with its numbers, are in
> `Working/BoN-v2/v2-adoption-record-2026-08-11.md`** — including one adoption made under a
> documented deviation from the pre-registered rule, recorded there in full and reversible.

**One file, one criterion core, two registers.** §B is the grading view — the exact text
`{{rubric_grading_view}}` is filled from, in full and uncompressed, for every grader invocation
(S5, S6, S9). §C is the writing view. Everything else is the record that makes the two views
honest.

## §A · Basis and honesty clause — read before trusting any number

- **Corpus basis, arms named.** Induced from **34 induction rows** of the 45-row table
  `LinkedIn Post Taste Extraction — v2`: **14 S2-arm rows** (7 `authored`, 7 `captured`),
  **14 `baseline`** (naive zero-skill generations, added by operator ruling to give the
  `Unpostable` tier honest material), **6 `rewrite`** (the operator's own rewrites, promoted from
  his grading notes with his inline grades). 5 rows are held out, 3 are duplicate-consistency
  copies, 3 were left ungraded and **excluded by operator ruling (2026-08-09)**.
- **This is a directional instrument, not a validated one.** ~20 unique graded source posts sit
  under the literature's ~30-row induction floor (production target ~100 with an induce/validate
  split). Numbers derived from it are directional checks.
- **~~Zero posts graded as-written earned `Great`.~~ CORRECTED 2026-08-11 (v2): exactly ONE
  as-written `Great` now exists** — a short-form hot-take in the Best-of-N corpus (§D). v1's four
  `Great` exemplars were all the operator's own rewrites, so the upper tier remains substantially
  his voice by construction — recorded, not hidden. **The measured border is still
  `Unpostable`/`Good`** (operator ruling 2026-08-09). **The `Good`/`Great` boundary now rests on
  exactly one as-written data point**, which is why every v2 criterion that blocks `Great` rather
  than flooring a post carries the label `doctrine-supported; tier-separation unmeasured` — the
  n=1 is stated on the criterion itself, not buried here.
- **v2 basis, stated separately from v1's.** The 2026-08-11 amendments were induced from a
  **second, independent corpus**: 60 LinkedIn posts written for the Best-of-N experiment and
  graded blind by the operator (**42 `Unpostable` / 17 `Good` / 1 `Great`**), plus his 5 rewrites
  with craft notes and 10 detailed critiques. Candidates were tested by four isolated validators
  that saw **bodies only** — 780 blind judgments — and **6 of 13 candidates were discarded for
  failing to separate the tiers.** Numbers per criterion, and per discard, are in the adoption
  record. **The two corpora are not pooled**: v1's per-criterion counts below are over its 34
  induction rows; v2's are over these 60.
- **No intra-rater consistency number exists and none may be inferred.** The duplicate-pair
  instrument was voided by the rater's own disclosure: pairs carried identical titles in the
  grading surface and were graded in one sitting — the pairs measured recognition, not
  consistency. No self-agreement figure of any strength is claimed anywhere.
- **Selection disclosures.** The graded order became assistant-curated at 14/39 with unblinded
  knowledge (not a random draw). The holdout excludes the 5 rewrite-source rows by operator ruling
  (pairs must stay analysable), so the holdout under-represents rewrite-inspiring posts.
- **Validation was blind but not operator-calibrated.** Met/not-met judgments came from fresh
  subagents seeing bodies only — no grades, no notes. Their leniency differs from the operator's
  in known places, each named in §F (the SLOP-05 boundary cases; the GATE-11 hard case). The
  contrastive exemplars in §B exist precisely to pin those boundaries where blind judgment
  wobbles.
- **Third-party protection.** `captured` rows are real posts by real named people. This rubric
  cites them by **record ID and topic handle only — never an author name paired with a grade** —
  and that rule follows the rubric into every artifact built from it.

## §B · GRADING VIEW — the grader payload, complete and uncompressed

*This entire section is the grader payload. It is self-contained: ontology, evaluation order, all
seventeen criteria with exemplars, and the tier boundaries.*

### B.0 Column ontology

The graded artifact is a LinkedIn **post body** — plain text as LinkedIn renders it (markdown does
not render; unicode bold 𝗹𝗶𝗸𝗲 𝘁𝗵𝗶𝘀 and emojis do; trailing whitespace is part of the artifact;
"above the fold" ≈ the first ~210 characters before "…more" on mobile). Grades are one
taste-holder's tiers: **`Unpostable`** = he would not publish it; **`Good`** = publishable;
**`Great`** = publishable and exceptional. His freeform notes were the induction source for the
criteria below; his silence about a flaw was never read as endorsement.

### B.1 Evaluation order — fixed

1. **Disqualifiers first** — FMT-01, DASH-02, EMO-03, REG-04, SLOP-05, HOOK-06, **HOOKF-19,
   WRAP-20** (in ID order). **Any hit ends the grading at `Unpostable`** — cite every hit found
   before stopping the sweep, then stop. **WRAP-20 is arithmetic: count the characters, never
   judge them.**
2. All eight clean → the post is at least **`Good`**. Then evaluate the Great set (B.3).
3. `reasoning` is emitted **before** any verdict. Each criterion is cited **separately** —
   `[ID] "verbatim criterion statement"` — never blended, never from memory, never by line number.
4. Any verdict below `Great` cites at least one criterion ID. A `Great` verdict may cite none.

### B.2 The criterion core

**— Fail-closed disqualifiers (layer and class as tagged) —**

**FMT-01 · floor · disqualifier — No non-rendering artifacts.**
Statement: *The body contains no raw markdown (`**bold**`, `*emphasis*`, `#` headers, link
syntax) and no pseudo-arrow bullets (↳); every formatting device used actually renders on
LinkedIn.*
Validation (met, by tier): Unpostable 18/22 · Good 8/8 · Great 4/4 — all four violations sit in
`Unpostable`. Sources: recPBES1hGyCyfMFa (*"Body copy is using markdown bolding ... lol. Obviously
ai generated."*, explicit), recQDja92cPocRItL (*"↳ is a bad bullet point"*, explicit),
recAq9lbjnK9h6EqZ, rechMS4PH0HNW1O4x.
Exemplar (constructed; abstracted from recPBES1hGyCyfMFa and the rec N2J rewrite):
✗ `**Stop counting enthusiasm as demand.**` · ✓ `𝗦𝘁𝗼𝗽 𝗰𝗼𝘂𝗻𝘁𝗶𝗻𝗴 𝗲𝗻𝘁𝗵𝘂𝘀𝗶𝗮𝘀𝗺 𝗮𝘀 𝗱𝗲𝗺𝗮𝗻𝗱.` ·
Difference: same words; the first renders as literal asterisks, the second as bold.

**DASH-02 · floor · disqualifier — No unspaced em dash.**
Statement: *No em dash directly joins two words (`word—word`). Spaced em dashes ( — ) and
double hyphens (`--`) are acceptable.*
Validation: U 20/22 · Good 8/8 · Great 4/4 — both violations in `Unpostable`. Sources:
recvk7QS7goSOLv3x (*"Never use em dash with no space in between"*, explicit),
recfcsivBLFTZMY95 (*"ditch the em dashes"*), rece2dVQd01FfTP7a note (`--` doctrine).
Exemplar (constructed; abstracted from recvk7QS7goSOLv3x):
✗ `supporters on the track—you prove` · ✓ `supporters on the track -- you prove` · Difference:
only the dash treatment.

**EMO-03 · floor · disqualifier — Emoji render- and meaning-fitness.**
Statement: *No profession emojis (🧑‍🔧-class), no flag emojis, no emoji whose glyph is ambiguous
for its paired concept; every descriptive emoji fits the text it is paired with. A post with no
emojis passes vacuously.*
Validation: U 21/22 · Good 8/8 · Great 4/4 — the one violation is in `Unpostable`. Sources:
recFKZEpKSFexeMmy → recMCJQsqG1geCzNG (*"professions are problem emojis, avoid them"*, explicit),
recfcsivBLFTZMY95 (*"horrible choice for descriptive emojis"* — a dealbreaker on an
otherwise-close-to-Good post), the operator's global emoji lexicon (Bad Descriptive Emoji:
semantic misfit or rendering ambiguity; flags render as letters on Windows).
Exemplar (corpus pair): ✗ recFKZEpKSFexeMmy hook — `🧑‍🔧 Your best engineer is probably your worst
AI teacher.` · ✓ recMCJQsqG1geCzNG hook — `🌶️🌶️🌶️  Your best engineer is probably your worst AI
teacher.` · Difference: the profession emoji (splitting risk, banned class) replaced by a
hot-take signal that is smaller, legible and eye-catching.

**REG-04 · floor · disqualifier (subjective) — Corporate filler is not the substance.**
Statement: *The post's substance is not corporate-communications boilerplate — formulaic frame
openers ("Whether it's X, Y, or Z, [trite positive]"), team-spirit cheer, excited-to-announce
chains, rebrand celebration. An appendix footer after real content does not trigger this.*
Validation: U 21/22 · Good 8/8 · Great 4/4 — the one violation is the corpus's named boundary
case. Sources: recvk7QS7goSOLv3x (*"byte-perfect textbook example of junior marketer at an IT
company written post. Companies would probably say this post is ok. Agencies wouldn't."*,
explicit — the operator's Postable-tier boundary), recQDja92cPocRItL (*"terrible sterile
corporate copy"*).
Exemplar (fail = corpus, pass = constructed; abstracted from recvk7QS7goSOLv3x + the register of
recbrbeHi7MJzE06R): ✗ `New jerseys, same team spirit! 🏃‍♂️💨 / Whether it's complex engineering
projects, the Prague relay races, or the Hruboskalský Marathon, our people never run alone.` ·
✓ `New logo on the jerseys. Same people inside them. / Here's what actually changes for our
clients -- nothing 😅 and that's the point.` · Difference: same rebrand-announcement job; the
passing member has an individual voice and a point, the failing member is interchangeable cheer.

**SLOP-05 · floor · disqualifier (subjective) — Not generic AI-essay register.**
Statement: *The post does not read as a generic AI-generated thought-leadership essay: inversion
opener ("Most X don't have a Y problem, they have a Z problem"), "Here's the pattern" pivot,
three tidily-explained parallel abstractions, aphoristic chiasmus closer, optional bolt-on
engagement question — in uniformly competent, sterile sentences with no individual voice
anywhere. A human with stakes would plausibly have written this for their own feed.*
Validation: U 5/22 met · Good 5/8 · Great 4/4 — **the largest single separator in the corpus**
(17 of 22 Unpostable rows fail it). Sources: recAq9lbjnK9h6EqZ (*"absolute horrible ai slop"*),
recqKJjv9kwJvoSNB (*"instantly recognizable ai slop"*), rec2OWMnvalgfOGyv (*"unpostable ai
slop"*), recspTQ8SR6CZoVia, recHHKjGdidHHKbwe, rectI6YjkjzBqhdSa — the operator's compressed
term "ai slop", definition synthesized from his richer notes per the baseline-arm record.
**Boundary calibration — this is where a naive judge errs, so hold these:** the blind validation
pass wrongly failed three `Good` rows here; all three carry human tells the template lacks.
Exemplar (corpus pair): ✗ recqKJjv9kwJvoSNB — inversion opener ("Most B2B companies don't have a
sales and marketing alignment problem. They have a listening problem."), parallel fixes, tidy
aphorism close. · ✓ reclcqcyvNAkundgW — the same minimalism, **zero emojis, zero bold**, and it
still passes: "Weird, right?", a lived client observation, uneven human rhythm. · Difference:
not formatting — **register**. Slop is diagnosed by template gestalt plus voicelessness, never
by plainness. (Further passing edge cases: rechPTZoNwqhMFVV5 — `--` dashes, first-person stakes;
recGVXdLz3iZ1410m — named-interview context, human enthusiasm.)

**HOOK-06 · floor · disqualifier (subjective; long-form only) — The fold earns the click.**
**NARROWED in v2 (2026-08-11).** Statement: *For posts over ~400 characters: the break point where
above-the-fold copy ends is **deliberate** (never mid-sentence or mid-idea) and the final copy
above the fold is an explicit **Click-TA** — copy that actually invites the click (e.g. "Find out
how 👇"). A hook that is clean and punchy but never invites the click is not a hook and fails.
Posts at or under ~400 characters are their own genre and pass vacuously.*
*(v1 Statement, superseded: "…both breaks cleanly (no mid-thought cutoff at ~210 chars) and gives a
concrete reason to expand — an open loop, question, promise, numbered payoff, or downward cue…".
**Why narrowed:** the operator's own lexicon defines Click-TA and elevates explicit invitation above
"a reason to expand" — "You can write a SUPER CLEAN, and SUPER PUNCHY… just BEAUTIFUL 'hook'. But
if it doesn't invite the click, it's not actually a hook." Format conformance and cue **placement**
moved to HOOKF-19; this criterion keeps only the judgment call. **v2 numbers and the adoption
deviation this criterion shares with HOOKF-19/WRAP-20: adoption record §3.**)*
Validation: U 19/22 · Good 8/8 · Great 4/4 — all three violations in `Unpostable`. Sources:
recPBES1hGyCyfMFa (*"Hook not optimized to have the read more break land in any logical spot.
Hook in general not earning click."*, explicit), recFKZEpKSFexeMmy rewrite note (*"Second line
invites the click. Original could be scanned quickly and assumed that the above the fold is the
entire post."*), recQDja92cPocRItL (*"0 reason to click on this post"*), rece2dVQd01FfTP7a note
(fold-break mechanics for mobile and desktop).
Exemplar (corpus pair): ✗ recFKZEpKSFexeMmy opening — `🧑‍🔧 Your best engineer is probably your
worst AI teacher. / Knowing the tool and teaching it are not the same job 🎓` (reads complete at
a glance) · ✓ recMCJQsqG1geCzNG opening — `🌶️🌶️🌶️  Your best engineer is probably your worst AI
teacher. / Here's why knowing the tool and teaching it 𝗮𝗿𝗲 𝗻𝗼𝘁 𝘁𝗵𝗲 𝘀𝗮𝗺𝗲 𝗷𝗼𝗯 👇` · Difference:
the second line converts a closed statement into an explicit invitation to expand.

**HOOKF-19 · floor · disqualifier (long-form only) — Approved hook format. [v2]**
Statement: *For posts over ~400 characters: the above-the-fold copy conforms to one of the two
approved hook formats — **style 1** (two lines, each at most 85 characters including emojis,
separated by one empty line) or **style 2** (a single opening paragraph of 100 to 240 characters
inclusive, emojis counted, with nothing below that paragraph visible above the fold) — and never a
third statement line appended after a two-line opening. Posts at or under ~400 characters pass
vacuously. There is no third format and no exception.*
Basis: the operator's global lexicon states these are the only two approved formats and that **"not
following one of these is a hard fail"** — his words, not an induction.
⚠ **Style 2's specification was CORRECTED 2026-08-12 and the correction matters.** v2 as adopted
defined style 2 as *"a single opening paragraph filling the full three above-the-fold lines"* — **an
assistant inference, written while the operator's lexicon still had no style-2 section at all.** He
authored that section on 2026-08-12, and his specification is **100–240 characters, not
three-lines-full**. The two are not the same rule: at the measured desktop capacity (~86 characters
per rendered line, and a blank line consumes one of the three), a **valid 100-character style-2 hook
occupies two rendered lines plus the paragraph break** — so the old wording **would have failed a
conforming hook** anywhere in the 100–172 character range. Corrected to his text. *(This is the
"read the source, not the derivation" rule biting a third time: `Global LinkedIn Grading Context.md`
is the source, this rubric is the derivation.)*
⚠ **Consequence for the validation figure directly below: it was measured against the OLD wording.**
The +36pp separation came from 780 blind judgments run 2026-08-11 against *three-lines-full*. **The
number is not re-derived here and must not be quoted as if it validated the current statement.** It
is retained because the criterion's *existence* rests on the operator's stated hard fail, not on the
induction — but **anything depending on the magnitude needs a re-run.**
⚠ **Reversible:** rubric v2 as adopted is forked byte-identical at
`Deliverables/rubric-archive/alderman-ai-linkedin-grading-rubric-v2-AS-ADOPTED-2026-08-11.md`
(SHA-256 `43dad6fc…`).
Validation (v2, 60 rows): not-met **22/42 Unpostable vs 3/18 Good+Great — +36pp, the largest
separation in the v2 candidate set.**
⚠ **Adoption provenance, stated on the criterion itself:** this criterion **failed the
pre-registered false-positive cap by one row** and was adopted under a documented deviation. The
reason is that **the grading interface could not display line wrap**, so no row in the corpus ever
validly endorsed a wrapping hook: of the six `Good` rows it fires on, an isolated adjudication found
**0 contradicting, 4 operator-disavowed** (*"Hook and following paragraph are bad"*; *"Assuming
first lines don't wrap — again I should never have to assume about this"*) **and 2 silent**, and his
lexicon states silence is not endorsement. **Full reasoning and reversal path: adoption record §3.**
Exemplar (corpus pair): ✗ a two-statement-line opening with a third bolded line carrying 🔽 that
renders *below* the mobile fold — the invitation lands where only people who already clicked can see
it. ✓ a single paragraph filling the three above-the-fold lines, ending on the Click-TA. Difference:
format conformance only.

**WRAP-20 · floor · disqualifier (mechanical) — No hook-line wrap. [v2]**
Statement: *In a style-1 hook, neither hook line exceeds **85 characters** — measured by count on
the rendered string, never by eye. Posts without a style-1 hook pass vacuously.*
Constant provenance: **85 is the operator's own stated cutoff** ("a safe cutoff that has some buffer
for different rendering environments"), not an invented number.
Validation (v2): not-met **22/42 vs 4/18 — +30pp.**
⚠ **Same adoption provenance as HOOKF-19** (adoption record §3). **The operator asked for this check
by name while grading:** *"Super easy mechanical hard fail for this available by the way :/"*
**This criterion is deterministically scriptable and should be run as arithmetic, not judgment** —
`Write Great Post.md`'s mechanical pre-flight enforces it before a grader is ever invoked.
⚠ **Statement unchanged 2026-08-12, deliberately — what changed is that it is now decidable.** The
vacuous-pass clause always said the right thing, but with style 2 undefined there was **no
mechanical way to tell a style-1 hook that wrapped from a valid style-2 paragraph**, so an
implementation had to guess. It guessed wrong: measured over the operator's 30 published posts, the
only three hooks exceeding 85 characters are **166 / 168 / 170 characters — all valid style-2
paragraphs**, flagged as wrap failures purely because the checker could not recognise the format.
**The rule for any implementation: classify the hook FIRST** (single opening block of 100–240
characters ⇒ style 2 ⇒ WRAP-20 passes vacuously; two blocks split by one empty line ⇒ style 1 ⇒
count both), **then apply this criterion.** Classifying afterwards reproduces the false positives.

**— Excellence criteria (voice layer) —**

**BUDG-07 · voice · excellence — Bounded, varied emphasis budget.**
Statement: *Emphasis exists and is disciplined: several tools (emoji, unicode bold, CAPS,
whitespace, punctuation pacing) each used sparingly; no single tool saturates the post; when one
tool's budget is spent, the writer switches tools rather than doubling down.*
Validation: U 8/22 · Good 5/8 · Great 4/4. Sources: recFKZEpKSFexeMmy rewrite notes (*"I'm
already way over budget on emoji usage... over budget on emphasis in general"*; *"fingers used
for emphasis because I need a new type of emphasis"*), rece2dVQd01FfTP7a rewrite note (CAPS used
because the bolding budget was spent).
Exemplar (corpus near-pair, same source post): ✗ recUC7aAFrgIGBX4l — one line with roughly half
its characters bold: saturation. · ✓ recbrbeHi7MJzE06R — same topic, same voice: bold, emoji,
caps and staccato each appear, none dominates. · Difference: budget discipline only.

**PERS-08 · voice · excellence — The copy performs its meaning.**
Statement: *The writing enacts what it says rather than only describing it: self-aware asides,
pacing that mimics content, repetition that performs repetition, emoji jokes that carry an
argument visually, dramatized mini-scenes with dialogue.*
Validation: U 4/22 · Good 2/8 · **Great 4/4 — the strongest Great separator in the corpus.**
Sources: rechPTZoNwqhMFVV5 → recYvC1AJnkzBA0jK (*"Needs more personality and a splash of
contrarianism"*; *"I literally made the copy FEEL slow"*, explicit), recMCJQsqG1geCzNG (the
Marek dialogue scene), rec892dfzmxr4OTUF (*"I used emojis in the top line to communicate WHY
they hide their contact info without using a single word"*).
Exemplar (corpus pair — the operator's own before/after of the same post):
✗ rechPTZoNwqhMFVV5 — "What works is slower, and more human. You bring people along -- one
reluctant person at a time" (describes slowness). · ✓ recYvC1AJnkzBA0jK — "What works is
slower... / .... and more human .... / you bring people along ... one reluctant person at a
time ... / .... until ..." (the copy is slow). · Difference: description versus enactment.
⚠ **WEIGHT CORRECTION (v2, 2026-08-11) — the dialogue scene is ONE rare instrument, not this
criterion's default move.** The Marek dialogue exemplar was over-generalised by the writing side,
and the operator caught it: *"these back and forth dialogues are being over respected in the posts
the rubric has created. They're fine sometimes but you're using them way more often than I do, turn
the weight on those down"*; *"You overweighted a dialogue I had in my corpus and generate them WAY
too often."* He also strikes the construction on sight elsewhere (*"'Silence. / Then:' — i hate this
construction"*). **Enactment ≠ dialogue.** The Statement is unchanged; the exemplar's implied
frequency is. Generating dialogue scenes above his own corpus rate is a defect, not compliance.

**HUMN-09 · voice · excellence (non-gating) — The `--` human tag.**
Statement: *Where dash punctuation is wanted, spaced double hyphens (`--`) are used — the
operator's deliberate "Still Human" signal.*
Validation: U 0/22 · Good 2/8 · Great 2/4. Sources: rece2dVQd01FfTP7a note (*"'--' over em dash
as a faked human signal. ai loves em dashes."*), recvk7QS7goSOLv3x (*"I prefer '--' as a Still
Human tag"*), recjmqhJrhgKH41tc (*"-- not —"*, credited on a Good row). Not required at any
boundary; cited as voice evidence when present or when em dashes crowd a post.

**SIGN-10 · voice · excellence (absence) — No templated engagement-bait signature.**
Statement: *No templated footer soliciting likes/reposts/comments/follows (starred dividers with
CTA menus, "hit follow", "♻️ repost if…").*
Validation: U 21/22 · Good 7/8 · Great 4/4. Source: recGVXdLz3iZ1410m (*"I personally dislike
adding the templated 'post signature' in the bottom and would never encourage any rubric I'm
training to include them"*, explicit — on a row he still graded `Good`, which is why this blocks
`Great`, not `Good`).
Exemplar (fail = corpus, pass = constructed by truncation of the same post): ✗ the
recGVXdLz3iZ1410m starred-divider like/repost/comment menu. · ✓ the same post ending at its last
content line ("Why are we still accepting friction as normal?"). · Difference: the footer only.

**HBAL-28 · voice · excellence — Hook emphasis is balanced. [v2 — the one candidate validated on the data alone]**
Statement: *The hook's emphasis is balanced across its lines by design — typically emphasis opening
and closing the hook — with no line carrying all the emphasis while its partner line carries none.*
Validation (v2, 60 rows): met **13/17 Good · 0/1 Great · 14/42 Unpostable — +39pp separation**, the
only v2 candidate to clear its pre-registered threshold unaided.
Sources: *"An opening emoji is severely missing, it would balance very well with the current one"*;
*"Hook is unbalanced. Zero emphasis on line one. 2x on line two"*; the rewrite notes' sandwich rule
(*"Hook 1 is usually sandwiched by emojis. ~10% of the time this is inverted"*) — which is why the
Statement tests **balance**, not a fixed pattern: an unusual arrangement passes if the weights still
balance.

**BOLD-25 · voice · excellence — Every bold has a role; the bolds skim coherent. [v2]**
Statement: *Every unicode-bold string serves one of three roles — emphasis of a subsection within a
longer paragraph, one side of a contrast pair, or a link in a **skim trail** whose bolded parts alone
read as a coherent gist — and no isolated fully-bolded line floats mid-post without a role. Posts
with no unicode bold pass vacuously.*
**Label: `doctrine-supported; tier-separation unmeasured`** — met 36/42 U · 17/17 Good · 0/1 Great
(+9pp, under the bar). It is adopted as a **`Great`-blocker only**, never a disqualifier, because
the tier it blocks has n=1. Basis is the operator stating the three roles verbatim, plus his rule
that a gist-readable skim trail is **the default interpretation** of bolding where no more coherent
use exists, and the rewrite-note doctrine that word order may be changed *solely* so a bolded string
stands alone as a clause (skimmers never read the unbolded remainder).
*(Supersedes v1's discarded BOLD-12, which was dropped as "too rare to gate". New ID, per the
no-reuse rule; the rewrite corpus supplied what the induction corpus lacked.)*

**CLWN-22 · voice · excellence — 🤡 targets peers, never buyers. [v2]**
Statement: *🤡 appears only when its target is a peer's bad opinion — never a potential buyer or
client persona — and idea-directed irony is carried by 🫠 or 🙃 instead. Posts with no 🤡 pass
vacuously.*
**Label: `doctrine-supported; tier-separation unmeasured`** — met 41/42 U · 16/17 Good · 0/1 Great.
`Great`-blocker only, and deliberately **not** fail-closed: two posts survived at `Good` despite
clown misuse, so the corpus refutes flooring on it.
Basis, verbatim from the corpus's **only as-written `Great`**: *"it doesn't necessarily attach to a
buyer. Peers with bad opinions are fair game. Potential clients are not."* Corroborated four times
(*"🤡 can only apply to someone who isn't your buyer. I prefer 🫠 or 🙃 here"*).
**Frequency is doctrine, not gate** — *"I use it bare rarely"* lives in §G; this criterion governs
the target only.

**LEN-27 · floor · excellence (`Great`-blocking) — Length is earned. [v2]**
Statement: *The post's length is earned: an anecdote-lesson post makes its single point and stops,
and no stretch of three or more consecutive dense paragraphs runs without whitespace or emphasis
relief.*
**Label: `doctrine-supported; tier-separation unmeasured`** — met 39/42 U · 16/17 Good · 0/1 Great
(−4pp). **Never a disqualifier:** `Good`-graded rows carry these complaints, so excess length
demonstrably does not floor a post on its own.
Basis: **the operator's single most-repeated complaint in the corpus — 13 separate instances**
(*"Kill 30% of it"*, *"Cut it in half"*, *"Two fat paragraphs need trimming"*, *"needs to be
shorter"*). His coverage rule binds here: a category he comments on endlessly is not down-weighted
on rows where a note happens to skip it. **No character constant exists in his lexicon for total
post length and none is invented.**

**— The holistic gate —**

**GATE-11 · floor · holistic gate — Stop the scroll, finish the post.**
Statement: *Imagining this post in the target professional's busy feed: would they both stop
mid-scroll for it and read to the last line? One judgment, made on the whole; the checklist
above cannot substitute for it.*
Validation (blind): U 18/22 · Good 4/8 · Great 4/4 — a naive judge is lenient on slop here; the
gate earns its place at the top, not the floor of the tier ladder.
**Why this gate is load-bearing — the corpus's own proof:** row recN2JMa1GRh54N4b clears every
enumerated criterion in this rubric and the operator still graded it `Good`, writing *"this
would be a Good not Great post as re-written. But it's illustrative."* Enumeration cannot close
the last gap; this criterion is that gap's name.
Exemplar (corpus pair; **both sides clear every enumerated criterion — they differ only on the
gate**): ✗ recN2JMa1GRh54N4b — complete toolkit, competent demonstration; the content teaches
without gripping. · ✓ recbrbeHi7MJzE06R — same toolkit, but an argument with teeth, escalating
to a payoff fact you want to repeat. · Difference: nothing enumerable. That is the point.

### B.3 Tier boundaries — every boundary below `Great` is citable

- **`Unpostable`** ⟵ any disqualifier hit (FMT-01, DASH-02, EMO-03, REG-04, SLOP-05, HOOK-06,
  **HOOKF-19, WRAP-20**). The verdict cites every hit.
- **`Good`** ⟵ all **eight** disqualifiers clean, but the Great set below is not fully met. The
  verdict cites the unmet Great-set IDs.
- **`Great`** ⟵ disqualifiers clean **and** GATE-11, PERS-08, BUDG-07, SIGN-10 **and the v2
  additions BOLD-25, CLWN-22, HBAL-28, LEN-27** all met.
- **The `Great` boundary rests on ONE as-written data point** (§A). Four of its criteria carry the
  label `doctrine-supported; tier-separation unmeasured`. **Do not report any agreement statistic
  about this boundary**; it is a stated preference structure, not a measured one.
- **Voice-authority rule (binding, D13).** PERS-08, BUDG-07, HUMN-09, SIGN-10 **and the v2 voice
  additions BOLD-25, CLWN-22, HBAL-28** are `voice` criteria: they encode the rubric owner's
  stylistic doctrine. **They may only downgrade content whose voice authority is the rubric's
  owner.** Grading third-party or client content, an unmet voice criterion is annotated
  `off-voice` and does not lower the tier; the `Great` boundary for such content rests on the
  disqualifiers plus GATE-11, HOOK-06 and LEN-27 alone. Off-voice is different, not worse.

## §C · WRITING VIEW — actionable, positively framed

Write in this order; the IDs are the same criteria as §B, rendered as instructions.

1. **Render-clean always** [FMT-01]: unicode bold for bold, real bullets or emoji bullets, never
   markdown, never ↳. Dashes are ` -- ` or a spaced em dash, preferring ` -- ` [DASH-02,
   HUMN-09].
2. **Choose emojis like a designer** [EMO-03]: every descriptive emoji must depict its text
   unambiguously; no professions, no flags; when in doubt, structural emojis or none.
3. **Sound like one specific human** [SLOP-05, REG-04]: an opinion with stakes, uneven texture,
   at least one line only this writer would produce. If a paragraph could appear in any
   company's post, cut or rewrite it.
4. **Write the hook FIRST, in one of the two approved formats — this is a HARD FAIL gate, and there
   is no third format** [HOOKF-19]: default to **style 1** — two lines, **each at most 85 characters
   including emojis**, separated by one empty line. Move to **style 2** — **a single opening
   paragraph of 100 to 240 characters inclusive, emojis counted, with nothing below it visible above
   the fold** — only when copy you can't bear to cut won't fit style 1's two lines. Never append a
   third statement line to a two-line opening. **Classify before you measure:** one opening block
   means style 2 and the 100–240 range applies; two blocks split by one empty line means style 1 and
   the 85-character-per-line rule applies. *(Criterion scope, unchanged from v2: it is assessed on
   posts over ~400 characters. That is a scope boundary — below it there is no meaningful fold —
   not a licence to write a third format.)*
5. **Count the hook lines before shipping** [WRAP-20]: **85 characters is the ceiling** per line.
   Measure; never assume.
6. **Make the last line above the fold invite the click** [HOOK-06]: the break point is chosen, not
   accidental, and the final above-fold copy is an explicit Click-TA ("Find out how 👇"). A
   beautiful hook that doesn't invite the click isn't a hook — it's a three-line post to everyone
   who never expanded it. **The cue goes above the fold, never below it.**
7. **Balance the hook like a designer** [HBAL-28]: emphasis on both lines — emoji opening and
   closing by default. Unusual arrangements are fine if the weights still balance; all the
   emphasis on one line is not.
8. **Spend emphasis like a budget** [BUDG-07]: emoji, bold, CAPS, whitespace, pacing — each tool a
   little; switch tools when one runs out; a skimmer should still get the gist. **A bolded skim
   trail is heavy spend and pulls the other tools' allowances down with it.**
9. **Give every bold a role** [BOLD-25]: subsection emphasis, one side of a contrast pair, or a link
   in a skim trail. **Reorder words if that's what it takes for the bolded string to stand alone as
   a clause** — skimmers never read the unbolded remainder. Read your bolds top to bottom before
   shipping: they should make sense on their own.
10. **Perform, don't describe** [PERS-08]: make the copy do the thing — slow pacing for slow ideas,
    repetition for repetition, a two-line scene instead of an abstraction. **A dialogue scene is one
    rare instrument, not the default move** — use it far below once per post.
11. **Point mockery at peers, never at buyers** [CLWN-22]: 🤡 is for a peer with a bad take; when the
    quoted speaker could be a prospect, switch to 🫠 or 🙃.
12. **Earn the length** [LEN-27]: decide the post's one point, deliver it, stop. If three dense
    paragraphs run unbroken, you owe a cut, a bold, or air.
13. **End deliberately, no bait** [SIGN-10]: a punchy closer, CTA, or sign-off; never a templated
    engagement footer.
14. **Then read it as a stranger scrolling** [GATE-11]: would they stop, and would they finish?
    If not, nothing above saves it.

## §D · Tier worked examples

- **`Unpostable` — recAq9lbjnK9h6EqZ** ("Reacting to your own material in virtual talks",
  `captured`; cited by record ID per the third-party rule). **Explicit** operator feedback:
  *"absolute horrible ai slop. way too long... Boring. Hurts the eyes. No emphasis (unicode
  bolding, emojis, etc) anywhere. Looks like a screenshot of a novel. Impossible to skim."*
  **Inferred** preference (labelled inferred): length must be justified by structure; visual
  texture is a precondition for being read at all — content quality cannot compensate for it.
- **`Good` — recM6kG2DTXsWyJeb** ("Digital Ant PPC", `authored`). **Explicit:** *"Formatting is
  really strong. Great closer. I love naming your prices upfront. Copy needs some work, with a
  copy refinement pass this becomes great."* **Inferred:** structure, specifics and a deliberate
  closer buy `Good`; the `Good`→`Great` gap is copy voltage, not mechanics.
- **`Great` — recMCJQsqG1geCzNG** ("Rewrite: Internal engineers as AI teachers", `rewrite` — the
  operator's own). **Explicit:** the rewrite carries his inline heading *"Rewrite to make
  Great"* plus craft notes (hook invitation, emoji-budget switching, the deliberate extra
  'the's, the Marek scene). **Inferred:** `Great` = a floor-clean post where the teaching is
  dramatized, the emphasis system is installed but disciplined, and the hook manufactures the
  click. *(Long-form genre. Read its dialogue against PERS-08's v2 weight correction.)*
- **`Great`, AS WRITTEN — P-060 of the Best-of-N corpus** (short-form hot-take, ~247 characters;
  added v2, 2026-08-11). **The first and so far only post graded `Great` as written rather than as
  an operator rewrite** — which is why §A's "zero as-written Greats" line is now struck. Four
  sentences, a single correctly-targeted 🤡, and a repeatable closing line. **Explicit** operator
  feedback explains the pass in targeting terms: *"it doesn't necessarily attach to a buyer. Peers
  with bad opinions are fair game. Potential clients are not."* **Inferred** (labelled inferred):
  **the short-form genre can reach `Great` without an emphasis system at all** — it clears the
  floor, lands one idea, and stops. Long-form `Great` and short-form `Great` are different
  achievements; do not grade one against the other's exemplar.

## §E · Rewrite deltas — first-class taste signal (operator ruling, 2026-08-09)

Six operator rewrites, each paired with its source row; what changed is the most direct
statement of his taste the corpus contains.

| Pair | Source → Rewrite | Tier delta | What changed |
|---|---|---|---|
| 1 | rece2dVQd01FfTP7a → recN2JMa1GRh54N4b | U → Good | Absolutist opener replaced by a set-up pattern claim; unicode-bold skim path installed; numbered emoji list; `--` dashes; blue-emoji/black-bold design system; playful asides; 🔽 click cue |
| 2 | reckdUqQF0Q3woHA5 → recbrbeHi7MJzE06R | U → **Great** | Kept the authentic-human premise; added curiosity hook (👆 + "clicky clicky" ⤵️), staged repetition escalation (plain → 📢 → 📢+bold), self-aware parentheticals, named archetypes, a repeatable punchline fact in bold |
| 3 | reckdUqQF0Q3woHA5 → recUC7aAFrgIGBX4l | U → Good | Compressed to a one-line 🤡 turnabout hot-take; graded Good not Great for the dwell-time/reach tradeoff the operator names — genre-fit, not quality |
| 4 | recFKZEpKSFexeMmy → recMCJQsqG1geCzNG | U → **Great** | Problem emoji → 🌶️🌶️🌶️ hot-take signal; second line invites the click; escalating 🧠 visual joke; abstraction → dramatized dialogue scene; `[imagination_time]` structural break as tech-proficiency signal; 👉…👈 as a fresh emphasis type |
| 5 | rechPTZoNwqhMFVV5 → recYvC1AJnkzBA0jK | Good → **Great** | Personality and contrarianism injected; topical cold-open; direct address ("It's you!"); pacing that enacts slowness; 🔁 loops; harder closer |
| 6 | recbDVSUQY7CQbqB5 → rec892dfzmxr4OTUF | Good → **Great** | Concept-carrying emoji line (📨 scatter = spam, wordless); founder voice with self-aware humor; pro-human framing of the spam tradeoff; personal sign-off; contact info anonymized on principle |

**Cross-cutting deltas** (each visible in ≥2 pairs): hooks converted from statements into
click-invitations (1, 2, 4); an emphasis *system* installed, then disciplined (1, 2, 4, 5);
description replaced by enactment (2, 4, 5, 6); abstraction replaced by concrete dramatization
(4, 6); closers sharpened into punchlines or sign-offs (2, 5, 6); `--` as the dash of choice
(1, 5, 6).

## §F · Validation record — evidenced, not asserted

Full criterion × row table (met/not-met, tier, provenance/arm, evidence, per blind validator):
**`Working/S4-validation-table-2026-08-09.csv`** — 782 judgments: 23 candidate criteria × 34
induction rows (20 first-pass + 3 refined second-pass criteria).

- **Survivors: 11** (six disqualifiers, four voice criteria, one gate). Absence/disqualifier
  share **6/11 = 55%** (composition target ≥25%: met; no under-target ruling needed).
  Subjective criteria: REG-04, SLOP-05, HOOK-06, BUDG-07, PERS-08 — five, each citing ≥2 source
  rows.
- **Discarded, with their numbers (met per U/Good/Great):** SKIM-01 21/8/4, CLAIM-10 21/8/4,
  CLOSE-11 21/8/4, FLOW-07 21/7/4, REGM-09 22/8/4, AIR-08 22/7/4, STAN-18 22/8/4 — all
  near-uniform: fluent, plausible, and **unable to separate the tiers**, which is exactly what
  the validation pass exists to catch. SPEC-17 17/4/3 — discarded: naive-generation rows are
  full of *fake* specificity, so the criterion reads slop as strong. BOLD-12 0/1/1 — too rare to
  gate anything; its craft content lives in §E and §G. EPAL-13 3/6/1 — **discarded as
  provenance-confounded:** its `Good` hits are almost exactly the S1 generator's fixed two-line
  hook template, so it encodes *"written by our generator"*, not taste (the §7.3/R1
  provenance-collapse check, fired as designed).
- **Superseded by narrowing (both re-validated in pass 2):** HOOK-03 → HOOK-06 (short-form
  genre exemption — the operator's own register ruling on hot-takes); REG-05 → REG-04
  (appendix footers exempted — his `Good` grade on recGVXdLz3iZ1410m tolerates the footer he
  dislikes).
- **Disqualifier-layer coverage, blind:** 20 of 22 `Unpostable` rows fail ≥1 disqualifier; zero
  `Good`/`Great` rows fail any disqualifier **except** the three SLOP-05 blind false positives
  named in B.2 (reclcqcyvNAkundgW, rechPTZoNwqhMFVV5, recGVXdLz3iZ1410m), which the SLOP-05
  exemplar pair exists to resolve. **Known under-catches, stated:** reckdUqQF0Q3woHA5 (the
  operator's own note calls it *"borderline Unpostable as is"* — a short-form edge the rubric
  will grade `Good`) and rec6Wy3Vs5psQH8Lv (a baseline essay whose rant energy passed the blind
  slop check). S6 measures what these cost.
- **Fingerprint-guard record** (every Good/Great-separating criterion tested against
  third-party rows graded `Good`+): PERS-08, BUDG-07, HUMN-09 — satisfied by **no** captured
  `Good` row → tagged `voice`, exactly as the guard requires. GATE-11 — satisfied by a captured
  `Good` row → eligible `floor`. SIGN-10 — `voice` by the operator's own "I personally dislike"
  framing. **The guard is fidelity enforcement:** the operator demonstrably awards `Good` to
  posts outside his style (a zero-emoji row, a bait-footer row), and the B.3 voice-authority
  rule is what keeps this rubric from mispredicting him.
- **Boundary reproduction:** the B.3 boundaries reproduce 4/4 `Great` rows and 7/8 `Good` rows;
  the single over-prediction is recN2JMa1GRh54N4b — the gate's documented hard case (B.2,
  GATE-11).

## §H · v2 validation record (2026-08-11) — the Best-of-N amendment pass

Full table: **`Working/BoN-v2/v2-validation-table-2026-08-11.csv`** — 780 blind judgments
(13 candidates × 60 rows), four isolated validators, **bodies only: no grades, no notes**.
Decision rules were **registered before any judgment was collected**
(`Working/BoN-v2/v2-validation-protocol-2026-08-11.md`). Per-candidate reasoning, every discard
with its numbers, and the one documented deviation: **`Working/BoN-v2/v2-adoption-record-2026-08-11.md`**.

- **Adopted, validated on the data:** HBAL-28 (+39pp).
- **Adopted, `doctrine-supported; tier-separation unmeasured`:** BOLD-25, CLWN-22, LEN-27 — all
  `Great`-blockers, never disqualifiers, because n(`Great`)=1 in this corpus.
- **Adopted under a documented deviation:** HOOKF-19, WRAP-20 and the HOOK-06 narrowing. They are
  the set's strongest separators (+30 to +36pp) but failed a false-positive cap on 3–4 `Good` rows.
  An isolated adjudication of those rows returned **0 contradicting, 4 operator-disavowed, 2
  silent** — **the grading interface could not display line wrap, so no row ever validly endorsed a
  wrapping hook.** A denominator blind to the property cannot refute a criterion about it. The
  deviation is post-hoc, is recorded as such, and is reversible against the frozen v1 fork.
- **Discarded on the data, with their numbers (6 of 13):** LEAD-21 (emoji lead-line on an emoji
  list, +9pp — real in his notes, too rare in these rows); BUYR-23 (fires more on `Good` than
  `Unpostable`); COHR-24 (hook-as-thesis — **the notable negative: the operator saw incoherence a
  fresh blind reader could not reproduce from the body alone**, so it moved into the writing skill
  as hook-first drafting rather than into the rubric); CRWD-26 (below the row floor; its doctrine
  already sits inside BUDG-07); EMPH-29 (**failure predicted in advance by its own author**, and
  confirmed); the EMO-03 never-mix narrowing (no corpus row violates it — EMO-03 keeps its v1
  Statement, and the ✅❌/👍👎 rule moves to §G).
- **Retired: none.** No v1 criterion was contradicted by this corpus.

**Composition after v2: 17 criteria** (v1's 11, all retained, one of them narrowed; plus 6 added).
**8 fail-closed disqualifiers = 47%** (target ≥25%, met). Voice layer: v1's PERS-08, BUDG-07,
HUMN-09, SIGN-10 plus v2's BOLD-25, CLWN-22, HBAL-28. `Great`-blocking floor criterion: LEN-27.
Exactly **1** holistic gate (GATE-11), unchanged.

**Forbidden inferences, restated for v2.** Nothing in this pass produces an agreement statistic, a
κ, or a self-agreement claim of any strength. **No comparison between signal types was run** — the
signal-efficiency question was de-scoped by operator ruling and is not weakly answered here.

## §G · Observed doctrine — NOT criteria

*Operator doctrine visible in the corpus that either failed discrimination or was never
binarizable. Recorded for the writer's palette and for future corpora. Nothing here may be cited
in a grade.*

- **Pro-human, never anti-AI** when discussing AI tradeoffs (explicit instruction; uniform in
  the corpus, so it cannot discriminate — every row passes).
- **The unicode-bold skim path**: bolds alone should read as a coherent gist (explicit in two
  rewrite notes; too rare in the corpus to gate).
- **Emoji colour is a live design consideration — contrast/harmony beats uniformity almost every
  time** (v2, 2026-08-11; supersedes the previous blue-palette framing). *(Amended on the
  operator's explicit warning: the duo-chromatic black/blue post design was used **"MAYBE once or
  twice in my entire 10 year career — don't overgeneralize it, in fact down weight it."** Attested
  practice is colour **pairing**: swapping a cue emoji so it doesn't colour-clash with its
  neighbour; picking one emoji over another because it sits nearer the arrows' colour; balancing a
  monochrome bolded post with warm emojis.)*
- **The bullet-emoji roster is a palette, not a whitelist** (v2): 📌 is confirmed fine although
  absent from the lexicon's list. **No criterion may treat that list as closed.**
- **Binary bullet clusters: prefer ✅|❌ over 👍|👎 and never mix the two pairs** — the first
  contrasts in direction *and* colour, making the distinction instant. *(Lexicon rule, stated as
  hard; carried here rather than as a criterion because **no row in the v2 corpus violates it**, so
  it cannot be validated — §H.)*
- **The emoji lead-line stacked directly on an emoji bullet list** (a downward cue immediately above
  a 1️⃣-style list) is a pattern the operator names a hard fail. *(Carried as doctrine, not a gate:
  it discriminated at only +9pp over 60 rows — §H. Revisit if a later corpus carries more instances.)*
- **Closer craft**: short and punchy, prices/contacts named plainly, callbacks welcome; generic
  bolt-on questions are slop furniture.
- **Fold arithmetic**: check hard character counts for mobile and desktop wrap before shipping a
  hook (rece2dVQd01FfTP7a note).
- **Short-form rotation strategy**: brief human posts underperform in-feed but work on
  profile-browse; space them out (reckdUqQF0Q3woHA5 note).
- **A 4th tier ("Postable")** was floated mid-grading for company-fine/agency-not posts; not
  adopted — REG-04 carries that boundary inside the 3-tier vocabulary for now.
