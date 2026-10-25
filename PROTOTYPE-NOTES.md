# Prototype 1.3 — notes for review

Scope, from PR #1: stop designing 1.3 in the abstract and build the
playable slice, then judge it by playing it. Scene selector, not
locomotion. No second restoration, no journal fragment, no clock
machinery.

What is in this prototype (v0.1.3):
- Four scenes, one geography, one weather: Forecourt, Side path,
  Platform, Waiting room. Clock position, roofline, platform, window,
  light direction, and the train's path do not rearrange between scenes.
  Side-path views are ground-level, not a top-down map.
- Fixed light: one overcast afternoon, one direction. The door reveals
  soft daylight that was already there — a soft spill, not a sunbeam,
  and no time-of-day variation.
- Door first, clock second, separated in logic: door opens after
  clearing the threshold (by hand) and freeing the hinge (oil can from
  the service niche, beside the entrance, in full view), in either
  order. The note helps and never gates progress. The clock stays
  stopped throughout — opening the door does not start it.
- See / reach / enter: forecourt glimpse through the waiting-room
  windows, an overgrown exterior path around the baggage end to the
  platform's east end, and the interior plus sheltered through-route
  only after the door opens. The door is the most satisfying way, not
  the only way. Active rails are fenced, gated, and never interactable.
- Three arrival orders work: door → niche, niche → door, exterior
  path → return → door.
- Shutter latch is its own action, on the platform, by hand. Tapping
  stops only if the player latches it — it does not silently happen
  when the door opens.
- Window wipe is the single interior discovery, optional and
  persistent until Reset: one tap wipes a circle in interior dust and
  soot, revealing a framed view of platform, fence, rails, and the
  clock face off-centre. The rest of the pane stays aged, the outside
  glass stays weathered. Leaving the dust alone is not playing
  incorrectly. The chair sits slightly askew by the window, with a worn
  sill — evidence of habit, not proof of whose habit. Neither is
  clickable, and the chair goes first if it reads as staged.
- Discoverability, not pixel hunts: in-scene affordances visible
  before interaction (handle, latch, niche opening, dusty pane), plus
  a reachable contextual action control where needed. One tap performs
  the action. Focus/hover labels are clarification only, never the
  sole invitation. Buttons are 44px or larger, log sits above the
  actions, and muted play works — every change is visible, not just
  heard.
- First train: passes once, after the first tap, engine first heading
  left. It can be missed without breaking anything. It is punctuation,
  not a gate. The clock does not move when it passes.
- Preserve some age: leaving the arrivals board faded is recorded,
  not scored as neglect.

Regression check (old Prototype 1 behaviours that must be gone):
- Clock does NOT start when the door opens.
- The niche is NOT called a switch house. The retired lineside hut is
  a later discovery, not a prerequisite.
- Shutter and wipe are optional and separate, not bundled with the door.

Deliberately not in Prototype 1.3:
- No locomotion/map simulation, no inventory economy, no branching
  ending interface, no second train, no journal fragments, no drainage
  repair, no clock mechanism or winding, no second major restoration.

What to test:
- Can you find the door, the niche, and the side path without being told?
- Does opening the door change how the place feels, not just what rooms you can enter?
- Did you notice the train, or miss it, and did that matter?
- What did the build make awkward, or unexpectedly compelling?

Progress persists in the browser (localStorage) until Reset.
