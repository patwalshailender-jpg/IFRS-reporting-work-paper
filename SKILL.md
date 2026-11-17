---
name: "ifrs-accounting-position-paper"
description: "Draft an IFRS technical accounting position paper (issue, guidance, analysis, conclusion) for an investment transaction or accounting question in a pension fund or investment entity."
---

# IFRS Accounting Position Paper

Produces an audit-ready technical accounting memo for a Financial Controller of a pension fund investment unit. Typical topics: IFRS 9 classification of a new investment, IFRS 10 control / investment entity assessment of a fund vehicle or SPV, IAS 28 / IFRS 11 significant influence or joint control, IFRS 13 fair value hierarchy levelling, IAS 40 investment property, IAS 21 FX, IAS 32 debt vs equity, and related IFRS 7 / IFRS 12 / IFRS 13 disclosures.

## Non-negotiable rules
1. **Cite only verified guidance.** Every paragraph reference must come from the reference map below or be confirmed on ifrs.org (or an IFRS Interpretations Committee agenda decision on ifrs.org) during this task. Never invent paragraph numbers, case law or agenda decisions. If unsure, write the standard name only and mark it `[verify para]`.
2. **Effective dates matter.** State the reporting period and check which version of each standard applies. Known items: Amendments to the Classification and Measurement of Financial Instruments (IFRS 9 / IFRS 7, May 2024) are effective for annual periods beginning on or after 1 January 2026. IFRS 18 replaces IAS 1 for annual periods beginning on or after 1 January 2027. Search ifrs.org for any later amendments.
3. **All numbers are computed in Python**, never mentally. Show the inputs and recheck totals before including figures or journal entries.
4. **Facts before conclusions.** If a fact that drives the conclusion is missing (e.g. contractual cash flow terms, voting rights, business model evidence), ask for it, or state it as an explicit assumption in section 3 and flag it in Open Points.
5. **Consider alternatives.** For each issue, set out at least two possible treatments and say why one is rejected.
6. Professional, concise tone. Use tables for comparisons. The memo is a draft for preparer and reviewer sign-off; never present it as final.

## Workflow
1. **Intake:** collect the transaction description, term sheet or agreements, the reporting entity and its year-end, the functional currency, the ownership structure, the amounts, and whether the entity is (or claims to be) an investment entity or applies IAS 26. Ask at most one consolidated list of questions; then proceed with labelled assumptions.
2. **Identify issues:** list each accounting question separately (e.g. Issue 1: classification; Issue 2: consolidation; Issue 3: fair value level).
3. **Research:** use the reference map; use WebSearch / WebFetch on ifrs.org for anything not in it, including IFRS Interpretations Committee agenda decisions relevant to the fact pattern.
4. **Analyse** each issue against the decision guides below.
5. **Quantify:** produce illustrative journal entries for initial recognition and subsequent measurement, plus the FS impact, all computed in Python.
6. **Draft** the memo in the structure below.
7. **Self-review** against the checklist, then deliver as a document (a Word .docx if the user asks for Word).

## Memo structure
**Header table:** To | From | Date | Subject | Reference no. | Reporting period | Status: DRAFT for review
1. **Purpose**: one paragraph.
2. **Executive summary**: issues → conclusions table (Issue | Conclusion | Key reference | Impact).
3. **Background and key facts**: numbered facts; assumptions clearly labelled "Assumption".
4. **Accounting issues**: numbered questions.
5. **Relevant authoritative guidance**: standard, paragraph and a short paraphrase (do not reproduce long extracts of the standards).
6. **Analysis**: per issue: alternatives table (Alternative | Supporting arguments | Counter-arguments), then reasoning, then conclusion.
7. **Conclusion and accounting treatment**: recognition, measurement, presentation.
8. **Illustrative journal entries**: Date | Account | Dr | Cr | Narrative (balanced, computed).
9. **Disclosure requirements**: IFRS 7, IFRS 12, IFRS 13 items triggered.
10. **Financial statement and KPI impact**: P&L, OCI, net assets, NAV / returns.
11. **Judgements, risks and open points**: what the auditor is likely to challenge, and the evidence needed.
12. **Sign-off**: Prepared by / Reviewed by / Approved by / Date (left blank).
**Appendix**: references with ifrs.org links; supporting calculations.

## Decision guides
**IFRS 9 classification of financial assets**
- Debt instruments: business model test plus SPPI test. Amortised cost if held to collect and SPPI (4.1.2); FVOCI if held to collect and sell and SPPI (4.1.2A); otherwise FVTPL (4.1.4). Fair value option to remove an accounting mismatch (4.1.5). SPPI means a basic lending arrangement (B4.1.7A). For instruments with contingent or ESG-linked features, apply the 2026 amendments.
- Equity instruments: FVTPL by default; an irrevocable FVOCI election at initial recognition for equity not held for trading (5.7.5). Fund units that are puttable instruments are not equity from the holder's perspective; check IFRS Interpretations Committee agenda decisions on ifrs.org before concluding `[verify]`.
- Initial recognition 3.1.1; initial measurement 5.1.1; derecognition 3.2; reclassification of financial assets only on a change in business model (4.4.1); impairment (ECL) section 5.5 for amortised cost / FVOCI debt.

**IFRS 10 / investment entities**
- Control requires power, exposure to variable returns, and the ability to use power to affect returns (para 7).
- Investment entity definition (27) and typical characteristics (28). An investment entity measures subsidiaries at FVTPL (31), except service subsidiaries that provide investment-related services, which are consolidated (32). Disclose the judgements (IFRS 12, incl. 9A).

**Associates and joint arrangements**
- Significant influence presumed at 20% or more of voting power (IAS 28.5). Venture capital organisations, mutual funds, unit trusts and similar entities may elect FVTPL under IFRS 9 for associates and joint ventures (IAS 28.18). Joint control and joint arrangements: IFRS 11.4–7.

**IFRS 13 fair value**
- Definition (9); hierarchy (72); Level 1 (76), Level 2 (81), Level 3 (86); disclosures (93). Level 3 requires valuation technique, unobservable inputs and sensitivity disclosures.

**Other**
- Retirement benefit plans: plan investments carried at fair value (IAS 26.32).
- Investment property: accounting policy choice (IAS 40.30); fair value model (IAS 40.33).
- Foreign currency monetary items retranslated at the closing rate (IAS 21.23).
- Financial liability vs equity: definitions (IAS 32.11); puttable instruments exception (IAS 32.16A–16D).
- Where no standard applies, use the IAS 8 hierarchy for developing an accounting policy `[verify para]`.

## Self-review checklist (complete before delivering)
- [ ] Every paragraph reference is from the reference map or verified on ifrs.org; anything unverified is marked `[verify]`.
- [ ] Effective dates and the reporting period are checked.
- [ ] Each issue has alternatives considered and a clear conclusion.
- [ ] Journal entries balance (checked in Python); figures agree to the facts.
- [ ] Assumptions are listed and carried into Open Points.
- [ ] Disclosure section covers IFRS 7 / 12 / 13 as relevant.
- [ ] No long verbatim extracts from the standards.
- [ ] Status is shown as DRAFT, with sign-off fields blank.