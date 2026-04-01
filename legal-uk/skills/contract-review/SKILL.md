---
name: contract-review
description: UK commercial contract review workflow — playbook-based clause-by-clause analysis with GREEN/YELLOW/RED risk classification and redline suggestions. Also covers contract law fundamentals (formation, terms, unfair terms under UCTA 1977/CRA 2015, misrepresentation, breach, remedies, limitation periods, force majeure). Replaces and absorbs the former contract-law skill.
---

# Contract Review — /contract-review

> **DISCLAIMER:** This skill provides legal information for England & Wales only. It does not constitute legal advice and is not a substitute for instruction of a qualified solicitor regulated by the SRA. Verify all citations on [legislation.gov.uk](https://www.legislation.gov.uk). Law stated as at March 2026.

## Arguments

The user invoked this with: **$ARGUMENTS**

This skill serves two purposes:

1. **Contract review workflow**: If the user pastes a contract, describes clauses, or asks for a review, use the Playbook-Based Review Workflow (Part A).
2. **Contract law reference**: If the user asks about contract law topics (formation, terms, breach, remedies, limitation, unfair terms, force majeure, misrepresentation), use the Reference Knowledge (Part B).

| Keyword | Section |
|---|---|
| `review` or contract text pasted | Part A — Playbook-Based Review |
| `formation` | Part B, §1 — Contract Formation |
| `formal-requirements` | Part B, §2 — Formal Requirements |
| `terms` | Part B, §3 — Terms & Classification |
| `unfair-terms` | Part B, §4 — Unfair Terms (UCTA 1977 / CRA 2015) |
| `misrepresentation` | Part B, §5 — Misrepresentation |
| `breach` or `remedies` | Part B, §6 — Breach & Remedies |
| `limitation` | Part B, §7 — Limitation Periods |
| `force-majeure` | Part B, §8 — Force Majeure & Frustration |
| `third-party` | Part B, §9 — Third Party Rights |
| `nom` or `oral-modification` | Part B, §10 — No Oral Modification Clauses |

## Response Constraints

1. **Cite only verified sources**: Only cite statutes, sections, and cases that appear in this skill document. Do not invent or generate case citations. If a relevant case is not in this skill, say: *"Case law generally supports this position — verify on BAILII or Westlaw UK."*
2. **Flag uncertainty explicitly**: Use phrases like *"as at March 2026"* or *"verify the current figure on legislation.gov.uk."*
3. **Issue-spotting, not advice**: Frame all outputs as issue identification — not as definitive legal advice.
4. **Scope boundaries**: If a query falls outside England & Wales, say so clearly.
5. **No fabricated citations**: If asked for a case or authority you cannot verify from this skill's content, explicitly say: *"I don't have a verified citation for that — please check BAILII (bailii.org) or instruct a solicitor."*

---

# PART A — Playbook-Based Contract Review Workflow

## Review Process

1. **Identify the contract type**: B2B service agreement, SaaS/technology licence, commercial supply, MSA/SOW, subcontracting, agency agreement.
2. **Determine the user's side**: Supplier or customer? Licensor or licensee? This changes the analysis.
3. **Read the entire contract** before flagging issues — clauses interact (e.g., an uncapped indemnity may be partially mitigated by a broad limitation of liability).
4. **Analyse each material clause** against the UK market standard positions below.
5. **Consider the contract holistically**: Is the overall risk allocation balanced?

## Clause Taxonomy and UK Market Standard Positions

### A.1 Definitions

**Market Standard**: Comprehensive, internally consistent defined terms including: "Agreement," "Business Day," "Charges/Fees," "Commencement Date," "Confidential Information," "Data Protection Legislation," "Deliverables," "Force Majeure Event," "Good Industry Practice," "Intellectual Property Rights," "Losses," "Services," "Term."

| Rating | Indicator |
|--------|-----------|
| GREEN | Definitions are clear, balanced, and complete |
| YELLOW | Key terms undefined or ambiguously defined; defined terms used inconsistently |
| RED | Definitions drafted to give one party unfair advantage (e.g., "Losses" defined to include indirect, consequential, and punitive damages in a one-sided indemnity) |

### A.2 Term and Commencement

**Market Standard (B2B Service)**: Fixed initial term of 12–36 months with option to renew. **Market Standard (SaaS)**: Initial subscription term of 12 months with automatic renewal; 30–90 days' notice for non-renewal.

| Rating | Indicator |
|--------|-----------|
| GREEN | Fixed initial term with clear renewal mechanism and adequate notice period |
| YELLOW | Auto-renewal with <30 days' non-renewal notice; rolling monthly with no minimum; initial term >36 months |
| RED | Evergreen contract with no right to terminate for convenience; minimum term 5+ years with punitive early termination charges |

### A.3 Termination

**Market Standard**: Both parties have reciprocal rights to terminate: (1) for convenience on 30–90 days' notice; (2) for material breach with 30-day cure period; (3) for insolvency (Insolvency Act 1986, s.123); (4) for change of control (Corporation Tax Act 2010, s.1124).

**CIGA 2020 note**: The Corporate Insolvency and Governance Act 2020, s.14 (inserting new s.233B into the Insolvency Act 1986) prevents suppliers from terminating supply contracts by reason of the customer's entry into certain insolvency procedures, unless the court gives permission.

| Rating | Indicator |
|--------|-----------|
| GREEN | Reciprocal termination rights for breach (with cure period), insolvency, and convenience |
| YELLOW | One-sided termination for convenience; cure period <14 days or >60 days; no termination for insolvency |
| RED | Only one party can terminate for breach; no cure period; punitive termination charges amounting to a penalty (*Cavendish Square Holding BV v Makdessi* [2015] UKSC 67); contract cannot be terminated during term |

### A.4 Limitation of Liability

This is the most critical clause in any UK commercial contract review.

**UCTA 1977 framework**:
- **s.2(1)**: Cannot exclude liability for death or personal injury from negligence — **void**.
- **s.2(2)**: Exclusion of liability for other negligence loss subject to **reasonableness test**.
- **s.3**: Where one party deals on the other's standard terms, exclusion of breach liability subject to reasonableness.
- **s.11**: Reasonableness test considers bargaining power, inducements, knowledge of the term, availability elsewhere.
- Liability for fraud cannot be excluded: *HIH Casualty and General Insurance Ltd v Chase Manhattan Bank* [2003] UKHL 6.

**Market standard multi-tier structure**:

| Tier | Coverage | Standard |
|------|----------|----------|
| **Tier 1 — Unlimited** | Death/PI from negligence (UCTA s.2(1)); fraud; wilful default; breach of confidentiality; IP infringement | Cannot be capped |
| **Tier 2 — Higher/separate cap** | Data protection breaches (UK GDPR); breach of indemnity | 2–5x annual contract value |
| **Tier 3 — General cap** | All other liabilities | 100–200% of charges paid/payable in preceding 12 months |
| **Tier 4 — Excluded losses** | Indirect, consequential, special damages (including loss of profit, revenue, business, goodwill, anticipated savings, data) | Reciprocal exclusion |

**Critical note on "consequential loss"**: Under *British Sugar Plc v NEI Power Projects Ltd* (1997) 87 BLR 42 (CA) and *Deepak Fertilisers & Petrochemicals Corp v ICI Chemicals & Polymers Ltd* [1999] 1 Lloyd's Rep 387 (CA), "consequential loss" in a contractual exclusion clause refers only to second-limb *Hadley v Baxendale* losses. **Direct loss of profit** that arises naturally from the breach is first-limb and is **not** caught by a standard exclusion of "indirect and consequential loss." To exclude loss of profit, the clause must expressly name it.

| Rating | Indicator |
|--------|-----------|
| GREEN | Multi-tier structure; UCTA-compliant; reciprocal exclusion of indirect/consequential loss; general cap at 100–200% annual value; separate higher caps for DP and IP |
| YELLOW | Low cap (<100% annual value); aggregate cap (not per-claim); no separate DP/IP cap; one-sided exclusion of indirect loss; exclusion of direct loss of profit |
| RED | Exclusion of all liability (unenforceable under UCTA on standard terms); exclusion of death/PI negligence liability (void under UCTA s.2(1)); one-sided unlimited liability; no cap at all |

### A.5 Indemnities

Under English law, an indemnity is a primary obligation to pay — distinguished from damages for breach. It may extend beyond the *Hadley v Baxendale* remoteness test: *Total Transport Corp v Arcadia Petroleum Ltd (The Eurus)* [1998] 1 Lloyd's Rep 351.

An indemnity claim accrues when the indemnified party suffers the loss, not when the breach occurred — affecting limitation under the Limitation Act 1980.

**Market standard**: IP infringement indemnity (supplier → customer); data protection indemnity; negligence/misconduct indemnity. Standard procedure: notice, conduct of defence, mitigation.

| Rating | Indicator |
|--------|-----------|
| GREEN | Reciprocal indemnities for IP, data breaches, third-party claims; subject to liability cap or separate reasonable cap; standard procedure |
| YELLOW | One-sided indemnity; indemnity for breach of warranty (blurs distinction); indemnity outside liability cap |
| RED | Uncapped one-sided indemnity covering all losses; indemnity for losses within indemnified party's control; indemnity covering indemnified party's own negligence |

### A.6 Warranties and Representations

Under English law, breach of warranty gives damages but generally not termination rights (unless breach amounts to repudiation). A false representation may give rise to claims under Misrepresentation Act 1967. Standard of care for services: reasonable care and skill (Supply of Goods and Services Act 1982, s.13).

| Rating | Indicator |
|--------|-----------|
| GREEN | Standard warranties (reasonable care and skill, authority, compliance with law, conformity to spec); reasonable warranty period |
| YELLOW | Heavily qualified warranties ("to the best of supplier's knowledge"); "fitness for purpose" (higher standard than reasonable care); customer gives broad information-accuracy warranties |
| RED | All warranties excluded ("as is"); no warranty of authority/capacity; customer warranties on matters outside its control |

### A.7 Force Majeure

English law does **not** recognise force majeure as a general doctrine — it operates only as a contractual provision: *Canary Wharf (BP4) T1 Ltd v European Medicines Agency* [2019] EWHC 335 (Ch). The doctrine of **frustration** is narrow: performance must become impossible, illegal, or radically different — not merely more expensive: *Davis Contractors Ltd v Fareham Urban District Council* [1956] AC 696 (HL).

Post-COVID: *MUR Shipping BV v RTI Ltd* [2022] EWCA Civ 1406 (duty to mitigate in force majeure context).

| Rating | Indicator |
|--------|-----------|
| GREEN | Comprehensive event list; reciprocal suspension; duty to mitigate; termination right after 60–90 days; payment obligations not excused |
| YELLOW | Narrow event list; no termination right after prolonged FM; clause excuses payment |
| RED | No FM clause (reliance on frustration is very narrow); one-sided FM; clause permanently discharges obligations |

### A.8 Intellectual Property Ownership

Under CDPA 1988: copyright in contractor-created works belongs to the **contractor** absent express written assignment (s.11(1)). Employer owns employee-created works (s.11(2)). Assignment must be in writing signed by assignor (s.90(3)). Under Patents Act 1977, s.39: employee inventions belong to employer only if made in course of normal duties where invention might reasonably be expected. The US "work-for-hire" doctrine (17 USC s.101) does **not** exist in English law.

| Rating | Indicator |
|--------|-----------|
| GREEN | Clear Background IP / Foreground IP distinction; Foreground IP assigned to customer in writing; licence-back for incorporated Background IP; moral rights waiver (CDPA 1988, ss.77–89) |
| YELLOW | IP ownership ambiguous; no clear assignment mechanism; supplier retains all IP and grants only a licence |
| RED | Customer must assign its own Background IP to supplier; no IP assignment at all for bespoke deliverables; IP provisions rely on US "work-for-hire" (ineffective under English law) |

### A.9 Data Protection

Where the contract involves processing personal data, UK GDPR Art.28(3) requires a written contract specifying: subject-matter, duration, nature/purpose, data types, data subject categories, controller obligations/rights. Plus specific processor obligations (process only on instructions, confidentiality, security measures, sub-processor requirements, assist with DSARs, breach notification, deletion/return, audit rights).

| Rating | Indicator |
|--------|-----------|
| GREEN | Comprehensive DPA complying with Art.28(3); clear controller/processor roles; sub-processor provisions; international transfer mechanism (UK IDTA or UK Addendum to EU SCCs); data breach notification |
| YELLOW | No DPA but basic DP provisions; or DPA based on EU (not UK) standard terms not updated for UK GDPR |
| RED | No DP provisions despite personal data processing; DPA makes processor a controller (shifting risk); permits unrestricted international transfers without transfer mechanism |

### A.10 Governing Law and Dispute Resolution

**Market Standard**: English law; exclusive jurisdiction of E&W courts. For higher-value contracts: LCIA or ICC arbitration with London seat. Courts strongly encourage mediation: *Churchill v Merthyr Tydfil County Borough Council* [2023] EWCA Civ 1416.

| Rating | Indicator |
|--------|-----------|
| GREEN | English law; exclusive E&W jurisdiction; or LCIA/ICC arbitration with London seat |
| YELLOW | Non-exclusive jurisdiction; asymmetric jurisdiction; foreign governing law (if commercially justified) |
| RED | Foreign law with no connection to parties; jurisdiction of foreign court with no reciprocal enforcement; no governing law clause |

### A.11 Anti-Bribery (Bribery Act 2010)

Bribery Act 2010, s.7: strict liability corporate offence of failure to prevent bribery by an "associated person." Defence: "adequate procedures" (Ministry of Justice guidance, March 2011 — six principles: proportionate procedures, top-level commitment, risk assessment, due diligence, communication, monitoring).

| Rating | Indicator |
|--------|-----------|
| GREEN | Reciprocal anti-bribery warranties; reference to Bribery Act 2010; adequate procedures obligations; immediate termination for breach |
| YELLOW | Anti-bribery clause present but weak (no adequate procedures reference, no termination right); or absent in contract involving public procurement/international counterparties |
| RED | No anti-bribery clause in contract involving high bribery-risk activities/jurisdictions; clause purports to exclude bribery liability |

### A.12 Modern Slavery (Modern Slavery Act 2015)

Modern Slavery Act 2015, s.54: commercial organisations with turnover ≥£36 million must produce annual slavery statement.

| Rating | Indicator |
|--------|-----------|
| GREEN | Comprehensive clause with warranties, audit rights, notification obligations, termination rights |
| YELLOW | Basic representation but no audit rights or notification obligations |
| RED | No clause in contract involving sectors/jurisdictions with known modern slavery risk |

### A.13 Late Payment

Late Payment of Commercial Debts (Interest) Act 1998: statutory interest at 8% above Bank of England base rate. Fixed compensation: £40 (debts <£1,000), £70 (£1,000–£9,999.99), £100 (≥£10,000). Statutory right to interest cannot be ousted unless contract provides a "substantial remedy."

| Rating | Indicator |
|--------|-----------|
| GREEN | 30-day payment terms; interest at statutory rate or higher; right to suspend for non-payment |
| YELLOW | 45–60 day terms; sub-statutory interest rate; no suspension right |
| RED | 90+ day terms; no interest on late payment; terms purporting to exclude statutory interest (may be ineffective) |

### A.14 IR35 / Off-Payroll Working

Since 6 April 2021, medium and large private sector clients must determine employment status (ITEPA 2003, Chapter 10, Part 2, as amended by Finance Act 2020). Small company exemption: CA 2006, s.382.

| Rating | Indicator |
|--------|-----------|
| GREEN | Addresses IR35 with status determination provisions, liability allocation, genuine self-employment indicators |
| YELLOW | No IR35 provisions in contract with a PSC |
| RED | Purports to guarantee "outside IR35" without genuine assessment; terms inconsistent with self-employment |

### A.15 Assignment and Subcontracting

| Rating | Indicator |
|--------|-----------|
| GREEN | Reciprocal restriction on assignment with consent; supplier may not subcontract without consent; intra-group assignment permitted (CA 2006, s.1159) |
| YELLOW | One-sided assignment restriction; no subcontracting restriction despite personnel-dependent services |
| RED | One party may assign to any third party without consent or notice; contract silent on assignment |

### A.16 Insurance

| Rating | Indicator |
|--------|-----------|
| GREEN | Requires supplier to maintain appropriate insurance (employers' liability min £5M per Employers' Liability (Compulsory Insurance) Act 1969; public liability; PI if applicable) and provide evidence on request |
| YELLOW | No insurance clause; or insurance levels below market standard |
| RED | Expressly excludes insurance requirements; obligations inconsistent with available insurance coverage |

---

## Review Output Format

```
## Contract Review Summary

**Contract Type**: [e.g., B2B SaaS Agreement]
**Your Side**: [Customer / Supplier]
**Governing Law**: [stated law]
**Overall Risk Assessment**: [GREEN / YELLOW / RED]

### Clause-by-Clause Analysis

| # | Clause | Rating | Issue | Priority |
|---|--------|--------|-------|----------|
| 1 | Limitation of Liability | [G/Y/R] | [brief note] | [Must-have / Should-have / Nice-to-have] |
| 2 | Indemnification | [G/Y/R] | [brief note] | ... |
| ... | ... | ... | ... | ... |

### Must-Have Redlines (Tier 1 — Deal Breakers)
[For each: clause reference, current language, proposed redline, rationale, fallback]

### Should-Have Redlines (Tier 2 — Strong Preferences)
[Same format]

### Nice-to-Have Redlines (Tier 3 — Concession Candidates)
[Same format]

### What This Means for Your Business
[Plain-English summary of the key risks and recommended actions]

### Recommended Next Steps
- [Specific actions — e.g., "ask your solicitor to review the liability cap," "propose your standard DPA"]
```

### Redline Format

For each redline:

**Clause**: [Section reference and clause name]
**Current language**: "[exact quote]"
**Proposed redline**: "[specific alternative language]"
**Rationale**: [1–2 sentences — suitable for sharing with the counterparty's solicitor]
**Priority**: [Must-have / Should-have / Nice-to-have]
**Fallback**: [Alternative position if primary redline is rejected]

---

# PART B — Contract Law Reference Knowledge

## 1. Contract Formation

A valid contract under English law requires five elements:

### 1.1 Offer

An offer is an expression of willingness to contract on stated terms, made with the intention that it will become binding once accepted. Distinguish from an **invitation to treat**:

- Display of goods in a shop is an invitation to treat: *Pharmaceutical Society of Great Britain v Boots Cash Chemists (Southern) Ltd* [1953] 1 QB 401.
- Unilateral promise may constitute an offer: *Carlill v Carbolic Smoke Ball Company* [1893] 1 QB 256 (CA).
- Advertisements are generally invitations to treat unless they amount to a unilateral offer (*Carlill*).

An offer may be revoked at any time before acceptance, provided revocation is communicated: *Byrne & Co v Leon Van Tienhoven & Co* (1880) 5 CPD 344.

### 1.2 Acceptance

Acceptance must be unqualified and communicated. A counter-offer destroys the original offer: *Hyde v Wrench* (1840) 3 Beav 334. The **postal rule** provides acceptance by post takes effect on posting: *Adams v Lindsell* (1818) 1 B & Ald 681. Does not apply to instantaneous communications (*Entores Ltd v Miles Far East Corporation* [1955] 2 QB 327) or email.

### 1.3 Consideration

Must be sufficient but need not be adequate: *Chappell & Co Ltd v Nestle Co Ltd* [1960] AC 87. Past consideration is not good consideration: *Re McArdle* [1951] Ch 669. Performance of existing duty is generally not consideration (*Stilk v Myrick* (1809) 2 Camp 317), but a **practical benefit** can suffice: *Williams v Roffey Bros* [1991] 1 QB 1 (CA).

### 1.4 Intention to Create Legal Relations

Presumed present in commercial agreements: *Edwards v Skyways Ltd* [1964] 1 WLR 349. Presumed absent in domestic arrangements: *Balfour v Balfour* [1919] 2 KB 571 (CA). Both presumptions rebuttable.

### 1.5 Capacity

Minors (under 18): contracts for necessaries binding (SGA 1979, s.3); employment/apprenticeship contracts binding if substantially for minor's benefit. Companies: CA 2006, s.39 (directors' power to bind), s.40 (third-party protection).

### 1.6 Deeds

A contract by deed requires no consideration. Requirements: LP(MP)A 1989, s.1 — must make clear it is a deed, signed in presence of attesting witness, delivered.

---

## 2. Formal Requirements

| Contract Type | Requirement | Authority |
|---|---|---|
| Sale/disposition of interest in land | Writing, signed by both parties, all terms in one document | LP(MP)A 1989, s.2 |
| Guarantee | Evidenced in writing, signed by guarantor | Statute of Frauds 1677, s.4 |
| Regulated consumer credit | Prescribed form, signed by debtor | Consumer Credit Act 1974, ss.60-65 |
| Copyright assignment | Writing, signed by assignor | CDPA 1988, s.90(3) |
| Lease >3 years | Must be by deed | LPA 1925, s.52 |

---

## 3. Terms & Classification

- **Condition**: Fundamental term; breach entitles termination + damages.
- **Warranty**: Lesser term; breach gives damages only.
- **Innominate term**: Classification depends on breach consequences: *Hong Kong Fir Shipping Co Ltd v Kawasaki Kisen Kaisha Ltd* [1962] 2 QB 26 (CA).

**Implied terms — Sale of Goods (SGA 1979)**: s.12 (title), s.13 (description), s.14(2) (satisfactory quality), s.14(3) (fitness for purpose), s.15 (sample). For B2C: superseded by CRA 2015, Part 1.

**Implied terms — Supply of Services (SGSA 1982)**: s.13 (reasonable care and skill), s.14 (reasonable time), s.15 (reasonable charge). For B2C: CRA 2015, ss.49-52.

**Entire agreement clauses**: Do not by themselves exclude misrepresentation liability: *AXA Sun Life Services plc v Campbell Martin Ltd* [2011] EWCA Civ 133. Separate exclusion needed, subject to MA 1967, s.3 reasonableness test.

---

## 4. Unfair Terms

### 4.1 B2B — UCTA 1977

| Section | Rule |
|---|---|
| s.2(1) | Cannot exclude death/PI negligence liability — **void** |
| s.2(2) | Other negligence loss exclusion subject to **reasonableness** |
| s.3 | On written standard terms: breach exclusion subject to reasonableness |
| s.6 | Title implied terms (SGA s.12) cannot be excluded; other implied terms (ss.13-15) subject to reasonableness in B2B |
| s.11 | Reasonableness test: fair and reasonable having regard to circumstances known or contemplated at time of contracting |

### 4.2 B2C — CRA 2015, Part 2

- **Fairness test** (s.62): Unfair if contrary to good faith, causes significant imbalance to consumer's detriment.
- **Core terms exemption** (s.64): Main subject matter/price exempt only if transparent and prominent.
- **Grey list** (Schedule 2): Indicative list of potentially unfair terms.
- **Effect** (s.67): Unfair term not binding on consumer; contract continues without it.

---

## 5. Misrepresentation

| Type | Mental Element | Damages Measure |
|---|---|---|
| **Fraudulent** | Knowingly false / reckless: *Derry v Peek* (1889) 14 App Cas 337 | Tort: all direct loss |
| **Negligent (statutory)** | Cannot prove reasonable grounds: MA 1967, s.2(1) | Fiction of fraud: *Royscot Trust v Rogerson* [1991] 2 QB 297 |
| **Innocent** | Reasonable grounds for belief | Damages in lieu of rescission: MA 1967, s.2(2) |

Exclusion of misrepresentation liability subject to reasonableness: MA 1967, s.3 (as substituted by UCTA 1977, s.8).

---

## 6. Breach & Remedies

**Damages**: Expectation measure — place innocent party in position had contract been performed: *Robinson v Harman* (1848) 1 Ex 850. **Remoteness**: *Hadley v Baxendale* (1854) 9 Ex 341; *The Achilleas* [2008] UKHL 48. **Mitigation** required: *British Westinghouse* [1912] AC 673.

**Anticipatory breach**: Innocent party may accept repudiation and sue immediately or affirm: *White & Carter v McGregor* [1962] AC 413.

**Penalty clauses**: *Cavendish Square v Makdessi* [2015] UKSC 67 — unenforceable if detriment is out of all proportion to legitimate interest. Liquidated damages for delay accrue up to termination: *Triple Point Technology v PTT* [2021] UKSC 29.

**Specific performance**: Equitable, discretionary; available for land sales; not for personal service contracts: *Co-operative Insurance v Argyll Stores* [1998] AC 1.

---

## 7. Limitation Periods

| Cause of Action | Period | Limitation Act 1980 |
|---|---|---|
| Simple contract | 6 years from accrual | s.5 |
| Deed | 12 years | s.8 |
| Tort (general) | 6 years | s.2 |
| Personal injury | 3 years from accrual/knowledge | s.11 |
| Latent damage (negligence) | 6 years or 3 years from knowledge; 15-year long-stop | ss.14A-14B |
| Contribution | 2 years from judgment/settlement | s.10 |

**Postponement**: Fraud/concealment/mistake — time runs from discovery (s.32). Disability — time runs from cessation (s.28). Acknowledgement/part-payment resets clock (ss.29-30).

---

## 8. Force Majeure & Frustration

**Force majeure**: No general doctrine in English law — purely contractual. Construed strictly: *Classic Maritime Inc v Limbungan Makmur Sdn Bhd* [2019] EWCA Civ 1102.

**Frustration**: Supervening event renders performance impossible, illegal, or radically different: *Taylor v Caldwell* (1863) 3 B & S 826. Not applicable where merely more expensive: *Davis Contractors v Fareham UDC* [1956] AC 696. Consequences governed by Law Reform (Frustrated Contracts) Act 1943.

---

## 9. Third Party Rights

Privity: only a party may enforce: *Dunlop Pneumatic Tyre v Selfridge* [1915] AC 847. Statutory exception: Contracts (Rights of Third Parties) Act 1999 — s.1(1)(a): express provision; s.1(1)(b): term conferring benefit. Standard practice: exclude the Act.

---

## 10. No Oral Modification Clauses

NOM clauses are effective: *Rock Advertising Ltd v MWB Business Exchange Centres Ltd* [2018] UKSC 24. A party seeking to enforce an oral variation despite a NOM clause may need to rely on estoppel.

---

## Key Statute Reference Table

| Short Title | Citation | Link |
|---|---|---|
| Unfair Contract Terms Act 1977 | c. 50 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1977/50) |
| Sale of Goods Act 1979 | c. 54 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1979/54) |
| Limitation Act 1980 | c. 58 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1980/58) |
| Supply of Goods and Services Act 1982 | c. 29 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1982/29) |
| CDPA 1988 | c. 48 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1988/48) |
| LP(MP)A 1989 | c. 34 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1989/34) |
| Misrepresentation Act 1967 | c. 7 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1967/7) |
| Contracts (Rights of Third Parties) Act 1999 | c. 31 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1999/31) |
| Consumer Rights Act 2015 | c. 15 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/2015/15) |
| Bribery Act 2010 | c. 23 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/2010/23) |
| Modern Slavery Act 2015 | c. 30 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/2015/30) |
| Late Payment of Commercial Debts (Interest) Act 1998 | c. 20 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1998/20) |
| Insolvency Act 1986 | c. 45 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1986/45) |
| CIGA 2020 | c. 12 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/2020/12) |
| Patents Act 1977 | c. 37 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1977/37) |
| Companies Act 2006 | c. 46 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/2006/46) |
| Arbitration Act 1996 | c. 23 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1996/23) |

## Court Fees Reference (HMCTS)

| Claim Value | Issue Fee |
|------------|----------|
| Up to £300 | £35 |
| £300.01–£500 | £50 |
| £500.01–£1,000 | £70 |
| £1,000.01–£1,500 | £80 |
| £1,500.01–£3,000 | £115 |
| £3,000.01–£5,000 | £205 |
| £5,000.01–£10,000 | £455 |
| £10,000.01–£200,000 | 5% of claim value |
| Over £200,000 | £10,000 (capped) |

*Citation*: Civil Proceedings Fees Order 2008 (SI 2008/1053), as amended. Verify current fees at date of use.

## Solicitor Hourly Rates (Guideline — for costs context)

| Location | Grade A (8+ PQE) | Grade B (4–8 PQE) |
|----------|------------------|--------------------|
| London (City/Central) | £512–£647/hr | £348–£460/hr |
| London (Outer) | £450–£550/hr | £320–£420/hr |
| Regional centres | £350–£450/hr | £260–£350/hr |
| Other regions | £280–£380/hr | £220–£290/hr |

*Citation*: Civil Justice Council, Guideline Hourly Rates. Actual rates may be higher. Verify current rates.
