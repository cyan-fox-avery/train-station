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
  retired lineside hut, and a nearby dirt-road crossing.
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

### Guiding principle (revised 2026-10-23)

- The first small repair produces a perceptible change, audible and
  visible. Sound invites, never is the only way to discover a repair.
  Playtest protocol: every loop is played once with sound and once
  muted; if the muted version is incomprehensible, the environment is
  under-signalling.

### Overhead layout (provisional, 2026-10-23)

```
        ACTIVE RAILS  |  low fence / closed gate — do not cross
  ────────────────── PLATFORM ──────────────────  [clock pole]
  [baggage end] | [agent bay + ticket wicket] | [waiting room]
                | [public entrance — blocked] |
  [service niche, beside the entrance: oil can + note, in view]
  ────────────────── FORECOURT / GRAVEL ──────────────────
  ────────────────── DIRT ROAD ──────────────────
  east along the platform → traces of a former siding → retired lineside hut (later discovery)
```

Through-building desire: road → forecourt → blocked public entrance →
waiting room → platform. Opening the door makes the place traversable,
not just a room accessible. Heritage records inform this layout, they do
not dictate a single station design: Cranberry Portage (people and goods
moving through/beside), Lake Louise (sightline through a station you
cannot yet cross to the platform beyond), Toronto Cabin D (an
interlocking cabin is not evidence every rural stop had a switch house).
Our station stays small and fictional: no second-floor residence, no
Lake Louise scale.

### Sightline / access map (2026-10-23, from Mira's spatial challenge)

The waiting room is not the only physically plausible way to the
platform. It is merely the most satisfying way.

- See from the forecourt: south face, blocked public entrance, service
  niche, clock pole above the roofline (top, not face), and through the
  waiting-room windows a glimpse of light and a sliver of platform.
- Reach without the door: forecourt, both sides of the building, and a
  worn, overgrown exterior path around the baggage end to the platform's
  east end. From there: clock face, shutter, tracks — with a low fence
  and closed gate between player and ballast. A view, not a pleasant
  route; muddy, exposed, no interior.
- Enter only after the door repair: waiting-room interior, agent bay
  and ticket wicket from inside, and the sheltered through-route
  road → forecourt → waiting room → platform, with a new sightline
  straight from the forecourt through the open door to the platform.
- Active rails: never interactable, physical not magical — fence
  intact, gate closed, ballast beyond, no cross-track action, no signal
  or switch operation.
- First train from the forecourt: heard first, seen second — movement
  through windows and over the roofline, a blur not a spectacle. From
  the exterior side path, seen fully at the platform edge, behind the
  fence. What to notice is the station's stillness: train passes,
  clock does not move, shutter still taps, door still sticks.

### Believability principle (canon, 2026-10-23)

- The station should remain believable even if the player never fixes
  anything. Interactions reveal a place; they must not invent its
  architecture to justify themselves. Test every new room, tool, and
  obstacle against this: would this building still make sense if the
  player walked away and left it exactly as found?
- Securing the loose shutter is a separate, optional, by-hand action,
  not bundled with oiling the door and not required for the door payoff.
  Door payoff alone: hinge groan → smooth swing, latch catches, shaft
  of daylight, newly accessible interior. Prototype 1.3 will show this
  as animation (door shake on failed try, smooth swing, light shaft,
  shutter still tapping until secured), not just prose.
- Three-path test: door first, service niche first, or ignore both and
  explore outside — each understandable without reading the note. The
  note confirms, it does not unlock.

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

### The clock — second discovery, not first payoff (decided 2026-10-23)

- Door-first, clock-second. The first playable slice ends at the door
  opening. The clock remains stopped, visible, and compelling as the
  second discovery. Its repair must be earned by finding its actual
  mechanism, not just "wind it later."
- The clock is the exterior multi-faced clock on its pole above the
  platform, not an interior clock. It is the landmark the whole platform
  reads against.
- No documented small Canadian station example yet establishes our
  specific multi-faced exterior pole clock or its indoor winding
  arrangement, and a mechanism ticking inside an outdoor clock may not
  be audible across the whole platform. That is a research gap, not a
  license to say it existed. Do not force the clock as the first audible
  reward until mechanism and listening distance are earned.
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
- The first useful maintenance item is in a visible, station-side
  service niche beside the public entrance — oil can and mundane note,
  in the same view as the door. The note is not required. The retired
  lineside hut is a later discovery, not a prerequisite to entering
  the first room. The player never operates anything connected to the
  active railway.
- Discoverability without a quest marker or NPC: a continuous,
  weather-tied, local soundscape from arrival — a loose shutter tapping
  irregularly with wind gusts, the hinge groaning when tested, a strip
  of paper fluttering at the threshold. No fixed-timer hint, no second
  train. If a player still misses the door, that is a composition and
  sightline problem to fix in testing, not a louder hint.
- The one hard gate is spatial, not a key chain: the platform can't
  be reached through the building until the door is open. A room you
  can't enter yet is a question, not a locked quest step.

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

### Prototype 1.3 scope (updated 2026-10-23, from Mira's motivation challenge)

- Scene selector, not locomotion: forecourt / side path / platform /
  waiting room as illustrated viewpoints, before investing in movement.
- Door reward is a changed composition, not a shortcut: opening the
  door gives a new view and a new interior, with daylight revealing the
  ticket wicket, worn floorboards, and a trace of the caretaker. No time
  pressure, stamina, or wet penalty is invented to make "dry and direct"
  matter.
- Single interior discovery: wipe a circle clear in the grimed
  waiting-room window. A deliberate action, not a scrubbing simulator.
  Result: a framed view of platform, clock, and tracks from inside.
  Player can return to that window later; a later train is noticed
  from that vantage. No journal given away; grime itself is the trace
  of how long the room has been closed.
- Opening sequence as a test, not a mandatory script: forecourt →
  optional exterior path (stopped clock, platform, old station name
  sign with a missing letter — optional, never required, never
  punished) → door in either order → shutter independently optional →
  door opens to new view/interior, clock stays stopped → player who
  never repairs the door still appreciates the outside station.
- Early train is missable by design: no pausing, interrupting, or
  cinematic camera. Still clock + abandoned room carry the premise
  independently. Sound/vibration may naturally catch attention.
- Visual treatment: small, illustrated views built in the prototype
  (forecourt + interior reveal) with flat colour, light shaft, shadows,
  and readable spatial relationships — not an expensive art pass, and
  NOT photo-based references of a real station, to avoid implying a
  real station is our fictional station.

### Prototype 1.3 scope (next build, from 2026-10-23 discussion)

- Separate door and clock repairs in logic: door opens, clock stays
  stopped, clock repair marked as next. Add a Layout view with the
  overhead map above. Rename switch house → service niche + retired
  lineside hut throughout. Add visual shutter shift, paper flutter, and
  door shake, so muted play still signals the repair.

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
