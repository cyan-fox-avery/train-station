# Prototype 1 — notes for review

Scope, from PR #1: one platform view, one waiting-room interior, a passing
train, one environmental clue, one small repair, and a persistent
audible/visual consequence.

What is in this prototype:
- Platform: stopped exterior clock, ivy-draped waiting-room door, faded
  timetable, switch house, track.
- One train, early (about 12 seconds after load), passing once only.
- Try the door: a seized hinge sounds and behaves differently from a
  locked door; debris at the threshold is visible in the text.
- Switch house: oil can on an open shelf, plus the mundane caretaker note
  about the sticking door. That note names the hinge, not the solution.
- Wander the platform: weather-tied soundscape notes, paper, drainage.
- Repairs, in either order: free the hinge (needs the oil can), clear
  the threshold by hand. At most one found tool in this loop.
- Payoff: door opens, waiting-room interior opens, exterior clock starts
  ticking (Web Audio tick + moving hands), heard from the platform.
- Waiting room: faded arrivals board, dusty lost-and-found shelf, and a
  maintenance notice pointing to drainage — the next loop, not built here.
- Preserve some age as a choice: leaving the arrivals board faded is
  recorded, not scored as neglect.
- Progress persists in the browser (localStorage) until Reset.

Deliberately not in Prototype 1:
- No inventory economy, no branching ending interface, no second train,
  no journal fragments, no drainage repair, no locked clock mechanism.
  The clock sound is a tick for now; the mechanism is provisional
  (mechanical tick vs. impulse click) pending small-Canadian-station
  research, as agreed in PR #1.

What to test:
- Did you notice the problem without being told?
- Did trying the door make sense?
- Did you want to look around afterwards?
