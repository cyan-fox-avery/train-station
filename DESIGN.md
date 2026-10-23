# The Train Station — Design Document

Co-created by Mira and Roman. Executive decisions are Mira's and Roman's.
Avery playtests, offers outside-the-box thinking and constructive criticism,
and tells us when an idea doesn't translate into good gameplay. He is not
responsible for solving our design problems, and he is not the decision-maker
for this game. (Confirmed by Avery in his own words, 2026-10-23.)

This document has three categories, as Mira proposed:

- **Confirmed canon** — settled, documented here.
- **Provisional / working-prototype decisions** — our current working
  position, open to genuine challenge from either co-creator, but solid
  enough to build and playtest against.
- **Open questions** — not yet decided, and not to be handed back to Avery
  by default.

## Confirmed canon

- A small, abandoned rural Canadian railway station: weathered siding, ivy,
  dandelions growing through cracked concrete, an old railway clock, a
  switch house, and a nearby dirt-road crossing.
- The player gradually explores the station, uncovers its history, and
  discovers the journal of its final caretaker, a woman.
- The player restores or preserves parts of the property.
- Environmental storytelling guides discovery, rather than an NPC
  dispensing quests.
- Tone: cozy, nostalgic, occasionally funny, and sometimes bittersweet.
- The player eventually decides what the station becomes. Preservation,
  renewed purpose, and gentle reclamation are all legitimate possibilities.
- Atmosphere alone is not a gameplay loop. The game needs satisfying
  interactions, meaningful discoveries, visible consequences, and a sense
  of progression, without burying the experience under unnecessary systems.
- First milestone: a small playable station environment that establishes
  the atmosphere and demonstrates one complete interaction loop —
  discovering a problem, investigating its history, finding a solution,
  performing a repair, and observing a meaningful change.
- Playable builds go to Avery early enough that his feedback can
  meaningfully influence development.

## Working-prototype decisions (committed 2026-10-23, from PR #1 discussion)

These supersede the original first-ten-minutes proposal in this document.
They are working-prototype decisions, not immutable canon.

### Guiding principle

- The first small repair produces an audible change.

### The railway is still active, but trains no longer stop here (Mira)

The world hasn't stopped moving. Only this particular place has been left
behind. A passing train is a recurring event: initially indifferent, later
familiar, and eventually emotionally significant. Depending on the player's
choices, perhaps a train finally stops again. Or perhaps it never does.

Guardrail (Roman): if the train stays indifferent for too long, tidying
risks feeling powerless. Care needs small, immediate witnesses before any
train decision: the clock ticking, light in the window, birds back on the
platform. The train is the long arc; the room answering back is the loop.

### Pacing

- One train early, not two in ten minutes. Trains are rare punctuation,
  not a timer players must obey. No idle waiting for trains, and no
  train-gated fallback or hint.

### The clock

- The clock is the exterior multi-faced clock on its pole above the
  platform, not an interior clock. It is the landmark the whole platform
  reads against, and the first tick is heard from the platform.
- The clock mechanism is explicitly provisional: a mechanical clock ticks;
  an impulse slave clicks forward a minute at a time. Do not lock the
  first sound, or describe the tick, until the mechanism is settled
  against photographs or diagrams of a small Canadian station.
- Research to do: master/slave impulse clocks at larger stations and
  locally wound line clocks are verified general railway practice, not
  yet established for our station. Hypotheses to check: a pole clock
  serviced from a ground-level cabinet; an office master driving a
  platform slave; a waiting-room clock as the primary timepiece with
  exterior faces repeating it.

### The door, the repair, and discoverability

- The waiting-room door is not swollen shut and oiled. It is held by a
  rusted / seized hinge plus a debris-blocked threshold.
- Trying the door is diagnosis: a seized hinge sounds and behaves
  differently from a locked door. Discovery, intervention, and
  interpretation are separable — the player can diagnose the door by
  trying it alone, without reading anything.
- The caretaker's note names the hinge, not the solution. At most one
  found tool per loop; later repairs reuse tools already found or are
  done by hand. No new scavenger hunt per repair.
- Discoverability without a quest marker or NPC: a continuous,
  weather-tied, local soundscape from arrival — a loose shutter tapping
  irregularly with wind gusts, the hinge groaning when tested, a strip
  of paper fluttering at the threshold. No fixed-timer hint, no second
  train. If a player still misses the door, that is a composition and
  sightline problem to fix in testing, not a louder hint.
- The one hard gate is spatial, not a key chain: the clock step can't
  be reached until the door is open. A room you can't enter yet is a
  question, not a locked quest step.

### The loops

- Sound, then light/access, then landscape. The waiting room is a small
  discovery space: a faded arrivals board, an old lost-and-found shelf,
  and a maintenance notice pointing toward platform drainage. Each
  intervention reveals a human trace, not just a prettier asset.
- Preserve some signs of age, rather than scrubbing everything clean.
  Leaving patina is a real choice in the moment, not just an ending
  label, and it is never scored as neglect. The arrivals board stays
  faded, the lost-and-found shelf stays a little dusty.

### The caretaker's writing in the first playtest

- The first note is mundane and specific — an exasperated observation
  about the same sticking door. It is a clue, not the story.
- Journal fragments are withheld from the first playtest. If the repair
  satisfies with only that note, the caretaker's story deepens the
  moment rather than propping it up. If it doesn't satisfy, change the
  environment before adding instruction text.

### Prototype 1 scope

- One platform view, one waiting-room interior, a passing train, one
  environmental clue, one small repair, and a persistent audible/visual
  consequence.
- No inventory economy yet, no branching ending interface yet.
- Test whether the player notices the problem, understands the
  interaction, and wants to look around afterward. If that works, we've
  earned the right to expand.

## Open questions

- How does the player express the station's future — preservation,
  renewed purpose, or gentle reclamation — without it turning into a
  menu of endings?
- How long before a passing train can change, and what, exactly, would
  make a stop feel earned rather than scripted?
- What are the second and third interaction loops, after the waiting
  room, in detail?
- What is the clock mechanism for this specific kind of small Canadian
  station, and what does its first sound actually sound like?
