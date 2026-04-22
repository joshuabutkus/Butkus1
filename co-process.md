# ALPINE CO PROCESS — CHANGE ORDER APPROVAL AND CONTINGENCY MANAGEMENT
*Last Updated: 26_04_22*
*Part of Alpine Professional Operating System — see system-state.md for system identity.*
*Update this document after every session that touches CO approval, contingency management, Formula C, or budget structure.*

---

## 1. CO FRAMEWORK OVERVIEW

This document governs Alpine's change order approval authority and contingency management process. The framework applies independently to hard cost and soft cost budgets, each tracked separately with their own contingency. Its purpose is to define the PM's delegated approval authority in a way that is immune to owner-driven budget changes, enforceable without judgment calls, and protective of both the owner's risk position and the PM's operational autonomy within appropriate bounds.

---

## 2. HARD COST CO THRESHOLD FRAMEWORK

Applies independently to hard cost and soft cost budgets (each tracked separately with their own contingency).

### Rule 1 — Threshold Formula (Formula C)
```
PM threshold = Remaining contingency ÷ Original hard cost contract sum
```
Denominator is fixed at project start. Never adjusted for owner scope additions or budget increases. Threshold decays only as contingency is spent. Applied per division line item: PM threshold % × division original contract value = maximum PM-approvable CO amount for that division.

### Rule 2 — Approval Routing
- Below threshold → PM approves. Contingency drawn automatically. Reported to owner in quarterly hard cost review.
- At or above threshold → Owner approval required before work proceeds. No PM discretion. Principal brings to owner. Exception: 1–2 per project maximum in rare timing circumstances, at Principal discretion only.

*Note: TPM sub-threshold CO delegation during PM absence is not automatic — see TPM Role definition in alpine-operating-model.md.*

### Rule 3 — Owner-Directed Scope Additions
Owner additions never draw from contingency. Budget increase required and authorized by owner before work is contracted. Routes to Principal regardless of size. Has no effect on Formula C denominator.

### Rule 4 — Contingency Review Trigger
When cumulative owner scope additions reach the initial contingency percentage of original hard cost, PM flags to Principal immediately. No further scope additions processed until Principal has re-analyzed risk, proposed a specific top-up to owner, and received either written approval or written decline. If owner declines: (a) documented in writing — owner explicitly assumes the risk gap, and (b) PM threshold continues on Formula C but Principal and PM are both aware the cushion is thinner than the original analysis assumed.

---

## 3. SOFT COST CO RULES

*Hard/soft cost separation confirmed — each budget has independent contingency and the CO framework applies to each independently. Soft cost CO approval rules not yet explicitly mapped.*

---

## 4. FORMULA EVALUATION RECORD

Six formulas were evaluated before Formula C was selected. Rejected formulas and reasons:

| Formula | Description | Rejection Reason |
|---|---|---|
| A | Remaining contingency ÷ Current contract sum | Denominator grows with owner scope adds; threshold decays even when contingency is untouched |
| B | Original contingency ÷ Original contract sum | Fixed ratio; ignores actual contingency spend; never reflects genuine erosion |
| D | Remaining contingency ÷ (Original + owner additions) | Penalizes owner for doing scope adds correctly; makes correct process look like risk |
| E | Remaining contingency ÷ Remaining contract sum | Similar to A; erodes with scope adds that have nothing to do with contingency |
| F | Remaining contingency ÷ (Original sum × billing rate) | Introduces billing-rate dependency; adds noise unrelated to risk |
| C | Remaining contingency ÷ Original hard cost contract sum | **Selected.** Immune to owner scope additions; denominator anchored to scope contingency was sized for |

**DP Validation:** Formula C was stress-tested against a real $50M→$72M six-structure project. Formula A threshold decayed 73% (15%→4%) over 18 months; 11 percentage points of that decay were caused by correct budget process (owner scope adds), not contingency spend. Formula C threshold at the same point = 5.76% — 44% higher authority, accurately reflecting only genuine contingency burn.

---

## 5. DOMAIN STATUS

```
Domain: CO Process
Status: In Progress
Last Output: Formula C locked; 4 rules fully defined; DP validation completed ($50M→$72M project)
             Hard/soft cost separation confirmed with independent contingencies
Open: Soft cost CO rules not yet explicitly mapped
      CO framework not yet output as standalone reference document
      Per-project exception log format not yet built
```

---

## 6. DECISIONS LOG (append-only)

```
26_04_21 | Hard Cost CO threshold formula locked: Formula C — remaining contingency ÷ original hard cost
26_04_21 | Formula C rationale: immune to owner scope additions; denominator anchored to scope contingency was sized for
26_04_21 | Formulas A/B/D/E/F evaluated and rejected: A and E erode with scope adds; B ignores top-ups; D penalizes top-ups; F introduces billing-rate dependency
26_04_21 | CO approval routing locked: below threshold = PM approves + auto contingency draw + quarterly reporting; above threshold = owner approval required, no PM discretion (1-2 exceptions per project max)
26_04_21 | Owner scope additions confirmed: never draw contingency; always budget increase; always to Principal regardless of size
26_04_21 | Contingency review trigger defined: fires when cumulative scope additions ≥ initial contingency % of original HC
26_04_21 | Owner decline of contingency top-up: documented in writing (owner assumes risk) + Formula C continues with acknowledged thinner cushion
26_04_21 | Hard/soft cost budgets tracked separately with independent contingencies; CO framework applies to each independently
26_04_21 | Project DP analysis completed: Formula A vs C stress test on real $50M→$72M six-structure project
26_04_21 | DP finding: Formula A threshold decayed 73% (15%→4%) in 18 months; 11pp of that decay caused by correct budget process, not contingency spend
26_04_21 | DP finding: Formula C threshold at same point = 5.76% — 44% higher authority, reflecting only genuine contingency burn
26_04_21 | DP PDF report produced and delivered
```

---

## 7. OPEN QUESTIONS

```
1. How does the CO framework apply to soft cost budget specifically — are the approval routing rules identical or do soft cost COs have different thresholds?
2. Should the CO approval exception (1–2 per project maximum) be formally logged per project, and where does that log live?
3. What is the standard format for the written owner decline of a contingency top-up?
```

---

## 8. ACTIVE WORKSTREAM

Formula C locked and DP-validated. Next: output CO framework as standalone reference document and map soft cost CO rules explicitly.

---

## 9. NEXT MOVES (prioritized)

```
1. OUTPUT — CO Framework as Standalone Reference Document
   Why: Framework is locked; needs to exist as a referenceable artifact for PM onboarding and owner communication
   How: Encode Formula C + 4 rules + approval routing + contingency trigger into single structured doc

2. DEFINE — Soft Cost CO Rules
   Why: Hard/soft separation is confirmed but only hard cost rules are fully specified
   How: Determine whether Formula C applies identically to soft cost or requires adjustment; encode as rule set

3. BUILD — Per-Project CO Exception Log
   Why: The 1–2 exception limit per project requires tracking to be enforceable
   How: Simple log format (date, CO number, reason, Principal authorization) that lives in the project file
```

---

*Update Decisions Log and Domain Status after every meaningful session.*
*Re-pin to Claude project before starting any new workstream chat.*
