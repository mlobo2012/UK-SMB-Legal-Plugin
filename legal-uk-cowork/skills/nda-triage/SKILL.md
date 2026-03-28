---
name: nda-triage
description: UK-specific NDA screening workflow — classifies NDAs as GREEN (safe to sign), YELLOW (flag with solicitor), or RED (do not sign). Covers English law NDA norms, standard exclusions, restraint of trade, UCTA 1977, UK GDPR, Competition Act 1998, and SRA Warning Notice compliance.
argument-hint: "<paste or describe the NDA> — or ask about UK NDA norms, standard clauses, or triage criteria"
---

# NDA Triage — /nda-triage

> **DISCLAIMER:** This skill provides legal information for England & Wales only. It does not constitute legal advice and is not a substitute for instruction of a qualified solicitor regulated by the SRA. Verify all citations on [legislation.gov.uk](https://www.legislation.gov.uk). Law stated as at March 2026.

## Arguments

The user invoked this with: **$ARGUMENTS**

If the user has pasted or described an NDA, perform a full triage analysis using the workflow below. If the user asks a general question about UK NDA norms, answer using the reference knowledge in this skill.

## Response Constraints

1. **Cite only verified sources**: Only cite statutes, sections, and cases that appear in this skill document. Do not invent or generate case citations. If a relevant case is not in this skill, say: *"Case law generally supports this position — verify on BAILII or Westlaw UK."*
2. **Flag uncertainty explicitly**: If you are not certain about a threshold, rate, or procedural rule, say so. Use phrases like *"as at March 2026"* or *"verify the current figure on legislation.gov.uk."*
3. **Issue-spotting, not advice**: Frame all outputs as issue identification to help the user prepare for professional consultation — not as definitive legal advice.
4. **Scope boundaries**: If a query falls outside England & Wales, or involves devolved Scottish/Northern Irish law, say so clearly and refer the user to appropriate jurisdiction-specific resources.
5. **No fabricated citations**: If asked for a case or authority you cannot verify from this skill's content, explicitly say: *"I don't have a verified citation for that — please check BAILII (bailii.org) or instruct a solicitor."*

---

## NDA Triage Workflow

### Step 1: Identify Agreement Structure

- **Type**: Mutual NDA, Unilateral (disclosing party), or Unilateral (receiving party)
- **Appropriateness**: Mutual NDAs are standard for B2B transactions between parties of comparable bargaining power. Unilateral NDAs are standard in employment contexts and where there is a clear asymmetry (e.g., a potential acquirer accessing a target's data room).
- **Standalone check**: Confirm the NDA is a standalone agreement, not a confidentiality section embedded in a larger commercial agreement.

### Step 2: Check Governing Law and Jurisdiction

| Indicator | Classification |
|-----------|---------------|
| England and Wales law, exclusive jurisdiction of E&W courts | GREEN |
| Foreign jurisdiction (e.g., New York, Delaware, California) — may be acceptable in cross-border transactions but introduces cost and enforcement risk for UK SMBs | YELLOW |
| Unconnected foreign jurisdiction; one-sided jurisdiction clause (disclosing party may sue anywhere, receiving party restricted to foreign court) | RED |

*Citation*: English law does not recognise a general doctrine of good faith in commercial contracts (*Walford v Miles* [1992] 2 AC 128), meaning NDA obligations are interpreted strictly as written. Post-Brexit, the retained Rome I Regulation (EC 593/2008) continues to determine applicable law for contractual obligations involving a foreign element.

**What this means for your business**: If the NDA is governed by US state law, litigating a dispute in the US is significantly more expensive than in England and Wales. US discovery obligations are broader and more burdensome than English law disclosure (CPR Part 31). A US court judgment must be enforced in England through fresh proceedings.

### Step 3: Check Definition of Confidential Information

| Indicator | Classification |
|-----------|---------------|
| Reasonably broad but tied to a defined "Purpose"; includes a marking/identification mechanism (14–30 days for oral disclosures) | GREEN |
| Extremely broad with no nexus to Purpose; covers information that may be publicly available | YELLOW |
| Covers "all information of any kind" without limitation or standard carve-outs — blanket secrecy obligation | RED |
| No "Purpose" defined, or Purpose so broad as to be meaningless | RED |

### Step 4: Verify Standard Exclusions

Under standard English law practice, **all four** of these carve-outs are essential:

1. Information that is or becomes publicly available (other than through breach by the receiving party)
2. Information already in the receiving party's possession before disclosure
3. Information independently developed without use of the disclosing party's confidential information
4. Information received from a third party not bound by confidentiality

| Indicator | Classification |
|-----------|---------------|
| All four exclusions present | GREEN |
| One exclusion missing or modified | YELLOW |
| Two or more exclusions missing | RED |

### Step 5: Check Permitted Disclosures

Standard UK NDAs permit disclosure:
- As required by law, regulation, or court order
- To professional advisers on a confidential basis
- To auditors
- As required by FCA/PRA obligations (FSMA 2000)

**Critical — whistleblowing carve-out**: The Public Interest Disclosure Act 1998 (PIDA) protects qualifying disclosures under the Employment Rights Act 1996, ss.43A–43L. An NDA **cannot lawfully restrict** a "protected disclosure." The SRA Warning Notice on NDAs (March 2018, updated November 2019) confirms that solicitors must not draft or use NDAs that attempt to prevent legitimate reporting to regulators including the SRA, FCA, or police.

| Indicator | Classification |
|-----------|---------------|
| Permits disclosures required by law/regulation; does not restrict whistleblowing; includes regulatory reporting carve-outs | GREEN |
| No express whistleblowing carve-out, but general confidentiality obligations do not explicitly restrict such reporting | YELLOW |
| Expressly restricts regulatory reporting, whistleblowing, or cooperation with investigations — such provisions are **void under statute** (ERA 1996, s.43J) | RED |

### Step 6: Check Confidentiality Obligations

| Indicator | Classification |
|-----------|---------------|
| Mutual obligations (in mutual NDA), proportionate, limited to defined Purpose; standard of care is "reasonable" or "no less than own confidential information" | GREEN |
| Receiving party must procure that Representatives enter direct undertakings with disclosing party (commercially burdensome, non-standard) | YELLOW |
| Strict liability for any breach with no reference to reasonable care; receiving party liable for all acts/omissions of Representatives regardless of reasonable steps | RED |

### Step 7: Check Term and Duration

*Citation*: The Trade Secrets (Enforcement, etc.) Regulations 2018 (SI 2018/597) provides a statutory framework — a "trade secret" is information that: (a) is secret; (b) has commercial value because it is secret; and (c) has been subject to reasonable steps to keep it secret.

| Indicator | Classification |
|-----------|---------------|
| Confidentiality obligations run 2–5 years from disclosure; longer/indefinite period for trade secrets | GREEN |
| Perpetual obligations for all confidential information (not just trade secrets) — may be disproportionate | YELLOW |
| No duration specified (creates uncertainty); or >20 years for routine business information | RED |

### Step 8: Check Return/Destruction Provisions

| Indicator | Classification |
|-----------|---------------|
| Return or destroy on termination/request; carve-outs for routine IT backups and legal/regulatory retention; written certification (not sworn affidavit) | GREEN |
| Requires destruction only with no carve-out for routine backups — may be impractical | YELLOW |
| Immediate return/destruction with no carve-outs; penalties for failure to comply | RED |

### Step 9: Check for Problematic Provisions

#### Non-Compete and Non-Solicitation

Under English law, all covenants in restraint of trade are prima facie void unless the party enforcing can show: (1) the restraint protects a "legitimate business interest" and (2) the restraint goes no further than reasonably necessary: *Nordenfelt v Maxim Nordenfelt Guns and Ammunition Co Ltd* [1894] AC 535 (HL); *Esso Petroleum Co Ltd v Harper's Garage (Stourport) Ltd* [1968] AC 269 (HL).

Courts may sever unenforceable restrictions under the blue-pencil doctrine: *Egon Zehnder Ltd v Tillman* [2019] UKSC 32.

| Indicator | Classification |
|-----------|---------------|
| No non-compete or non-solicitation; or narrowly tailored non-solicitation limited to specific customers/contacts, duration ≤6–12 months | GREEN |
| Non-solicitation clause of 12–24 months; or covering employees as well as customers | YELLOW |
| **Any non-compete clause in an NDA** (as opposed to a business sale or employment agreement); non-solicitation >24 months; restriction unlimited in geographical scope | RED |

#### Intellectual Property

| Indicator | Classification |
|-----------|---------------|
| No IP provisions beyond standard "no grant of rights/licence" clause | GREEN |
| Licence provisions beyond what's necessary for the Purpose | YELLOW |
| Assignment of receiving party's IP — entirely inappropriate in an NDA | RED |

#### Indemnity

Under English law, an indemnity is a primary obligation to pay (distinct from damages for breach). It may extend to losses that would not be recoverable as damages under the remoteness test in *Hadley v Baxendale* (1854) 9 Exch 341 and *Transfield Shipping Inc v Mercator Shipping Inc (The Achilleas)* [2008] UKHL 48.

| Indicator | Classification |
|-----------|---------------|
| No indemnity, or mutual/capped indemnity limited to direct losses | GREEN |
| One-sided indemnity in favour of disclosing party, with cap | YELLOW |
| Uncapped one-sided indemnity covering all losses including indirect/consequential and loss of profit | RED |

#### Penalty Clauses

Under *Cavendish Square Holding BV v Makdessi* [2015] UKSC 67, a clause is unenforceable as a penalty if it imposes a detriment "out of all proportion to any legitimate interest" of the innocent party.

| Indicator | Classification |
|-----------|---------------|
| No liquidated damages provision | GREEN |
| Disproportionate liquidated damages (e.g., £1 million for any breach in a routine SMB NDA) | RED |

#### Remedies

| Indicator | Classification |
|-----------|---------------|
| Acknowledges right to seek injunctive relief without purporting to guarantee its grant (under *American Cyanamid Co v Ethicon Ltd* [1975] AC 396, the court retains discretion) | GREEN |
| Purports to grant automatic right to injunctive relief (not possible under English law) | RED |

#### Other Red Flags

- **Personal guarantees** from directors — highly unusual in UK commercial NDA practice
- **Waiver of legal professional privilege**
- **Audit rights** — not standard in UK B2B NDA practice

### Step 10: Check Data Protection Compatibility

Where confidential information includes personal data (UK GDPR Article 4(1)):

| Indicator | Classification |
|-----------|---------------|
| NDA includes a data protection clause acknowledging compliance with UK GDPR/DPA 2018; does not restrict either party from complying with DP obligations | GREEN |
| No mention of data protection, but confidential information likely includes personal data | YELLOW |
| Purports to override or restrict DP obligations (e.g., prohibiting disclosure in response to a DSAR under UK GDPR Art.15, or restricting breach notification under Art.33) | RED |

*Citation*: UK GDPR Art.15 (right of access); Art.33 (breach notification to ICO within 72 hours); DPA 2018, s.45. A receiving party cannot rely on the NDA to refuse to comply with a DSAR — data protection obligations are statutory and override contractual confidentiality.

### Step 11: Check Competition Law Risk

*Citation*: Competition Act 1998, s.2 (Chapter I prohibition); CMA, Information sharing agreements guidance (OFT1389, adopted by CMA).

| Indicator | Classification |
|-----------|---------------|
| NDA is between non-competing parties; or between competitors with clean team provisions restricting access to competitively sensitive information | GREEN |
| NDA between competitors without clean team provisions, but scope of information sharing is limited and defined | YELLOW |
| NDA designed to facilitate exchange of competitively sensitive information between competitors without adequate safeguards; or contains provisions restricting competitive activity beyond protecting confidential information | RED |

### Step 12: UCTA 1977 Assessment

If the NDA is presented on one party's standard terms, exclusion/limitation clauses are subject to the reasonableness test under UCTA 1977, s.3 and s.11.

| Indicator | Classification |
|-----------|---------------|
| No exclusion/limitation clauses, or balanced clauses satisfying the UCTA reasonableness test | GREEN |
| Presented on one party's standard terms with exclusion clauses that may be subject to UCTA reasonableness test | YELLOW |
| Exclusion clauses clearly unreasonable (e.g., excluding all liability for breach including fraudulent concealment); or NDA with a consumer containing terms likely unfair under CRA 2015 Part 2 | RED |

---

## Triage Output Format

After analysing all steps, produce the following structured output:

```
## NDA Triage Result

**Overall Classification**: [GREEN / YELLOW / RED]
**Governing Law**: [stated law and jurisdiction]
**NDA Type**: [Mutual / Unilateral — direction]
**Counterparty**: [if identified]

### Summary
[1–3 sentences: what this means for your business in plain English]

### Clause-by-Clause Assessment

| # | Clause Area | Rating | Issue |
|---|-------------|--------|-------|
| 1 | Governing Law | [G/Y/R] | [brief note] |
| 2 | Definition of CI | [G/Y/R] | [brief note] |
| 3 | Standard Exclusions | [G/Y/R] | [brief note] |
| ... | ... | ... | ... |

### RED Flags (if any)
[List each RED issue with a plain-English explanation of what it means for your business]

### YELLOW Flags (if any)
[List each YELLOW issue with suggested action]

### Recommended Action
- **GREEN**: Safe to sign. No solicitor review required for this NDA.
- **YELLOW**: Flag these specific issues with your solicitor before signing. Typical turnaround: 1–2 business days.
- **RED**: Do not sign. Get legal advice immediately. [Specific recommendation — e.g., propose your own standard form NDA as a counter, or instruct a solicitor to negotiate specific clauses.]
```

---

## Quick Reference: Standard UK NDA Checklist

| Check | GREEN | YELLOW | RED |
|-------|-------|--------|-----|
| Governing law | England and Wales | Foreign jurisdiction (US/other) | Unconnected foreign jurisdiction; one-sided jurisdiction |
| Parties | Both clearly identified legal persons | One party is offshore entity or SPV | Unidentified party; personal guarantees required |
| Purpose | Clearly defined, specific | Vague or broad | Absent or meaningless |
| Mutuality | Mutual (both parties) or appropriate unilateral | Unilateral where bilateral expected | N/A |
| Confidential Information | Broad but tied to Purpose | Extremely broad; no nexus to Purpose | Covers all information; no exclusions |
| Exclusions | All four standard exclusions present | One exclusion missing or modified | Two or more exclusions missing |
| Permitted disclosures | Law, regulation, whistleblowing | Law/regulation only; no whistleblowing carve-out | Restricts law/regulation/whistleblowing |
| Confidentiality standard | Reasonable care / no less than own | Strict liability with caveats | Absolute strict liability |
| Duration | 2–5 years (trade secrets: longer/indefinite) | 5–10 years all information | Perpetual all information; no duration stated |
| Non-solicitation | Absent or limited (≤12 months) | 12–24 months; broad scope | >24 months; unlimited scope |
| Non-compete | Absent | N/A | Present in NDA |
| IP assignment | No IP provisions | Licence provisions | Assignment of receiving party's IP |
| Indemnity | Absent or mutual/capped | One-sided, capped | One-sided, uncapped |
| Return/destruction | Standard carve-outs | No backup carve-out | No carve-outs; penalties |
| Data protection | DP clause present | No DP clause; PI likely involved | Purports to override DP obligations |
| Competition | Non-competitors; or clean team | Competitors; no clean team | Facilitates anti-competitive info sharing |
| Remedies | Acknowledges injunctive relief (court discretion) | N/A | Purports to guarantee injunctive relief; penalty clause |

---

## Key UK vs US NDA Differences

UK SMBs frequently encounter US-drafted NDAs. Key differences to flag:

| Issue | US Position | UK Position | Triage Impact |
|-------|------------|-------------|---------------|
| Governing law | US state law (typically Delaware, NY, CA) | English law preferred for UK SMBs | YELLOW if US law |
| Injunctive relief | Often includes bond waiver | English law uses cross-undertaking in damages (*American Cyanamid*) — no bond posting | Note difference |
| Attorney's fees | "Prevailing party" clause standard (American Rule) | Loser pays (CPR 44.2(2)(a)) — clause unnecessary | Note difference |
| Work-for-hire | Available under 17 USC s.101 | Does not exist under English law (CDPA 1988, ss.11, 90(3)) — contractor retains copyright absent written assignment | RED if NDA relies on work-for-hire |
| Non-compete | Varies by state (CA: generally unenforceable) | Restraint of trade doctrine applies uniformly | RED if non-compete in NDA |

---

## Key Statute Reference Table

| Short Title | Citation | Link |
|---|---|---|
| Unfair Contract Terms Act 1977 | c. 50 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1977/50) |
| Employment Rights Act 1996 | c. 18 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1996/18) |
| Public Interest Disclosure Act 1998 | c. 23 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1998/23) |
| Competition Act 1998 | c. 41 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1998/41) |
| Consumer Rights Act 2015 | c. 15 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/2015/15) |
| Trade Secrets (Enforcement, etc.) Regulations 2018 | SI 2018/597 | [legislation.gov.uk](https://www.legislation.gov.uk/uksi/2018/597) |
| Copyright, Designs and Patents Act 1988 | c. 48 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1988/48) |
| Misrepresentation Act 1967 | c. 7 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1967/7) |
| Financial Services and Markets Act 2000 | c. 8 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/2000/8) |

## Key Case Law

| Case | Citation | Principle |
|------|----------|-----------|
| *Walford v Miles* | [1992] 2 AC 128 (HL) | No general duty of good faith in English commercial contracts |
| *Nordenfelt v Maxim Nordenfelt* | [1894] AC 535 (HL) | Restraint of trade doctrine — must protect legitimate interest, no wider than necessary |
| *Egon Zehnder v Tillman* | [2019] UKSC 32 | Blue-pencil severance of unenforceable restrictions |
| *Cavendish Square v Makdessi* | [2015] UKSC 67 | Penalty clause test — disproportionate to legitimate interest |
| *American Cyanamid v Ethicon* | [1975] AC 396 | Interim injunction principles — court retains discretion |
| *Hadley v Baxendale* | (1854) 9 Exch 341 | Remoteness of damages — two-limb test |
| *Faccenda Chicken v Fowler* | [1987] Ch 117 (CA) | Classification of confidential information in employment |
| *Vestergaard Frandsen v Bestnet* | [2013] UKSC 31 | Trade secret protection and springboard relief |

## Regulatory Guidance

- SRA Warning Notice on NDAs (March 2018, updated November 2019) — solicitors must not draft NDAs that restrict protected disclosures
- ICO Guide to the UK GDPR: Right of access — controller cannot refuse DSAR on grounds of contractual confidentiality
- ICO Guidance on Personal Data Breaches — 72-hour notification obligation overrides NDA restrictions
- CMA, Information sharing agreements guidance (OFT1389, adopted by CMA)
