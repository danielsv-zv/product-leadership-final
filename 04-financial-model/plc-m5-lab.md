# Master Product Financials & Strategic Bets, Module 5 Lab

## Make your evaluation and funding decision
- **What assumption is doing the most work? If this number is 20-30% off, what changes?:** The Standard-to-Enterprise upsell rate lifting from 6% to 8%. A 20–30% miss on upsell puts it at 5.6–6.4%, at or below the 6% baseline, which means zero incremental ARR and no payback on a $180,000 build. The case doesn't degrade, it disappears
- **What is the structural problem in this case? Look past the headline numbers for something that does not hold up on closer inspection.:** The case treats the full $28,000 Enterprise contract as incremental ARR, but an upsold account was already paying for Standard. The incremental figure is the delta between tiers, not the Enterprise price, so the $896,000 headline is overstated by 400 accounts' worth of existing revenue that the case never subtracts.
- **Is the kill criterion complete and actionable? Does it name the consequence, or hand the decision back to the room?:** No. It names a metric, a threshold (7%) and a date (end of Q3). In addition, the consequence is soft: "paused" isn't stopped, as it says "reallocated before headcount is committed" reallocates capacity nobody had committed yet, and no one is named as the decider.

The threshold also can't fire cleanly. Baseline is 6%, target 8% (killing at 7% lets the feature survive at half the lift it was funded for) and payback of 2.4 months doesn't hold at 7% on the same $180,000 build. And end of Q3 is two quarters post-launch, so the call arrives after the money is spent and the sunk-cost argument is strongest.
- **Your verdict: FUND / FUND WITH ONE CONDITION / DO NOT FUND. If a condition, name it; otherwise explain in one sentence.:** FUND WITH ONE CONDITION: Rebuild the case on real incremental ARR (the Standard-to-Enterprise delta, not the full $28,000) with the 12% churn actually applied and the AI layer's running costs included, then reset the kill criterion against those numbers so it fires before the money is gone: 7.5% checkpoint at 90 days post-launch, hard cut at 7% by end of Q2, engineers back to Field Capture, remaining budget released, product lead decides without a review meeting.

It's one condition, not two: you can't set an honest threshold on an inflated number. I'd fund it because 32 upsells across 400 Standard accounts is achievable and $180,000 is a small build against that upside.

## Write your business case
- **The strategic bet. What specific outcome are you backing, who does it serve, and what is the mechanism that connects the product decision to a financial result?:** Removing the biggest reason a foreman abandons a log mid-entry: 14 required fields down to 4. It serves the foremen, but the money is at the firm — the GC is who pays and who churns. The mechanism is that when the log actually gets filed, the field data reaches the office, the firm stops losing it, and that's what reduces churn, extends customer lifetime and maximizes LTV.
- **The assumptions. List the assumptions your case rests on, then rank them: which one, if wrong, most changes your conclusion?:** 1. Foremen don't complete the log because it's too long, not because they don't want to be on record. 
2. Log completion on pilot projects goes from 23% to 70% within 90 days.
3. Field data arriving reliably retains one at-risk account per year: $250k ACV against a $60k build.
4. The build stays a one-off $60k with no recurring cost (no added infrastructure, no support load). Removing form fields is the cheapest item on the board to run, which is why payback lands inside the first retained renewal rather than across a full year.

Number 1 is the one that most changes my conclusion: If the barrier is exposure, completion stays flat, no account is retained, and the $60k build returns $0. Every other assumption degrades the case; this one deletes it.
- **The expected return. What does the bet generate and when? Express it at unit level (per customer) and at scale (what volume hits target).:** Unit level. One retained enterprise account is $250k of ARR that would otherwise have left. No incremental COGS so effectively all of it drops through. Against a $60k one-off build, breakeven is 0.24 accounts.

At scale. 38 top-100 accounts, 8% logo churn, so roughly 3 at risk in a year. Retaining one of the three returns $250k on $60k, a 4.2x return in Year 1; retaining two returns $500k. Field-seat expansion inside the retained accounts is upside I'm not counting, because pricing isn't my call.
- **The kill criterion. Name the specific metric, threshold, timeline, and financial consequence that tells the team to stop. Actionable, not a conversation.:** If log completion on the 25 pilot projects has not reached 45% by 60 days post-launch, we stop. The four engineers move back to the Now Rocks the same week, the remaining Field Capture budget for the quarter is released, and the $60k is written off rather than defended with a second iteration.

## Stress-test and finalize
- **Paste your finalized business case here.:** The strategic bet. Removing the biggest reason a foreman abandons a log mid-entry: 14 required fields down to 4. It serves the foremen, but the money is at the firm — the GC is who pays and who churns. The mechanism is that when the log actually gets filed, the field data reaches the office, the firm stops losing it, and that's what reduces churn, extends customer lifetime and maximizes LTV.

The assumptions, ranked.

Foremen don't complete the log because it's too long, not because they don't want to be on record.
Log completion on pilot projects goes from 23% to 70% within 90 days.
Field data arriving reliably retains one at-risk account per year: $250k ACV against a $60k build.
The build stays a one-off $60k with no recurring cost (no added infrastructure, no support load). Removing form fields is the cheapest item on the board to run, which is why payback lands inside the first retained renewal rather than across a full year.

Number 1 is the one that most changes my conclusion: if the barrier is exposure, completion stays flat, no account is retained, and the $60k build returns $0. Every other assumption degrades the case; this one deletes it.

The expected return.

Unit level. One retained enterprise account is $250k of ARR that would otherwise have left. No incremental COGS, so effectively all of it drops through. But a $250k renewal turns on switching cost, integrations, procurement and the relationship as well as field adoption, so I state the return in attribution bands rather than claiming the whole contract:

Attribution of the renewal to field adoption	Value per retained account	Return on a $60k build
100%	$250k	4.2x
50%	$125k	2.1x
25%	$62.5k	1.04x

It survives at 25%. That is the number I'll defend: even if field adoption is only a quarter of why the account stays, the bet pays for itself inside Year 1.

What moves me between bands: the renewal debriefs on the two named at-risk accounts, and whether "our field teams don't use it" appears as a stated objection. If it's cited as a primary reason in either, I move to the 50% band; if it's absent from both, I drop to 25% and the bet is judged on payback alone.

At scale. 38 top-100 accounts, 8% logo churn, so roughly 3 at risk in a year. At 50% attribution, retaining one returns $125k on $60k and retaining two returns $250k. Field-seat expansion inside the retained accounts is upside I'm not counting, because pricing isn't my call.

The kill criterion. If log completion on the 25 pilot projects has not reached 45% by 60 days post-launch, we stop. The team moves back to the Now Rocks the same week, the remaining Field Capture budget for the quarter is released, and the $60k is written off rather than defended with a second iteration. Product lead decides on the data, no review meeting.
