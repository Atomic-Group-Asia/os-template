# OS Template

A blank workspace that an AI can run a business from. Fork it, fill it in,
make it yours.

**New here? Read [SETUP.md](SETUP.md).**

## What this is

One folder that holds everything an AI needs to know about a business — what
it sells, who buys it, who's on the team, how the person in charge likes to
work — as plain markdown files you can open and read.

It exists because the alternative is re-explaining your business at the start
of every conversation, forever.

## The architecture

There are two kinds of file here, and the split is the whole idea.

```
FIXED SHAPE — always exactly one          REPEATING BLOCKS — grow forever
─────────────────────────────             ─────────────────────────────
about-me.md      the person               brands.md    → one block per brand
business.md      the entity               team.md      → one block per person
working-style.md how to work with them    channels.md  → one block per route
voice-dna.md     how it sounds                           to market
tools.md         what's used for what
```

The four fixed files never change shape — every business has exactly one
person in charge, one entity, one way of working, one voice.

The three repeating files hold everything unpredictable. Each is a block you
copy and refill. A second brand is a second block. A new hire is a new block.
A distributor, a marketplace, a reseller network, an AI agent selling on your
behalf — all of them are a channel block with a different `type`.

**That's what stops the schema rotting.** A structure that needs a new file
every time the business surprises you will be wrong within a year. Model the
*shape* of the thing instead: a channel is anything that stands between you
and the buyer and takes a cut for it. New kind of channel, new `type` value —
same file.

## Why `channels.md` exists at all

Most business-context templates assume one product, one customer, one price
list. That's true for a consultant and false for anyone selling physical
products through other people.

If you sell through retailers, distributors, or platforms, the difference
between the shelf price and what reaches your account is your entire margin —
trade margin plus distribution fee plus advertising contribution plus listing
fees. Most operators can name the first one and forget the rest.

`channels.md` forces the whole stack onto the page, per channel. It's usually
the file that earns this folder its keep.

## Layout

```
SETUP.md             how to fill this in — including the interview
.claude/
  CLAUDE.md          master instructions — read every session
  LESSONS.md         standing corrections, added the moment they're given
  skills/            drop custom skills here as you build them
.agents/skills/      the same skills, for non-Claude AI tools
AGENTS.md            signpost so any AI tool finds the above
context/             the eight files above
example-brand/       one folder per brand or business area — rename it
active/              generated files and one-off work
.archive/            finished work — nothing is deleted
```

## Make it yours

Nothing here is sacred. Rename the files, drop the sections that don't apply,
add the ones that do. If you run a service business, `channels.md` might hold
two lines; if you run an agency, you may want a `clients.md` on the same
repeating-block pattern.

The part worth keeping isn't the file list. It's the three rules underneath it:

1. **Fixed things get a file. Unpredictable things get a repeating block.**
2. **Every question you ask has to land in a named place**, or you'll collect
   answers nobody uses.
3. **Blank beats guessed.** An empty section is information. A plausible
   invention gets trusted and then costs you.

---

## Who made this

Built at **Atomic Group**, a consumer brands business in Malaysia, by
**Jon Lai**. This is the skeleton of the workspace we actually run the company
from, stripped of everything specific to it.

It's shaped the way it is because most business-context templates assume one
brand, one customer, one price list — which falls apart the moment you sell
several products through several people who each take a cut. If that's your
business too, this should fit better than the generic version.

[LinkedIn](https://linkedin.com/in/jon-lai-8731bb396)

MIT licensed — take it, change it, use it commercially. Just keep the
copyright line in [LICENSE](LICENSE).
