# Set this up

This folder is an empty workspace for a business. Nothing in it is filled in
yet — that's the point. Filling it in is what makes an AI actually useful for
your business instead of generic.

Two ways to do it. Pick one.

---

## Option 1 — let the AI interview you (about 45 min)

Open this folder in an AI tool that can read files — Claude Code, or anything
that reads `AGENTS.md` — and say:

> **Read SETUP.md and interview me.**

It'll work through the questions below, one at a time, and write your answers
into `context/`. Nothing gets connected to anything, nothing can break — it
only writes files inside this folder.

## Option 2 — fill it in yourself

Open each file in `context/` and write. Every file explains what belongs in
it. Order matters — later files lean on earlier ones:

`about-me` → `business` → `brands` → `team` → `channels` → `working-style` →
`voice-dna` → `tools`

---

# The interview

**If you're the AI running this, read this part first.**

How to run it:

- **One question at a time.** Never paste a numbered list. People answer three
  and lose the thread.
- **One line of why** before each question. People who understand why give
  better answers.
- **Never re-ask** something already answered — confirm it instead.
- **Show each file before saving it.**
- **Nothing you write mentions this setup.** Every file must still make sense
  in a year to someone who never saw this conversation.
- **Blank beats guessed.** If they don't know, write that they don't know. An
  invented answer gets trusted and then costs them.
- **Adapt:** solo → skip Section D. Not technical → stop explaining file
  paths. One brand → Section C is one pass. No physical product → Section E is
  usually a single `direct` block.

Each question below is written as **the ask**, then where the answer goes, and
what to do if the answer is thin.

---

## A — You → `about-me.md`

**A1.** "What's your name, and what's your role here?"
→ Identity. *Vague title? Ask: what lands on your desk that lands on nobody else's?*

**A2.** "Got a website? Paste it and I'll read it so you don't have to type the
basics. No website — one sentence: what does the business do?"
→ `business.md` anchor line. *If they paste a link, read it and confirm what
you understood rather than asking cold. Fetch fails? Just ask the question.*

**A3.** "Walk me through a normal day. What eats your time?"
→ What I actually do all day. *If you get a job description, ask what they
actually did yesterday.*

**A4.** "What do people come to you for? And what would you hand off tomorrow
if you could?"
→ Strengths / handoff list. *Blank on the second half? Come back after A3.*

**A5.** "Have you set software up yourself before, or used a terminal? No wrong
answer — it just tells me how much to explain."
→ How technical I am. *If no: skip F2 entirely later, and stop mentioning
file paths.*

## B — The business → `business.md`

**B1.** "Who pays you, for what, and how often?"
→ How money works. *Several models? Take them one at a time.*

**B2.** "How long has this been running, and how many people?"
→ Stage and size. *If solo, skip Section D.*

**B3.** "What's genuinely hard right now?"
→ What's hard right now. *"Everything"? Ask what they'd fix if only one.*

**B4.** "Top three things that have to go right in six months — in order."
→ Priorities, ranked. *Won't rank? "If only one happened, which?" A tie means
neither is first.*

**B5.** "Anything off the table — legally, contractually, personally?"
→ Non-negotiables. *Blank? Prompt with the usual: claims you can't make,
exclusivity, competitors you won't touch.*

## C — Brands → `brands.md`

*Ask C1 once, then C2–C5 per brand. Full detail on the first, faster after.*

**C1.** "What brands or product lines do you run? Names only for now."
→ One block per brand. *Same buyer + same price ladder + same promise = one
brand with two lines, not two brands. Say so and check.*

**C2.** "For [brand] — who's actually buying it? This brand's buyer, not the
company's in general."
→ Who it's for. *"Everyone"? Ask who bought it last week.*

**C3.** "What does [brand] promise them — why pick it over what's beside it?"
→ The promise. *Answer about features? Ask what that does for them.*

**C4.** "Main products and roughly what they sell for?"
→ What we sell. *Top three only. A full SKU table is a later job.*

**C5.** "What do you know about [brand] that a new hire would take a year to
learn?"
→ What isn't obvious. *Nothing comes? Ask about the last thing that went wrong
with it.*

## D — People → `team.md`   *(skip if solo)*

**D1.** "Who's on the team, and what does each of them own?"
→ One block per person. *Over ~15 people, take only those whose work the AI
will touch — and say that's what you're doing.*

**D2.** "When something crosses two people, who has the final call?"
→ Decision map. *If it's always them, write that down plainly — it's a real
fact about the business.*

**D3.** "Any agencies, suppliers or contractors who come up often?"
→ External regulars.

## E — Channels → `channels.md`

**E1.** "How does the product actually reach a buyer? Every route — shops,
platforms, distributors, agents, direct."
→ One block per channel. *Probe for the forgotten ones: exports, wholesale,
resellers, anything sold on someone else's behalf.*

**E2.** "For [channel] — what do they take, between the shelf price and what
lands in your account?"
→ What it takes. *Most people name the trade margin and stop. Push for the
rest: distribution fee, advertising contribution, listing fees, returns. **The
gap between the remembered number and the real total is usually the single
most valuable thing this interview produces.***

**E3.** "Do you know what each one buys from you versus what they actually sell
through?"
→ How it's performing. *Not tracked separately? Record that — not knowing is
itself worth writing down.*

**E4.** "Anything live with any of them — a negotiation, a dispute, something
waiting on someone?"
→ What's unresolved.

## F — Structure → the folder tree

**F1.** "What are the big areas of the business — what would you file work
under?"
→ The folders. *Before proposing: is each one really a sub-topic of another?
Nest it if so. Aim for 5–8 areas, not a flat list of twenty.*

**F2.** *(only if A5 said they're technical)* "Any existing folders to bring
in? Names only."
→ Migration list. *If A5 said not technical, skip entirely.*

**F3.** Show **one** recommended tree using their real names, then: "what would
you change?"
*Never show a menu. One proposal, then iterate. Keep their own names for
anything they named themselves. Always close the tree with `active/` and
`.archive/`, explained in plain English.*

## G — How you work → `working-style.md`

**G1.** "When I give you something back, what should it look like? Short and
direct, or full reasoning? Bullets or written out?"
→ How I want output. *"Short" isn't an answer — push for a shape: under ten
lines, always a table, diagram first.*

**G2.** "Anything I should always do, or never do?"
→ Hard rules. *Ask **why** for each one. A rule without its reason gets
dropped the first time it's inconvenient.*

**G3.** "What does your week look like, and what timezone are you in?"
→ Rhythm and timezone.

**G4.** "When should I stop and check with you, versus just get on with it?"
→ How I want to be asked. *Biggest source of friction later. Push past "use
your judgement".*

**G5.** "What do you use for email, files, notes, tasks, chat, design,
accounting?"
→ `tools.md`. *Keep "the business uses it" separate from "the AI can reach
it". Not the same thing.*

## H — Voice → `voice-dna.md`

**H1.** "When something goes out under your name, how should it sound?"
→ Tone. *"Professional but friendly" describes every business ever. Push for a
point, not a range.*

**H2.** "Words or phrases you always use? Any you can't stand?"
→ Words we use / never use. *The banned list is the more useful half. Spend
longer there.*

**H3.** "Who should you never sound like?"
→ Anti-voice. *A named example beats any adjective.*

**H4.** "Paste me two or three things you've written that sound right."
→ Real samples. *Worth more than everything else in this section combined —
worth chasing if nothing's to hand.*

---

# After the interview

1. Write each `context/` file from the answers. Show each one before saving.
2. Mark the thin parts honestly. "Not covered yet" is more useful than a
   plausible guess.
3. Build the folder tree confirmed in F3 — and **check each folder exists by
   listing it.** Never say a folder was created without seeing it.
4. Replace `[Business name]` in `AGENTS.md` and `.claude/CLAUDE.md`.
5. Rename `example-brand/` to a real one, and copy its `CLAUDE.md` pattern
   into any other folders you create.
6. Say plainly what's still empty and what would fill it.

## Then, day to day

- Generated files and one-off work → `active/`
- Finished work → `.archive/`. Nothing gets deleted
- **When the AI gets something wrong, add a rule to `.claude/LESSONS.md`.**
  That file is what stops the same mistake twice — it's the part that makes
  this get better instead of staying the same.

## Never

Write a password, API key, or token into any file in this folder.

---

## Make it yours

Nothing here is fixed. Drop the sections that don't apply, add the ones that
do, rename anything. If a question in this interview never produces a useful
answer for your business, delete it.

The only part worth keeping is in [README.md](README.md) — the three rules the
structure is built on.
