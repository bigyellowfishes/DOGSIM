*Work in progress · grown from `gdd-template.md`*
*Doc: `▓▓▓▓▓▓▓▓▓▓` · full document written, sections 0 to 9 · still open: header facts, the wish hour, reminder channels, the test phone, and the creator's sign-off on the parts marked `[agent-decided]`*

# Pawsome Day Centre

**Decentraland Creator Success Program**

| | |
|---|---|
| Public experience title | Pawsome Day Centre · IP & [Content Policy](https://decentraland.org/content/) self-check: `TBD: the creator still has to check the names "Pawsome" and "doggidex"` |
| Deployment target | `TBD: not given yet` |
| Studio / team name | `TBD: not given yet` |
| Date | 2026-11-24 |
| Contact (Discord + email) | `TBD: not given yet` |

---

## 0. TL;DR

| | |
|---|---|
| **Player promise** | A cosy dog-adoption sim where you choose every pup's forever home, but a wrong match comes back to you. |
| **Primary player** | For players in Brazil, mainly women (men can play too), who already enjoy cosy pet and care games on their phone, arriving alone from Decentraland's Discover page, looking for a five-minute visit with a dog that knows them. `[agent-decided]` |
| **Current status** | Playable core loop in SDK7, built in Creator Hub: one corgi, eight pup actions, arrivals and adoptions working (a pup still leaves by itself when its hearts are full; needs, matching, the personal dog, the doggidex and the shared Park are not built yet). The Main Room, the Bathroom and the Park are built; Room 3 and Room 4 are empty. A dev menu can spawn, despawn and adopt a pup for testing. No playable link given yet. |
| **Requested round** | v0 (vertical slice) first, then v1 (4-week scope). |
| **Live at end of the round** | A player can run their own day centre at any hour: read each pup's needs, choose its home, keep a dog with a daily wish, fill the doggidex, and meet other carers' dogs in the Park for play-dates, live in our World. `[agent-decided]` |

---

## 1. Player Promise

**One-line promise.**

A cosy dog-adoption sim where you choose every pup's forever home, but a wrong match comes back to you. `[agent-choices ✓]`

---

## 2. First Minutes & How to Play

| Time | Player experience |
|---|---|
| **0–5 seconds after control** | You spawn in the Main Room, facing the arrivals kennel. The door slides open and a muddy, hungry pup runs in and stops in front of you, with a food bubble over its head. `[agent-choices ✓]` |
| **5–10 seconds** | You tap the pup. Its menu opens above its head and Eat is glowing. The goal is clear: give this pup what it needs. `[agent-choices ✓]` `[HYPOTHESIS H1-01]` |
| **10–60 seconds** | The pup eats from the bowl next to you and the first heart pops. A bath bubble appears; Follow and the Bathroom exit glow. You lead the pup to the splash pool for heart two. `[agent-choices ✓]` |
| **1–3 minutes** | A cuddle fills the last hearts. Three owner profiles appear by the adoption kennel. You pick one, the pup trots out under the bunting, and Adopted shows 1. `[agent-decided]` |
| **3–10 minutes** | A second pup arrives with different needs. Minutes after each match you learn how it went: settled in, or back at the door with less confidence. Your own card now sits among the owners: pick yourself and the pup stays. `[agent-choices ✓]` |
| **Natural stopping point** | Every match has had its answer. Your own dog's bed shows tomorrow's wish. `[agent-choices ✓]` |

**Player-facing How to Play.**

- Tap a pup and meet its needs `[agent-decided]`
- Full hearts mean ready: choose its home `[agent-decided]`
- Play-dates in the Park help both dogs `[agent-decided]`

---

## 3. Core Loop

| # | Step (verb) | What the player does (Player input → what they see or hear → what changes) | Why do it again? |
|---|---|---|---|
| 1 | Meet `[agent-choices ✓]` | The centre starts with one pup at a time; upgrades let it hold more, up to 5 at once (the creator's current thinking, not final). Upgrades come from the centre's star rating `[agent-choices ✓]`. The arrivals kennel door slides open and a pup runs in. You click the pup → an action menu opens above its head and its hearts bar appears → the pup is selected. | Every new pup is a new set of needs to read. `[agent-choices ✓]` |
| 2 | Care `[agent-choices ✓]` | Each pup arrives with a few visible needs that come from its traits: one is muddy, one is hungry, one is shy `[agent-choices ✓]`. You read the pup and pick the action it needs from its menu (such as Wash, Eat or Play), in any order → the pup does it, with hearts and speech bubbles → each need you meet adds a heart, and the pup gains confidence. Confidence is the process a pup goes through to get ready to be adopted. The hearts bar (5 hearts, called happiness in the build) shows it `[agent-decided]`. | Each need you meet adds a heart you can see and brings the pup closer to a home. `[agent-choices ✓]` |
| 3 | Lead `[agent-choices ✓]` | You press Follow → the pup trots after you through every room and up to the park → you press Unfollow to stop. A need can send you to another room: the bath for a muddy pup, the park for a restless one `[agent-choices ✓]`. | What the pup needs is in another room. `[agent-choices ✓]` |
| 4 | Match `[agent-choices ✓]` | A pup has the confidence to be adopted → you make the match from profiles of potential owners, and a pup can go to any home → the pup leaves through the adoption kennel and the Adopted counter goes up. If the home is not right, the pup may come back to you with less confidence, and you go through the process again. | A good match makes room for the next pup; a pup that comes back needs you again. `[agent-choices ✓]` |

| | |
|---|---|
| **One complete loop takes** | A loop ends when you match a ready pup with one of the potential owners and it leaves through the adoption kennel. A match that is not right can reopen the loop: the pup comes back. Target: a player can complete one loop in 5 minutes. That is longer than 90 seconds, so the earlier payoff is every heart; the first lands at about 15 seconds. `TBD: time it once needs and matching are playable` |
| **Decision, challenge, or expression** | Which home each pup goes to. Pups have traits and potential owners have profiles. Any pup can go to any home, so the choice is yours, and a match that is not right may come back. You can also keep one dog as your own pet: it always stays with you, and if the right owner comes up you can choose to let it be adopted. You keep a pup by picking your own card at the Match step `[agent-choices ✓]`. |
| **Shortest satisfying visit / typical session** | 5 minutes, one full loop / open-ended: a session can last as long as the player wants. |
| **Why repetition 10 differs from repetition 1** | Each pup arrives with different needs, because its traits differ, and the potential owners' profiles change too. So you have to read every pup and every match again. `[agent-choices ✓]` `[HYPOTHESIS H2-01]` |

**Pillars.**

1. Every pup gets a happy ending, in the end: setbacks yes, losses never. A pup can come back as many times as it takes; it is never taken away and there is no game over. `[agent-choices ✓]`
2. Overly cosy, pastel and cute.
3. The match is yours: any pup can go to any home, and the game never chooses for you. `[agent-choices ✓]`

---

## 4. Why Players Come Back

### 4.1 The next-day (D1) sentence

> "A player who enjoyed their first session returns the next day (D1) because Hook 2, their own dog, has a new daily wish at a fixed hour, and its bed shows tomorrow's wish before they leave." `[agent-choices ✓]` `[HYPOTHESIS H2-02]`

### 4.2 The progression chain

> **Repeatable action → persistent reward → new capability, status, or social role → new decision or challenge**

| Moment | What persists or has been built? | What becomes possible next? | How can another player tell? |
|---|---|---|---|
| **End of first session** | Your first doggidex stamps and, if you kept a pup, your own dog with "days together" at 1. `[agent-decided]` | Tomorrow's wish for your dog. `[agent-decided]` | Your dog walks with you in the Park, with its collar tag. `[agent-decided]` |
| **End of first week** | A star rating for your centre, about 13 of 20 stamps and 7 days together, if you make three matches a day (arithmetic, assuming breeds arrive at random). `[agent-decided]` | Stars have opened more kennels, so you care for several pups at once and choose which pup goes to which owner. `[agent-choices ✓]` | Your centre's stars show next to your carer's name in the Park. `[agent-decided]` |
| **Week 3+: what takes more than two weeks?** | Completing the doggidex. With 20 breeds arriving at random it takes about 72 successful matches, so three to four weeks at three matches a day (arithmetic). | The fifth kennel, and the full book. `[agent-decided]` | A doggidex ribbon on your dog's collar. `[agent-decided]` |

The centre has a star rating. Good matches raise it, and a pup that comes back lowers it a little. Stars unlock kennels, from one pup toward five. `[agent-choices ✓]` A kennel that is unlocked stays unlocked, so a lower rating is a setback and never a loss. `[agent-decided]`

You arrive and your dog is waiting by its bed with today's wish: a run in the park. Three pups are in the centre now, because your stars opened two more kennels. One is the beagle that came back on Tuesday, and today you find it a quieter home, which stamps entry 13 of 20. In the Park, another carer's dog wears a collar tag that says 21 days. `[agent-decided]`

Currency or tradable rewards: N/A. There is no currency; kennels unlock from the star rating.

### 4.3 Two return hooks

| Selected hook | Exact trigger or timing | What the player anticipates | Reminder channel + no-reminder fallback |
|---|---|---|---|
| **1.** Collection: the doggidex | An entry is stamped when a match sticks. A pup that comes back is not stamped until its next home works out. `[agent-choices ✓]` | Completing a big book of twenty or more breeds. `[agent-choices ✓]` | |
| **2.** Your own dog: the daily wish `[agent-choices ✓]` | One new wish each day (a run in the park, a bath, a nap by the window), changing at a fixed hour `[OPEN: waiting on picking the hour; the audience is in Brazil]`. Granting it adds a day to "days together". A missed day pauses the count and never resets it. | Tomorrow's wish, and a growing "days together" count on the dog's collar tag, which other players can see in the Park. | Fallback with no reminder: the dog's bed shows tomorrow's wish before you leave. |

The creator names a third reason to come back: to help other dogs. That is the core loop itself.

How you get your own dog: at the Match step your own card sits among the potential owners. Pick yourself and the pup stays. You can have one dog at a time, and the option appears from your second pup, about five to eight minutes into the first visit. Later your dog can appear in a match too, which is how you let it go to the right home. `[agent-choices ✓]`

---

## 5. Social by Design

| | |
|---|---|
| **The repeatable social loop** | Player A brings a dog to the Park and taps Player B's dog to offer a play-date → Player B taps to accept → the two dogs play and both gain hearts, and a shy pup gains confidence it cannot get alone → the friendship is saved: the dogs greet each other next time, and a daily wish can be "see my friend again", which is the reason to regroup. `[agent-choices ✓]` `[HYPOTHESIS H2-03]` |
| **The disappearance test** | Play-dates and dog friendships stop: "see my friend again" wishes cannot be granted and shy pups lose their fastest way to gain confidence. The centre, the matches, the doggidex and the rest of your dog's wishes carry on. `[agent-decided]` |
| **From strangers to a group** | Everyone in the Park is a carer with a dog, so there is one role. A dog that wants to play shows a bubble, and you tap it. No voice or shared language is needed. `[agent-decided]` |
| **Recognition & continuity** | Every player is a chibi carer they can dress, with a few choices such as hair and jumper colour `[agent-choices ✓]`. A name shows over each carer in the Park, next to the centre's stars `[agent-decided]`. Dog friendships persist: friend dogs greet each other the next time they meet, and a daily wish can ask to see a friend again. |
| **Quiet hours & player counts** | Players meet in the Park: every player who goes there can see all the other players there. When few people are online, a solo player can play everything, and a resident Park dog offers play-dates so no pup ever waits for another player. Social play becomes viable at 2 players; the ideal group is 4 to 6; the v1 tested maximum is 10 players. The daily wish often sends dogs to the Park, so players who are online at the same time pass through the same small lawn. `[agent-choices ✓]` |
| **Drop-in / drop-out** | A player who arrives late can offer a play-date at once. If a partner leaves halfway, your dog keeps the hearts it earned and the resident Park dog finishes the play-date. Saying no costs nothing. Each dog can receive one offer at a time, and no other player can touch anything inside your centre. `[agent-choices ✓]` |
| **Visible play (the bystander test)** | You see carers walking their dogs across a small lawn, and two dogs chasing each other while their carers watch. `[agent-decided]` |
| **Shareable play (the memorable moment)** | The graduation: a pup you cared for trots out under the bunting to its new family, and its stamp lands in your doggidex. `[agent-choices ✓]` |
| **Bring-a-friend** | When your dog's wish is "see my friend again", you want that one player in the Park. Once they arrive, the two dogs run to greet each other and the wish is granted for both of you. `[agent-decided]` |

---

## 6. Mobile-First

**Every core-loop verb on touch.**

The whole game is point and click: one click per action. On touch, each click is one tap `[agent-decided]` `[HYPOTHESIS H2-04]`. Built and tested on desktop only so far.

| Core-loop verb | How it works with touch controls |
|---|---|
| Meet | Tap the floor to walk. Tap the pup to open its menu. |
| Care | Tap the action the pup needs. |
| Lead | Tap Follow, then tap where to walk. Tap the glowing exit to change rooms, and step on the arrow tile to reach the Park. |
| Match | Tap one of the owner profile cards, or your own card to keep the pup. |

**UI plan.**

Small screen first: the camera has four on-screen buttons in a corner (rotate left, rotate right, zoom in, zoom out), so phones keep the orbit `[agent-choices ✓]`. The pup's actions open as large buttons within thumb reach `[agent-decided]`. Built so far on desktop: Arrived and Adopted counters, a hearts bar while a pup is selected, and the action menu above the pup. The dev menu is for testing only.

**Performance.**

Target: 60fps on recommended desktop hardware and 30fps on a named phone in the mobile client, both at 10 players, our v1 tested maximum. `TBD: the test phone is not named yet` The biggest risk is the Park at its maximum: 10 carers and 10 dogs, all animated at once. Plan: a player's centre shows only their own pups, and the Park shows one dog per player plus the resident dog. `[agent-decided]`

**Desktop-only dependencies.**

Two, both in the camera: zoom on the W/S keys and orbit by dragging. Decentraland's mobile documentation (checked 2026-11-24) lists the mobile client as touch only, with no keyboard shortcuts and no drag or swipe gestures. The on-screen camera buttons replace both, so nothing in the loop needs them. The scene also runs its own cameras, hides the player's avatar and works out taps with its own ray picking; the documentation does not say whether these work on mobile. `TBD: check the current build on a phone with the Creator Hub QR code` Names over carers will be our own text labels, because the platform's name tag component is listed as missing on mobile.

---

## 7. World, Look & Story

**Story / world.**

You run a snug little day centre for dogs waiting for a forever home. You look after each pup until it is happy and ready, then wave it off to its new family.

**Visual direction.**

A little isometric diorama: four rooms in a ring around the building's centre, one visible at a time, with a park above. Simple and clean, in flat single colours with no busy textures, and a pastel palette of mint, coral, lavender, pink and butter yellow. You play a chibi day-centre carer (not a vet): hair in buns with pink bows, a butter-yellow jumper and a mint apron with a pink heart. The two kennels show where pups come and go: arrivals on the left wall (mint with a coral roof, a "Welcome" mat) and adoptions on the right wall (lavender with a mint roof, graduation bunting, a "Goodbye" mat).

Our signature shot is the two doors: the whole cut-away room in one frame, with the mint Welcome kennel on the left, the lavender Goodbye kennel on the right, and one pup between them with the carer. `[agent-choices ✓]`

`[OPEN: waiting on a phone check for small-screen readability]`

---

## 8. Audience & Comparables

**Primary player + arrival context.**

For players in Brazil, mainly women (men can play too), who already enjoy cosy pet and care games on their phone, arriving alone from Decentraland's Discover page, looking for a five-minute visit with a dog that knows them. `[agent-decided]`

**How the first group arrives.**

The first players come from Decentraland's own Discover page: we list the World well and let players find it `[agent-choices ✓]`. We do not count on players overlapping: everything is playable alone, the resident Park dog covers play-dates, and two players are enough for social play to start. `[agent-decided]`

**Deliberately not for.**

Players who want competition, combat or a score to beat: nothing here can be won or lost. `[agent-decided]`

### Comparables

| | Comparable A, outside Decentraland: To The Rescue! | Comparable B, outside Decentraland: Nintendogs |
|---|---|---|
| What we observed works | Adopters come in wanting specific things, and you match dogs to them. Every dog has its own traits. The look is pastel and friendly. `[agent-decided]` | Care is direct: you pet, wash and play with the dog yourself and it reacts at once. Dogs never grow old or die, so it stays gentle. Short visits are enough. `[agent-decided]` |
| What does not fit our audience or context, and why | It turns into busy shelter management: money, disease, staff and many dogs at once. Reviewers called it hectic and stressful, and a dog can be sent away. That fights "cosy" and "losses never". `[agent-decided]` | The dogs are yours forever. Nothing ends, so there is no goodbye and nothing to match. It is a private, solo game built for its own hardware. `[agent-decided]` |
| What we will do differently | No money, no admin and no loss: one to five pups in a small diorama. A wrong match is not a failed sale; the pup comes back to you. `[agent-decided]` | The pups are not yours. You get each one ready and let it go, and you may keep just one. `[agent-decided]` |

---

## 9. 4 Week Plan (v1 scope)

| Week | What is playable / done |
|---|---|
| 1. Prototype definition | Needs and traits working on the corgi. Matching with owner profiles tested on paper, then in the build. One new breed built and timed. `[agent-decided]` |
| 2. Core interaction + first-group test | The full loop works alone from end to end: Meet, Care, Lead, Match, pups that come back, the star rating. A basic Park where two players can offer and accept a play-date. Playtest at 2 players, our social threshold. `[agent-decided]` |
| 3. Core systems refinement | Your own dog, the daily wish and "days together". Doggidex stamps that save. Kennel upgrades. Carers you can dress. More breeds. `[agent-decided]` |
| 4. Playable prototype, final design direction (mobile playtest) | Camera buttons and large action buttons. Phone playtest with up to 10 players in the Park. Saved dog friendships. The remaining breeds. Final look locked. `[agent-decided]` |

**What keeps the experience changing after launch.**

- Without building a new level, we can change or rotate which breeds arrive and the pool of daily wishes every week. `[agent-decided]`
- If an update is skipped, random needs, random owner profiles and the daily wish still create variation. `[agent-decided]`
- N/A: nothing resets, and progression gives no advantage over another player. `[agent-decided]`
- One player behaviour that would change what we build next: if players keep a dog but never visit the Park, we bring play-dates to the centre's front door. `[agent-decided]`

**Not building in v1.**

Nothing is held back: the creator plans the whole design for v1, including all twenty or more breeds, carers you can dress and saved dog friendships.

**Top risk + fallback.**

Top risk: the twenty breeds. Nineteen new breeds at about 4 hours each is about 76 of the roughly 180 hours planned across the four build weeks, which makes them the largest single item, and the 4 hours is an untested estimate. `TBD: time one breed in week 1 to replace the estimate` Fallback: if a breed takes longer, v1 launches with fewer breeds and the rest arrive a few at a time after launch, shown as silhouettes in the doggidex until then. `[agent-decided]`
