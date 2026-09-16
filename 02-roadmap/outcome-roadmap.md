# Outcome Roadmap & Trade-off Memo: Meridian

> Module 2 · Prioritization & Roadmapping for Product Leaders, ★ Deliverable 2
>
> Translate your strategy into a multi-team, outcome-driven roadmap, and a memo defending the hard prioritization calls behind it.

## 1. Outcome roadmap

_A multi-team roadmap organized by **outcomes**, not feature lists. Show how near-term revenue pressure is balanced against long-term platform bets._

### Now (0–3 months) — three bets, one question

Every Now item tests the same wager: **field non-adoption is an effort problem, and removing effort moves usage.** If that wager is wrong, all three are cheap enough to have been worth running anyway.

| Horizon | Outcome / bet | Owning team(s) | Success signal |
|---|---|---|---|
| Now (0 to 3 mo) | **We bet that cutting the daily log from 14 required fields to 4 will get a complete log filed before the truck leaves the gate, for foremen closing out a shift.** The wager: the form kills the log, not indifference *(Rock #1 · KR1, KR3)* | Field Capture (eng + design), PM | Log completion rate on pilot projects ≥ 70%; median observation-to-record under 4 hours by month 3, en route to 10 minutes |
| Now (0 to 3 mo) | **We bet that letting a foreman mark up the photo he already took will turn the camera roll into the record, for field teams documenting an issue.** The wager: the phone camera is our real competitor, and we win by absorbing it *(Rock #2 · KR2, KR3)* | Field Capture (eng + design) | ≥ 40% of photo documentation on pilot projects originates in-app rather than camera roll |
| Now (0 to 3 mo) | **We bet that pushing schedule changes to the phone will create the unprompted return visit, for superintendents and foremen planning tomorrow.** The wager: weekly-active is won by the return visit, not the first *(Rock #3 · KR1)* | Platform (notifications), Field Capture | Field-role weekly active 8% → 25% on pilot projects; ≥ 30% of sessions originate from a notification |
| Now (0 to 3 mo) | **⚑ Not a bet — the test. We learn whether the barrier is effort or exposure.** All three bets above wager on effort. Two weeks, three active projects, shadowing superintendents. Runs *in parallel* with the bets, not after | PM (lead), Research | A written verdict by week 3 that either confirms the effort hypothesis or reframes the roadmap from Next onward |

### Next (3–6 months) — sequenced behind the evidence

| # | Outcome / bet | Owning team(s) | Why it comes after Now |
|---|---|---|---|
| 1 | **Capture works for a foreman who is not at a desk and not on wifi** *(backlog #1 + #7, merged)* | Field Capture, Platform | The single largest bet on the board, and the one the evidence gate governs. Offline-first is architectural, so it must precede the dedicated app rather than be retrofitted — but neither starts until we know a foreman *wants* to file at all. |
| 2 | **A spoken observation becomes a correctly-typed record without a foreman choosing the type** *(backlog #9)* | AI/Ontology, Field Capture | This is the M1 moat — the construction ontology. It is only defensible once there is real field capture volume to train and validate against, which the Now bets create. |
| 3 | **A superintendent can see field activity across their projects without asking for a report** | Platform | The narrowest possible read surface, scoped to the *field* manager, not the exec. Serves the M1 management system (weekly field activation review, cohorted by superintendent) without reopening the reporting hard no. |
| 4 | **The renewal conversation is held on adoption evidence, not on a dashboard** *(the #10 answer)* | PM + exec sponsor, CS | The two at-risk renewals are real and dated. This is handled with a named exec sponsor and a committed date, not with engineering capacity — but it must be actively worked in this window, not deferred. |
| 5 | **Two clients stop losing data at the Procore boundary** *(backlog #8)* | Platform | Genuine breakage, genuinely small. It is a Fill Gaps item: it happens in the slack once the Rocks are moving, and never ahead of them. |

### Later (6–12 months) — bets, not commitments

_Each of these is strategically right and none is resourced. They are listed so they stop being re-litigated every quarter._

| Outcome / bet | Status |
|---|---|
| **The record becomes protective for the foreman, not just legible to the firm** — if the evidence gate returns "exposure", this is not a Later item, it becomes the strategy | Contingent bet — promoted immediately if the field study reframes the diagnosis |
| **Compliance obligations are met as a by-product of field capture rather than a separate workflow** *(backlog #5)* | Bet. Only viable once the ontology is reliable; depends on Next #2. |
| **The back office reads the field record without the field feeling watched** *(backlog #3, #10)* | Bet. Gated by the M1 hard no through Q3 2027. Data-model work is deliberately *not* started early: doing it quietly does not change what it enables. |
| **Subcontractors join the record instead of sitting outside it** *(backlog #14)* | Bet. Deliberately out of Where-to-play until field adoption clears 60%. |
| **Time and labour are captured from the same utterance as everything else** *(backlog #12)* | Bet, and the most exposure-sensitive item on the board. Revisit only after trust is demonstrably earned. |

_[screenshot or shareable link to your roadmap visual]_

## 2. Trade-off memo

_What did you sequence first, what did you push out, and what did you cut entirely, and why? Use WSJF / cost of delay reasoning where it helps._

> **I chose to sequence the three cheap field-capture bets first** because they share one hypothesis, cost roughly one team-quarter combined, and are each reversible. On WSJF terms they are unremarkable in value but exceptional in job size: Rock #1 alone is Impact 5 / Effort 1 after the reality check. Nothing else on the board returns that ratio, and the three together buy a falsifiable answer to the question the whole strategy rests on.
>
> **I pushed out the two large mobile bets — offline-first (#1) and the dedicated foreman app (#7)** — because both assume the barrier to field adoption is that mobile does not work well enough on site, and that assumption is not yet evidenced. My M1 pressure-test produced a competing explanation: foremen may avoid the record because it exposes them, not because the signal drops. I am not willing to spend a quarter of platform engineering to harden a channel before I know anyone wants to use it. The asymmetry decides it — if the field study says connectivity, I have lost two weeks; if it says exposure, I have saved a quarter. This is the call I would most expect to be challenged on, because #1 came from my own field research, and rejecting it means trusting that research about *what* foremen do while doubting it about *why*.
>
> **I cut the executive reporting dashboard (#10), time-tracking (#12) and the subcontractor portal (#14) entirely for this horizon** because all three serve the buyer rather than the user, and my M1 hard no says exactly that: no new analytics, reporting or ERP integration work for four quarters. #10 carries genuine dated cost of delay — two renewals at risk — and I am still saying no, because it would report on data that does not exist yet: a dashboard over 8% adoption is a dashboard of an empty job site. That cost is real but survivable, and it is answered with an exec sponsor and a committed date rather than with four engineers. #12 is worse than a distraction: building a stopwatch for foremen in the quarter I am asking them to trust the record would actively work against KR1.

## Link to full artifact

_[link to this deliverable in your repo]_
