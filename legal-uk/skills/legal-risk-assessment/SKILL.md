---
name: legal-risk-assessment
description: UK-specific legal risk classification workflow — severity x likelihood matrix calibrated to UK regulators (ICO, FCA, CMA, HSE, HMRC, Employment Tribunal). Covers penalty ranges, directors' duties, insurance requirements, and escalation criteria for SMBs.
argument-hint: "<describe the risk or scenario> — or ask about: risk-matrix, ico, fca, cma, hse, hmrc, tribunal, directors-duties, insurance, sanctions"
---

# Legal Risk Assessment — /legal-risk-assessment

> **DISCLAIMER:** This skill provides legal information for England & Wales only. It does not constitute legal advice and is not a substitute for instruction of a qualified solicitor regulated by the SRA. Verify all citations on [legislation.gov.uk](https://www.legislation.gov.uk). Law stated as at March 2026.

## Arguments

The user invoked this with: **$ARGUMENTS**

If the user describes a specific risk scenario, perform a full risk assessment using the workflow below. If the user asks a general question about UK regulatory enforcement or risk thresholds, answer using the reference knowledge in this skill.

## Response Constraints

1. **Cite only verified sources**: Only cite statutes, sections, and cases that appear in this skill document. Do not invent or generate case citations. If a relevant case is not in this skill, say: *"Case law generally supports this position — verify on BAILII or Westlaw UK."*
2. **Flag uncertainty explicitly**: Use phrases like *"as at March 2026"* or *"verify the current figure on legislation.gov.uk."*
3. **Issue-spotting, not advice**: Frame all outputs as issue identification — not as definitive legal advice.
4. **Scope boundaries**: If a query falls outside England & Wales, say so clearly.
5. **No fabricated citations**: If asked for a case or authority you cannot verify from this skill's content, say so.

---

## Risk Assessment Workflow

### Step 1: Describe the Risk

Identify: What is the specific legal or regulatory risk? What business activity does it relate to? Which regulator(s) or area of law is engaged?

### Step 2: Assess Severity (Impact)

| Level | Label | Description | £ Exposure Indicator |
|-------|-------|-------------|---------------------|
| 5 | **Critical** | Existential risk — criminal prosecution, unlimited fines, director disqualification, loss of regulatory licence, or insolvency | >£500k or unlimited |
| 4 | **High** | Major financial or reputational impact — regulatory fines £100k+, loss of key contracts, extended litigation | £100k–£500k |
| 3 | **Medium** | Significant but manageable — regulatory fines £10k–£100k, operational disruption, reputational damage | £10k–£100k |
| 2 | **Low** | Minor — regulatory warnings, small fines <£10k, limited operational disruption | <£10k |
| 1 | **Negligible** | De minimis — administrative inconvenience, no financial penalty | Nil |

### Step 3: Assess Likelihood (Probability)

| Level | Label | Description |
|-------|-------|-------------|
| 5 | **Almost Certain** | Expected to occur in the normal course of business |
| 4 | **Likely** | Will probably occur |
| 3 | **Possible** | Could occur |
| 2 | **Unlikely** | Not expected but could occur in exceptional circumstances |
| 1 | **Rare** | Would occur only in extraordinary circumstances |

### Step 4: Calculate Risk Score and Classify

**Risk Score = Severity × Likelihood** (range 1–25)

| Score | Level | Action |
|-------|-------|--------|
| 1–4 | **LOW** (GREEN) | Accept and monitor |
| 5–9 | **MODERATE** (YELLOW) | Implement mitigation; review periodically |
| 10–15 | **HIGH** (ORANGE) | Immediate mitigation required; consider insurance; schedule solicitor review |
| 16–25 | **CRITICAL** (RED) | Immediate solicitor engagement required; escalate to board/directors |

### Risk Matrix

```
                    LIKELIHOOD
                Rare  Unlikely  Possible  Likely  Almost Certain
                 (1)    (2)       (3)      (4)        (5)
SEVERITY
Critical (5)  |  5   |  10   |   15   |   20   |     25     |
High     (4)  |  4   |   8   |   12   |   16   |     20     |
Medium   (3)  |  3   |   6   |    9   |   12   |     15     |
Low      (2)  |  2   |   4   |    6   |    8   |     10     |
Negligible(1) |  1   |   2   |    3   |    4   |      5     |
```

### Step 5: Recommend Response

| Risk Level | Recommended Actions |
|------------|-------------------|
| **LOW** | Accept risk; document in risk register; include in periodic reviews (quarterly/annually) |
| **MODERATE** | Implement specific controls; assign owner; brief stakeholders; monitor monthly; define trigger events for escalation |
| **HIGH** | Escalate to senior management; develop mitigation plan; brief directors; consider outside solicitor; set weekly review cadence; consider insurance |
| **CRITICAL** | Immediate board escalation; instruct solicitor immediately; establish response team; consider insurance notification; activate crisis management if reputational risk; implement litigation hold if proceedings possible |

---

## UK Regulatory Enforcement Landscape

### ICO — Data Protection

**Jurisdiction**: UK GDPR, DPA 2018, PECR 2003, FOIA 2000.

**Penalty ranges**:
- **Higher maximum**: Up to **£17.5 million or 4% of total annual worldwide turnover** (whichever is higher) — for infringements of basic principles, consent conditions, data subject rights, international transfers (UK GDPR Art.83(5)–(6)).
- **Standard maximum**: Up to **£8.7 million or 2% of worldwide turnover** — for controller/processor obligation infringements (Art.83(4)).
- **PECR penalties**: Up to **£500,000** for unsolicited marketing breaches.
- **Criminal offences**: DPA 2018 ss.170-173 — obtaining/disclosing data without consent, re-identification of de-identified data, alteration to prevent DSAR disclosure. Punishable by fine on summary conviction.

*Citation*: UK GDPR Art.83(4)–(6); DPA 2018, ss.142, 146, 149, 155, 170-173; PECR, Reg.31.

**Risk calibration**:
- CRITICAL: Processing without lawful basis; systematic DSAR failures; large-scale unnotified breach; international transfers without safeguards
- HIGH: Data security failures exposing personal data; failure to conduct required DPIAs; non-compliance with ICO enforcement notice
- MEDIUM: Minor reported breaches; ROPA gaps; delayed DSAR responses
- LOW: Minor administrative non-compliance (e.g., delayed ICO registration renewal)

### FCA — Financial Services

**Jurisdiction**: FSMA 2000 — regulates banks, insurers, financial advisers, payment service providers.

**Penalty ranges**:
- **Financial penalties**: **Unlimited** (FSMA 2000, s.206).
- **Public censure**: FSMA 2000, s.205.
- **Permission variation/cancellation**: FSMA 2000, ss.55J–55K.
- **Prohibition orders**: FSMA 2000, s.56 — prohibit individuals from regulated functions.
- **Criminal prosecution**: Market abuse, insider dealing (Criminal Justice Act 1993, Part V), misleading statements (Financial Services Act 2012, s.89).

*Citation*: FSMA 2000, ss.56, 205, 206, 380–386; FCA Handbook, DEPP.

**Risk calibration**:
- CRITICAL: Carrying on regulated activities without authorisation (criminal offence, FSMA s.23); market abuse; insider dealing
- HIGH: Significant TCF failings; inadequate systems and controls; approved person misconduct
- MEDIUM: Minor rule breaches identified in supervisory review; late regulatory returns
- LOW: Administrative non-compliance

### CMA — Competition

**Jurisdiction**: Competition Act 1998, Enterprise Act 2002.

**Penalty ranges**:
- **Competition infringement fines**: Up to **10% of worldwide turnover** (Competition Act 1998, s.36).
- **Director disqualification**: Competition Disqualification Order up to **15 years** (Company Directors Disqualification Act 1986, s.9A).
- **Criminal cartel offence**: Up to **5 years' imprisonment and/or unlimited fine** (Enterprise Act 2002, s.188, as amended by Enterprise and Regulatory Reform Act 2013, s.47).

*Citation*: Competition Act 1998, s.36; Enterprise Act 2002, s.188; CMA73 (penalty guidance, April 2018).

**Risk calibration**:
- CRITICAL: Cartel participation (criminal offence); abuse of dominant position; gun-jumping in merger control
- HIGH: Anti-competitive agreements (vertical/horizontal); failure to notify qualifying merger
- MEDIUM: Information sharing with competitors without safeguards
- LOW: Minor competition compliance gaps

### HSE — Health and Safety

**Jurisdiction**: Health and Safety at Work etc. Act 1974 (HSWA 1974).

**Penalty ranges** (per Sentencing Council guidelines, effective 1 February 2016):
- **Unlimited fines** for serious offences.
- Very large organisations (turnover £50M+): Category 1: £1.6M–£20M+; Category 2: £800k–£4M.
- Large organisations (£10M–£50M): Category 1: £550k–£4M; Category 2: £200k–£1.6M.
- **Corporate manslaughter** (Corporate Manslaughter and Corporate Homicide Act 2007): **unlimited fine**.
- **Imprisonment**: Up to **2 years** for individual officers (HSWA 1974, s.33).

*Citation*: HSWA 1974, ss.21-22, 33; Sentencing Council guidelines (2016); Corporate Manslaughter Act 2007.

### HMRC — Tax

**Penalty ranges**:
- **Late filing**: CT return: £100 initial, £200 after 3 months, 10% of unpaid tax after 6 months (Finance Act 1998, Sch 18, para 17). SA return: £100 initial + daily penalties.
- **Late payment**: 5% of unpaid tax after 30 days; further 5% after 6 months; further 5% after 12 months (Finance Act 2009, Sch 56).
- **Inaccuracies**: Careless: 0–30% of potential lost revenue. Deliberate: 20–70%. Deliberate and concealed: 30–100% (Finance Act 2007, Sch 24).
- **Criminal prosecution**: Tax evasion (common law cheating the public revenue; Fraud Act 2006). **Failure to prevent facilitation of tax evasion** (Criminal Finances Act 2017, ss.45-46): strict liability corporate offence, **unlimited fine**.

*Citation*: Finance Act 1998, Sch 18; Finance Act 2007, Sch 24; Finance Act 2009, Sch 56; Criminal Finances Act 2017, ss.45-46.

### Employment Tribunal

**Key financial thresholds (2025/26 — verify current figures)**:
- **Unfair dismissal compensatory award cap**: Lower of 52 weeks' pay or statutory cap (circa £115,115 as at April 2025 — verify via Employment Rights (Increase of Limits) Order).
- **Basic award**: 0.5–1.5 weeks' pay per year of service (max 20 years). Weekly pay cap circa £700.
- **Discrimination claims**: **Unlimited** compensation. Vento bands for injury to feelings: Lower: £1,200–£11,200; Middle: £11,200–£33,700; Upper: £33,700–£56,200; exceptional cases may exceed upper band.
- **Whistleblowing dismissal** (ERA 1996, s.103A): **No cap** on compensation.
- **ACAS uplift**: Up to 25% increase/decrease for unreasonable failure to follow ACAS Code (TULR(C)A 1992, s.207A).

*Citation*: ERA 1996, ss.119-120, 124, 227; Vento v Chief Constable of West Yorkshire Police (No 2) [2003] EWCA Civ 1871; Presidential Guidance on Vento bands.

**Risk calibration**:
- CRITICAL: Systemic discrimination claims; whistleblowing detriment (no cap); pregnancy/maternity discrimination (no cap)
- HIGH: Individual unfair dismissal with high compensatory award; upper Vento band discrimination
- MEDIUM: Straightforward unfair dismissal; unauthorised deduction from wages
- LOW: Minor procedural disputes; ACAS early conciliation resolving claim

### Companies House

**Penalty ranges**:
- **Late filing penalties** (automatic civil penalties): Private companies: £150 (≤1 month), £375 (1–3 months), £750 (3–6 months), £1,500 (>6 months). Doubled if late for two successive years.
- **Compulsory strike-off**: CA 2006, s.1000.
- **Criminal offences**: Failure to file confirmation statement is a criminal offence (CA 2006, s.858).
- **ECCTA 2023**: Identity verification requirements; enhanced registrar powers; new corporate offence of failure to prevent fraud.

*Citation*: Companies (Late Filing Penalties) Regulations 2008 (SI 2008/497); CA 2006, ss.858, 1000; ECCTA 2023.

### Environment Agency

- **Unlimited fines** for serious environmental offences (Environmental Permitting Regulations 2016).
- **Imprisonment**: Up to 5 years on conviction on indictment.

*Citation*: Environmental Permitting (England and Wales) Regulations 2016 (SI 2016/1154).

### OFSI — Sanctions

- **Monetary penalties**: Strict liability. Maximum: greater of **£1 million or 50% of estimated value** of breach.
- **Criminal penalties**: Up to **7 years' imprisonment** and/or unlimited fine.

*Citation*: Sanctions and Anti-Money Laundering Act 2018; OFSI General Guidance (HM Treasury, updated 2024).

---

## Directors' Duties and Corporate Liability

### Directors' Duties (CA 2006, ss.171–177)

1. **s.171**: Act within powers
2. **s.172**: Promote success of the company (having regard to long-term consequences, employees, business relationships, community/environment, reputation, fairness between members)
3. **s.173**: Exercise independent judgment
4. **s.174**: Exercise reasonable care, skill, and diligence (objective + subjective standard)
5. **s.175**: Avoid conflicts of interest
6. **s.176**: Do not accept benefits from third parties
7. **s.177**: Declare interest in proposed transactions

### Wrongful Trading (IA 1986, s.214)

Director personally liable if company goes into insolvent liquidation and director knew or ought to have concluded there was no reasonable prospect of avoiding insolvent liquidation, and did not take every step to minimise loss to creditors.

### ECCTA 2023 — Failure to Prevent Fraud

"Large organisations" (meeting two of three: turnover >£36M, balance sheet >£18M, >250 employees) — guilty of offence if associated person commits specified fraud offence intending to benefit the organisation. Defence: reasonable fraud prevention procedures.

*Citation*: ECCTA 2023, Part 5.

---

## Insurance Requirements

### Compulsory Insurance

| Type | Requirement | Authority |
|------|------------|-----------|
| Employers' liability | Minimum £5M per claim; failure to insure = criminal offence (fine up to £2,500/day) | Employers' Liability (Compulsory Insurance) Act 1969 |
| Motor insurance | Third-party minimum | Road Traffic Act 1988, s.143 |
| Professional indemnity | Required for solicitors (SRA Rules), accountants, architects, financial advisers | Various |

### Standard Voluntary Insurance

- **Public liability**: £1–10M typical cover
- **Product liability**: Standard for manufacturers/distributors (Consumer Protection Act 1987)
- **D&O liability**: Standard for companies with external directors/investors
- **Cyber insurance**: Increasingly standard post-UK GDPR

### Insurability of Regulatory Fines

Under English law, criminal fines are **not insurable** (public policy — *Askey v Golden Wine Co Ltd* [1948] 2 All ER 35). Civil penalties (such as ICO monetary penalty notices) **may** be insurable — many cyber policies cover regulatory fines "where insurable by law." Position untested in courts for ICO fines specifically.

---

## Risk Assessment Output Format

```
## Legal Risk Assessment

**Date**: [assessment date]
**Risk Description**: [clear description]
**Regulator/Area**: [which regulator or area of law]

### Severity: [1–5] — [Label]
[Rationale — including potential £ exposure based on UK penalty ranges above]

### Likelihood: [1–5] — [Label]
[Rationale — including precedent, triggering events, current conditions]

### Risk Score: [Score] — [LOW/MODERATE/HIGH/CRITICAL]

### What This Means for Your Business
[Plain-English explanation of the risk, the worst-case scenario, and realistic likely outcome]

### Contributing Factors
[What increases the risk]

### Mitigating Factors
[What decreases the risk or limits exposure]

### Recommended Actions
| Action | Effectiveness | Cost/Effort | Recommended? |
|--------|-------------|-------------|--------------|
| [Action 1] | [High/Med/Low] | [High/Med/Low] | [Yes/No] |
| [Action 2] | ... | ... | ... |

### Insurance Considerations
[Is insurance available? What type? Is the potential penalty insurable?]

### When to Instruct a Solicitor
[Specific trigger — e.g., "if you receive a letter from the ICO," "before responding to the enforcement notice"]

### Monitoring Plan
[How and how often to review; trigger events for re-assessment]
```

---

## Quick Reference: Maximum Penalties by Regulator

| Regulator / Legislation | Maximum Penalty | Key Threshold |
|------------------------|----------------|---------------|
| ICO (UK GDPR — higher tier) | £17.5M or 4% global turnover | Any processing of personal data |
| ICO (UK GDPR — standard tier) | £8.7M or 2% global turnover | Controller/processor obligations |
| ICO (PECR) | £500,000 | Unsolicited electronic marketing |
| FCA | Unlimited | Regulated financial services |
| CMA | 10% global turnover | Competition infringements |
| CMA (criminal cartel) | 5 years imprisonment + unlimited fine | Cartel participation |
| HSE | Unlimited (Sentencing Council) | Health and safety offences |
| HMRC (inaccuracies) | Up to 100% of potential lost revenue | Tax returns |
| HMRC (criminal — tax evasion) | Unlimited fine + imprisonment | Tax evasion |
| Criminal Finances Act 2017 | Unlimited fine | Failure to prevent tax evasion facilitation |
| ECCTA 2023 | Unlimited fine | Failure to prevent fraud (large orgs) |
| OFSI (sanctions) | Greater of £1M or 50% of breach value | Financial sanctions breach |
| Companies House (late accounts) | £150–£7,500 (doubled for repeat) | Late filing |
| Employment Tribunal (unfair dismissal) | Statutory cap (~£115k) | Unfair dismissal |
| Employment Tribunal (discrimination) | Unlimited | Discrimination claims |
| Bribery Act 2010 (corporate) | Unlimited fine | Failure to prevent bribery |
| Corporate Manslaughter Act 2007 | Unlimited fine | Corporate manslaughter |
| Modern Slavery Act 2015 | Civil injunctions; director disqualification | Turnover >£36M |
