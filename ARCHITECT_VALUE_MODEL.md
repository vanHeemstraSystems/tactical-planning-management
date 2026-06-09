# Architect Value Model – Tactical Planning Layer

> *“A strategy is not a dusty document — it is a compass you check every day.”*
> This document connects the 6-year personal strategy to quarterly tactical decisions.

See parent: [`strategic-planning-management / PERSONAL_STRATEGY.md`](https://github.com/vanHeemstraSystems/strategic-planning-management/blob/main/PERSONAL_STRATEGY.md)

-----

## Purpose of This Document

At the tactical layer (6-quarter horizon), the key question is:

> **“Which themes and initiatives should I invest in — and which should I decline — based on my personal Business Model?”**

This document gives you a consistent filter to apply when planning each quarter’s tactical direction.

-----

## The Tactical Value Filter

Before committing to any tactical theme or initiative, apply this filter:

### Gate 1 — Strategic Alignment

*Does this theme serve my core value drivers?*

|My Value Driver         |Does This Theme Address It?|
|------------------------|---------------------------|
|Risk Reduction          |Yes / No / Partially       |
|Clarity for Stakeholders|Yes / No / Partially       |
|Independent Judgment    |Yes / No / Partially       |
|Mistake Prevention      |Yes / No / Partially       |
|Decision Acceleration   |Yes / No / Partially       |
|Knowledge Transfer      |Yes / No / Partially       |

**Rule:** At least two value drivers must be addressed. If zero or one — reject or reframe the theme.

### Gate 2 — Practice Health

*Does this theme engage me as architect or resource?*

```
[ ] Architect (judgment): I am deciding, advising, or reviewing trade-offs
[ ] Resource (execution): I am implementing someone else's decisions

If resource: Is there a clear path to architectural influence within this theme?
  Yes → accept with caution, set a reframe trigger point
  No  → decline or negotiate scope before committing
```

### Gate 3 — Navigational Principles

*Does this theme violate any of my non-negotiables?*

- [ ] The business goal is defined or can be established
- [ ] I will have genuine influence over architectural decisions
- [ ] I am not being pressured to skip due diligence
- [ ] There is a path to leaving the organisation more capable

**If any box is unchecked:** flag it before accepting the theme.

-----

## Tactical Theme Classification

When recording themes in your tactical planning system, classify each with:

```yaml
theme:
  title: ""
  architect_value_type: ""   # judgment | execution | knowledge-build | relationship | admin | misaligned
  value_drivers_served:      # list from: risk-reduction | clarity | independent-judgment |
    - ""                     #   mistake-prevention | decision-acceleration | knowledge-transfer
  gate_1_passed: true/false
  gate_2_passed: true/false
  gate_3_passed: true/false
  accepted: true/false
  reframe_trigger: ""        # If execution: what would need to change to make this judgment work?
```

-----

## Quarterly Review Questions

At the end of each quarter, before planning the next:

**Backward look:**

- Which themes delivered `judgment` value vs `execution` value?
- Were my architectural recommendations acted on across active themes?
- Which theme created the most lasting value (ADRs, capability uplift, risk averted)?
- Which theme was the biggest time-waster? Why did I accept it?

**Forward look:**

- What is the highest-leverage architectural theme I could pursue next quarter?
- Is there a pattern of execution-heavy work I need to break?
- Which relationships or domains need investment this coming period?

-----

## Architect Value Type Definitions

|Type             |Description                                                   |Target % of Themes|
|-----------------|--------------------------------------------------------------|------------------|
|`judgment`       |Deciding, advising, reviewing trade-offs — core architect work|>60%              |
|`execution`      |Implementing — sometimes necessary, watch the ratio           |<25%              |
|`knowledge-build`|Building your own expertise capital                           |10–20%            |
|`relationship`   |Strengthening key stakeholder connections                     |As needed         |
|`admin`          |Necessary overhead                                            |Minimise          |
|`misaligned`     |Should not have been accepted                                 |Target: 0%        |

-----

## Links Across the Hierarchy

|Direction|Level           |Document                                                                                                                    |
|---------|----------------|----------------------------------------------------------------------------------------------------------------------------|
|↑ Up     |Strategic (6yr) |[`PERSONAL_STRATEGY.md`](https://github.com/vanHeemstraSystems/strategic-planning-management/blob/main/PERSONAL_STRATEGY.md)|
|↓ Down   |PIPE (1 quarter)|[`ARCHITECT_VALUE_MODEL.md`](https://github.com/vanHeemstraSystems/pipe-management/blob/main/ARCHITECT_VALUE_MODEL.md)      |
