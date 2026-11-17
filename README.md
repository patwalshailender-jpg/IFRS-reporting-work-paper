# IFRS Position Paper

A Claude plugin for accountants, financial controllers and auditors. It drafts audit-ready **IFRS technical accounting position papers** for investment transactions in pension funds, investment entities and asset managers.

## What it does
Describe a transaction or accounting question, for example *"classify our 35% investment in an infrastructure fund LP"*, and Claude produces a structured memo:

1. Purpose and executive summary (issues → conclusions table)
2. Background facts and labelled assumptions
3. Accounting issues
4. Relevant authoritative guidance (standard and paragraph, paraphrased)
5. Analysis with alternative treatments considered
6. Conclusion and accounting treatment
7. Illustrative journal entries (computed and balanced)
8. Disclosure requirements (IFRS 7, IFRS 12, IFRS 13)
9. Financial statement and KPI impact
10. Judgements, risks and open points for the auditor
11. Sign-off block (Prepared / Reviewed / Approved)

**Standards covered:** IFRS 9, IFRS 10 (including investment entities), IFRS 11, IFRS 13, IAS 21, IAS 26, IAS 28, IAS 32, IAS 40, with effective-date checks (e.g. the 2026 IFRS 9/IFRS 7 amendments and IFRS 18 from 2027).

## Built-in quality controls
- Cites only verified IFRS paragraph references; anything unverified is flagged `[verify]`
- Checks which version of each standard applies to the reporting period
- Computes all figures and journal entries in code, never by estimation
- Considers at least two alternative treatments for every issue
- Marks every memo as a DRAFT for preparer and reviewer sign-off

## Example prompt
> Prepare an IFRS position paper. Entity: pension fund, year-end 31 December 2026. We invested USD 50m for 35% of an infrastructure fund LP; units are redeemable at NAV; we appoint 1 of 5 board members. Question: classification and measurement, and whether it is an associate.

## What it runs and connects to
This plugin contains a single skill (instructions only). It includes no scripts, hooks, MCP servers or external dependencies, stores no data, and sends no data anywhere. When verifying references, Claude may use its own built-in web search to read public pages on ifrs.org.

## Disclaimer
This plugin produces **draft** technical analysis to assist qualified accounting professionals. It is not professional advice and does not replace the judgement of a qualified accountant or auditor. Always verify references against the official standards at https://www.ifrs.org and apply your entity's facts, accounting policies and local regulatory requirements.

IFRS® is a trademark of the IFRS Foundation. This plugin is not affiliated with or endorsed by the IFRS Foundation or Anthropic.

## License
MIT. See LICENSE.
