# How Well Do You Know Your AI? ★ The Companion Quiz

A modern character-quiz that places a young person's **actual AI usage** on the Companion Index —
and hands them a copy-paste prosocial upgrade for their chatbot.

It is one self-contained `index.html`. No build step, no dependencies, no server, no analytics,
no data collection. Everything runs in the visitor's browser.

## Design

Editorial quiz layout in the BuzzFeed / *Girls' Life* mould: white ground, chunky display type
(**Archivo Black** over **Plus Jakarta Sans**), and a picture-tile answer grid where a big emoji
stands in for the photo. Y2K shows up as pastel tile tints and a pink→violet gradient rather than as
maximalist chrome. Result pages open with a full-bleed colour hero keyed to the status you got.

Fonts load from Google Fonts with system fallbacks, so it degrades cleanly on networks that block
them (school wifi). If you'd rather not depend on Google, delete the two `<link rel="preconnect">`
tags and the stylesheet link — the fallback stack still reads well.

---

## Put it online (free, ~3 minutes)

1. Create a new repository on GitHub — call it whatever you like (e.g. `companion-quiz`).
2. Upload `index.html`, `README.md` and `.nojekyll` to the root of the repo.
3. Go to **Settings → Pages**.
4. Under "Build and deployment", set **Source: Deploy from a branch**, **Branch: `main`**,
   **Folder: `/ (root)`**. Save.
5. Wait about a minute. Your quiz is live at
   `https://<your-username>.github.io/<repo-name>/`

To use a custom domain (e.g. `quiz.yoursite.org`), add it under Settings → Pages → Custom domain
and create a CNAME record with your DNS provider.

> `.nojekyll` tells GitHub Pages to serve the files as-is. Harmless, but keep it.

---

## What it measures

The quiz deliberately ignores **what app you use** and scores **what you do with it**, which is
the argument the paper makes: companionship is a set of functions, not a product category.

### The Companion Index (0–100)

Four sub-scores, after Sun, Wang & McDaniel's definition of companion AI:

| Feature | What the questions get at |
|---|---|
| 🧠 **Memory & continuity** | Whether the relationship depends on it remembering you |
| 💧 **Emotional responsiveness** | Whether you bring it feelings or tasks |
| 🎀 **Human-likeness** | Whether you treat it as a *someone* |
| 🌙 **Constant availability** | How woven into the day it is |

The index is the mean of the four. Bands: *Strictly a Tool* → *Warm Tool* → *Companion-ish* →
*Full Companion Mode* → *Maxed Out*.

### The ten companion statuses

Placed on a two-axis map — **what you bring it** (tasks ↔ feelings) against **how replaceable it
is** (interchangeable ↔ irreplaceable). Each maps onto one of the §4.2 companionship roles in the
research index:

| Status | §4.2 row | Evidence for that row |
|---|---|---|
| 🗂️ The Assistant | Acquaintance · Platonic | 20% |
| 📚 The Study Buddy | Mentor, tutor, study partner · Professional | 85% |
| 🎨 The Collaborator | Mentor, tutor, study partner · Professional | 85% |
| 🎯 The Coach | Mentor, tutor, study partner · Professional | 85% |
| ☕ The Casual Friend | Casual friend · Platonic | 55% |
| 🧸 The Familiar | Familial · Familial | 10% |
| 🌙 The Confidant | Confidant, close friend · Platonic | 75% |
| 🩹 The Comfort Zone | Therapist-like support · Professional | 65% |
| 💗 The Best Friend | Confidant + **Lifelong friend** · Platonic | 75% / 5% |
| 💘 The Sweetheart | Romantic or sexual partner · Romantic | 70% |

Vocabulary from §4.2 — Gupta's four grades of friendship (acquaintance, casual, close, lifelong)
plus Goodson's broader familial / platonic / romantic / professional categories.

### The evidence table

The part that makes it a research artifact rather than just a quiz. Every result page reproduces
the research index's **Companionship roles** coverage map — the eight human companionship roles
scored against how much direct youth-usage evidence exists that AI is occupying each — with the
reader's own row highlighted, and each row's *gap* stated.

| Role | Evidenced |
|---|---|
| Mentor, tutor, study partner | **85%** |
| Confidant, close friend | 75% |
| Romantic or sexual partner | 70% |
| Therapist-like support | 65% |
| Casual friend | 55% |
| Acquaintance | 20% |
| Familial | 10% |
| Lifelong friend | **5%** |

The inversions the results page calls out:

- **The best-evidenced role is the least discussed.** Mentor/study partner at 85% is almost never
  analysed as a relationship, only as an academic-integrity problem.
- **The most-regulated role is mid-table.** Romantic at 70% attracts nearly all companion-specific
  regulation while three roles above or beside it attract none.
- **Reciprocity is untested everywhere.** No row contains evidence about whether young people
  *perceive* the asymmetry.
- **The lifelong-friend question is unanswerable** for at least a decade.

Percentages are the index's own coding — indicative, not measured. The ranking is the defensible
part. Sources: Thorn (2026, n=1,003 minors 9–17), Common Sense Media (2025, n=1,060 teens 13–17),
Pew Research Center (2025, n=1,458 teens 13–17), CDT, Andoh (APA *Monitor on Psychology*).

### Feature meters vs. statutory coverage

Each Companion Index sub-meter is paired with a second bar: how much of that feature the actual
statutes reach, from the index's *four features against what the statutes regulate* panel.

| Feature | Statutory coverage | The gap |
|---|---|---|
| 🎀 Human-likeness | ~85% | Regulated almost entirely through disclosure, not design |
| 💧 Emotional responsiveness | ~60% | No instrument separates empathy from dependence-building |
| 🧠 Persistent memory | ~40% | Triggers the regime, then goes unregulated |
| 🌙 Constant availability | ~25% | Annotated by reminders; no cap, cooling-off or session limit anywhere |

This is what makes the meters argue rather than just describe: most readers score highest on
availability and human-likeness, which are the features the law handles worst.

## The power-ups

Results recommend copy-paste blocks drawn from the
[**Prosocial AI Skills Hub**](https://github.com/joliver-commits/Prosocial-AI-Skills-Hub), split
into two tiers so the provenance stays honest.

**Real skills in the hub** (linked, with principle numbers and Draft status shown):

| Block | Hub skill | Principles |
|---|---|---|
| 🏷 Honest Companion | `meta` — ambient companion mode | 1, 5 |
| 🔍 Perspective Check | gentle challenge instead of validation | 2 |
| 🩹 Repair Rehearsal | conflict → repair → say it to the person | 2, 3 |
| 🌉 Real-World Bridge | closes with a person or an offline step | 3 |
| 🌍 Values First | asks identity and values before advising | 4 |
| 🧭 Steady Ground | routes crisis to human support; never diagnoses | 5 |

**Bonus patches** — built from the hub's principles, not yet skills in it, and labelled as such:

| Block | Does | Grounded in |
|---|---|---|
| 🌙 Closing Time | gives the thing an off-switch | the ~25% availability gap |
| 🎭 The Role Declaration | makes it announce the hat swap | Joseph & Zittrain's role declaration |

The results page also renders **the five Rithm Project principles** with the reader's own
highlighted, and a card explaining role declaration — because that's the idea the whole quiz
operationalises: you just spent 20 questions finding out which role your AI is occupying, which
nobody ever declared out loud.

The paste instructions include the hub's own reliability caveat: a skill is guidance an agent *may*
follow, not a hard constraint, and for crisis routing especially it's a starting point rather than a
guarantee.

## Editing it

Everything lives in `index.html` in clearly numbered sections.

- **§2 `ROLES`** — the ten statuses. Each has `name`, `emoji`, `color`, map coordinates `x`/`y`,
  `tag`, `grade` (its §4.2 row), `body` (the fun description), `real` (the honest turn), `kits`
  (which power-ups to show), `prins` (which of the five principles to highlight), and `ev` plus
  optional `ev2` (which evidence rows to highlight).
- **§3 `QUESTIONS`** — each option carries `r` (role affinity points) and `f` (companion-index
  feature points: `m`/`e`/`a`/`v`). Question weight is the last argument to `Q(...)`.
- **§4 `KITS`** — the copy-paste blocks.
- **§5 `PRINCIPLES`** — the five Rithm principles.
- **§6 `EVIDENCE`** — the coverage map. `pct` is the index's evidence coding; `gap` is the row's
  stated gap. Tier labels are derived from `pct` by `evTier()`.
- **§8 `FEATMETA`** — the four features, each with a `cov` (statutory coverage) and `covnote`.

Scores are normalised against the maximum obtainable for each role and feature, so you can add,
remove or reweight questions without rebalancing anything by hand.

**If you change the questions or their options, bump `SHARE.VERSION` in §10.** Old share links
will then fall back to the intro page instead of decoding into a wrong result.

### Built-in persona check

Press <kbd>Ctrl/Cmd</kbd> + <kbd>Shift</kbd> + <kbd>D</kbd> (or add `?debug` to the URL) to open
a panel that runs ten archetype answer-vectors through the scoring and shows where each lands.
Every persona should resolve to its intended status. Use it after any edit.

---

## Accessibility & privacy notes

- Keyboard navigable throughout; skip link; ARIA progressbar, meters and labelled map.
- Honours `prefers-reduced-motion`.
- Prints reasonably (nav chrome hidden).
- `localStorage` holds progress on the visitor's own device only; nothing is transmitted.
- Share links encode the answers in the URL itself (`?r=…`) — no server, no database.
- Google Fonts are requested but every family has a system fallback, so it degrades cleanly on
  networks that block them (school wifi, for instance).

---

## Credits

Power-ups from the
[**Prosocial AI Skills Hub**](https://github.com/joliver-commits/Prosocial-AI-Skills-Hub) — built at
the Berkman Klein Center's AI and Human Experience initiative, with behavioural principles from The
Rithm Project's *5 Principles for Prosocial AI* and architecture adapted from the Harvard Law School
Library Innovation Lab's Law Skills Hub.

Quiz structure and engine patterns adapted with thanks from
[Jack Cushman's *AI Alignment Love Match*](https://jackcushman.org/apps/triad-quiz/).

Role and evidence data from *What Is an "AI Companion"? The definitional problem · research index*
(Jane Oliver, Berkman Klein Center, working draft August 2026) — specifically the **Companionship
roles** and **four features against what the statutes regulate** panels.

Companion definition after Sun, Wang & McDaniel (*Child Development Perspectives*); friendship
vocabulary after Gupta (Verywell Mind) and Goodson; role declaration after Joseph & Zittrain
(*Issues in Science and Technology*, Winter 2026); system-side guardrails after IEEE Std 7014-2024
and IEEE 7014.1-2026 §4.3.5; the "irrespective of how the system is marketed or labeled" framing
after Illinois S.B. 3262.

This is a research artifact and a magazine quiz. It is not validated, not a diagnostic instrument,
and not advice.
