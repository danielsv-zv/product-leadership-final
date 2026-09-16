# Prioritization & Roadmapping, Module 2 Lab

## How I scored (Impact vs Effort)

North star for Impact: **KR1 — weekly active field-role usage, 8% → 60%**. Impact is not "is this valuable"; it is "how many foremen open the app on a workday because of it".

The table below shows the adjusted numbers, ordered based on the KR's and following my North Star.

| # | Backlog item | Impact | Effort | Quadrant |
|---|---|---|---|---|
| 4 | Simplify daily log: 14 required fields → 4 | 5 | 1 | **Do Now** |
| 2 | Photo markup and annotation for field teams | 4 | 2 | **Do Now** |
| 11 | Push notifications for schedule changes | 3 | 1 | **Do Now** |
| 7 | Foreman-facing mobile app, separate from PM web | 5 | 5 | Plan Carefully |
| 9 | AI-assisted RFI drafting | 4 | 4 | Plan Carefully |
| 10 | Executive reporting dashboard, custom KPIs | 1 | 4 | Plan Carefully |
| 3 | Migrate data model for multi-project dashboards | 1 | 4 | Plan Carefully |
| 8 | Fix broken Procore import/export (2 clients) | 1 | 2 | Fill Gaps |
| 6 | Real-time weather data in scheduling | 1 | 2 | Fill Gaps |
| 13 | Web UI refresh ("looks outdated") | 1 | 3 | Avoid |
| 5 | Automated compliance checklist generator | 2 | 4 | Avoid |
| 1 | Offline-first mobile for poor connectivity | 4 | 4 | **Hard No** |
| 12 | Time-tracking module | 1 | 5 | **Hard No** |
| 14 | Subcontractor portal with document sharing | 1 | 5 | **Hard No** |

The four quadrants, and what each one means as a decision:

- **Do Now = Rocks.** High impact, low effort. These get named people and start immediately. If everything is a Rock, nothing is.
- **Plan Carefully.** High impact, high effort. The matrix does not decide these — **strategy does**. They get evaluated against the OKRs and sequenced deliberately, never started casually.
- **Fill Gaps.** Low impact, low effort. Real but small. They happen *after* the Rocks are moving, in the slack, and never before.
- **Avoid = Hard No.** Low impact, high effort. Say it out loud and write down why, so it does not come back next quarter wearing a different name.

## Prioritize your Rocks and your Hard Nos
- **Rock #1:** **Simplify the daily log — 14 required fields down to 4.** Impact 5, Effort 1. The highest-leverage item on the board: it removes the single biggest reason a foreman abandons a log mid-entry. It costs almost nothing and it serves KR1 and KR3 directly.
- **Rock #2:** **Photo markup and annotation for field teams.** Impact 4, Effort 2. The foreman already takes the photo — the phone camera is the competitor. This makes the photo *do the explaining*, which is the fastest path to "talk and photograph" capture without waiting on the full mobile app.
- **Rock #3:** **Push notifications for schedule changes.** Impact 3, Effort 1. The only item that gives a field user a reason to open Meridian when they were not already planning to. It creates the return visit that weekly-active measurement depends on, and it is what the superintendents explicitly asked for.
- **❌ Hard No #1:** **Offline-first mobile experience for poor-connectivity job sites (#1).** Impact 4, Effort 4 — and note that I am killing something I scored as genuinely high-impact. That is the point: this is not a low score, it is a **bet I have not earned the right to make**. The item assumes the barrier to field adoption is that mobile does not work well enough on site. That assumption is unvalidated, and my M1 pressure-test produced a competing explanation — foremen may be avoiding the record because it exposes them, not because the signal drops. Offline-first is a quarter of platform engineering spent hardening a channel I cannot yet prove anyone wants to use. If the two-week field study says connectivity is the blocker, this becomes a Rock immediately and I will have lost two weeks. If it says exposure, I will have saved a quarter. That asymmetry is the whole argument.
- **❌ Hard No #2:** **Time-tracking module (#12).** Impact 1, Effort 5. Three contract negotiations want it, which makes it a *sales* Rock, not a product one. It is a second product with its own payroll and compliance surface area — and it is the most surveillance-shaped item on the board. Building a stopwatch for foremen in the same quarter I am asking them to trust the record would work directly against KR1.
- **❌ Hard No #3:** **Subcontractor portal with document sharing (#14).** Impact 1, Effort 5. It expands *who* we serve before we have won the users we already have. Where to play says superintendents and foremen; subcontractors are a different segment with a different buying motion. Revisit once field adoption clears 60%.

## Show and swap
- **Do the Rock selections feel traceable to a clear strategy, or do they read like a feature list?:** Traceable. All three Rocks answer one question — *does a foreman open this app on a Tuesday?* — which is KR1 stated plainly. The tell is what they have in common: none of them serve the buyer. The buyer asked for #10, #12 and #14, and not one of those is a Rock. A feature list would have included at least one, because a feature list is what you get when you prioritize by who is asking rather than by what you are trying to move. The Hard Nos make the same point from the other direction, and one of them makes it uncomfortably: #12 and #14 are sales asks, but **#1 came from my own field research**. Saying no to a request is easy. Saying no to my own evidence — because I cannot yet tell which of two readings of it is true — is the call I would actually have to defend in the room.
- **Pick one Hard No and make the case for why it should actually be a Rock.:** **#1, offline-first mobile.** The honest case is the strongest one on this page. It came from *field research* — the same source as the insight driving my entire strategy, so I am selectively trusting my own evidence: I believe the research when it tells me foremen avoid the app, and disbelieve it when it tells me why. Construction sites genuinely do have poor connectivity; this is not a hypothesis, it is a physical fact about basements and steel frames. And there is a sequencing trap: offline-first is an architectural property, not a feature. It is far cheaper to build it in now than to retrofit it into #7 in two quarters, so "wait for evidence" may really mean "pay triple later". **Why I still say no:** connectivity is necessary but not sufficient. A foreman with perfect offline sync who does not want to file the record still does not file it. Offline-first only pays off *after* someone wants to use the product on site, and that is precisely what I have not proven. I would rather buy the answer for two weeks of research than a quarter of platform work — and if the answer is connectivity, I lose two weeks and gain conviction.

## Review and refine
- **Does every Now item read as a strategic bet, or does it sound like a feature description?:** Now, yes, but only after rewriting them. The backlog handed me three feature descriptions ("simplify the daily log", "photo markup", "push notifications"), and each one had to be restated in the form *we bet [action] will [outcome] for [who]* before it belonged on a roadmap: *we bet that cutting the daily log from 14 fields to 4 will get a complete log filed before the truck leaves the gate, for foremen closing out a shift*; *we bet that letting a foreman mark up the photo he already took will turn the camera roll into the record, for field teams documenting an issue*; *we bet that pushing schedule changes to the phone will create the unprompted return visit, for superintendents and foremen planning tomorrow*.
- **Can you trace every Now item back to one of your OKRs?:** Yes, and I tried to make the mapping deliberately narrow: every Now bet serves KR1, because a roadmap where each item points at a different KR is three roadmaps. *Log before leaving the site* → KR1 (removes the abandonment point) and KR3 (most of the 26-hour lag is a log the foreman postpones because it is too long). *Photo becomes the record* → KR2 (capture originating from a field device) and KR3. *A reason to open it unprompted* → KR1, converting one-time users into weekly-active ones.
- **If someone who had never seen your strategy read the Now column, would they know what problem you are solving this quarter?:** Yes, and the column is legible as much for what is absent as for what is present. A stranger reads three bets about logs, photos and phone alerts, and one research gate (with no dashboard, no reporting, no integration, no new segment anywhere in the column). The only available conclusion is that we are trying to get the people on the job site to use the product, and that we are not yet certain why they do not. That second half matters: a Now column containing an explicit evidence gate tells the reader we know which assumption we are standing on.


## Save your roadmap
- **Where did you save your roadmap? (link or file):** Three places in this repo, each serving a different reader:
  - **Visual roadmap (the deliverable):** [`02-roadmap/roadmap.html`](./roadmap.html) The Now/Next/Later board with the OKRs, the three bets, the evidence gate and the Hard Nos on one page.
  - **Written roadmap + trade-off memo:** [`02-roadmap/outcome-roadmap.md`](./outcome-roadmap.md) — the same roadmap with owning teams and success signals per item, plus the memo defending what was sequenced, pushed out and cut.
  - **Working notes (this file):** [`02-roadmap/plc-m2-lab.md`](./plc-m2-lab.md) — the Impact/Effort scoring for all 14 backlog items and the reasoning behind each Rock and Hard No.
