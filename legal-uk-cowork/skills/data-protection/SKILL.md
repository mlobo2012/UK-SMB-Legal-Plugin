---
name: data-protection
description: UK GDPR and Data Protection Act 2018 guidance — lawful bases, data subject rights, breach notification (72hr), DPIAs, international transfers (IDTA), ICO enforcement, PECR cookie consent, and Children's Code.
user-invocable: true
argument-hint: "<topic> — topics: lawful-basis, rights, breach, dpia, transfers, ico, pecr, children, processor"
allowed-tools: [Read, Glob, Grep]
---

# Data Protection & Privacy — /data-protection

> **DISCLAIMER:** Legal information for **England & Wales** only. Not legal advice.
> Verify on [legislation.gov.uk](https://www.legislation.gov.uk) and [ico.org.uk](https://ico.org.uk).
> UK GDPR = retained EU GDPR as amended by the DPPEC (EU Exit) Regulations 2019.

---

## 1. UK GDPR Principles (Article 5)

All processing of personal data must comply with seven principles (UK GDPR Art 5(1)-(2)):

| # | Principle | Article | Summary |
|---|-----------|---------|---------|
| 1 | **Lawfulness, fairness and transparency** | Art 5(1)(a) | Process lawfully under Art 6, fairly, and transparently via privacy notices. |
| 2 | **Purpose limitation** | Art 5(1)(b) | Collect for specified, explicit, legitimate purposes; no incompatible further processing. |
| 3 | **Data minimisation** | Art 5(1)(c) | Adequate, relevant, and limited to what is necessary. |
| 4 | **Accuracy** | Art 5(1)(d) | Keep personal data accurate and up to date; erase or rectify without delay. |
| 5 | **Storage limitation** | Art 5(1)(e) | Keep in identifiable form no longer than necessary; document retention periods. |
| 6 | **Integrity and confidentiality** | Art 5(1)(f) | Appropriate technical and organisational security measures. |
| 7 | **Accountability** | Art 5(2) | The controller must demonstrate compliance with all principles. |

---

## 2. Six Lawful Bases (Article 6(1))

Every act of processing requires **exactly one** lawful basis identified **before** processing begins.

| Basis | Article | Key requirement |
|-------|---------|-----------------|
| **Consent** | Art 6(1)(a) | Freely given, specific, informed, unambiguous; affirmative act; withdrawable at any time (Art 7). |
| **Contract** | Art 6(1)(b) | Necessary for performance of a contract with the data subject, or pre-contractual steps at their request. |
| **Legal obligation** | Art 6(1)(c) | Necessary to comply with a legal obligation on the controller (UK or retained EU law). |
| **Vital interests** | Art 6(1)(d) | Necessary to protect life of data subject or another person. Use only where no other basis applies. |
| **Public task** | Art 6(1)(e) | Necessary for a task in the public interest or official authority vested in the controller. |
| **Legitimate interests** | Art 6(1)(f) | Necessary for legitimate interests of controller or third party, unless overridden by data subject rights. Requires a documented Legitimate Interests Assessment (LIA). Not available to public authorities for core tasks. |

### GUIDED LAWFUL BASIS SELECTOR

Use the following decision workflow to identify the correct lawful basis. Work through each question in order, and recommend the **first** basis whose conditions are fully met.

```
STEP 1 — Is there a UK or retained-EU legal obligation requiring you to process this data?
  YES -> Lawful basis: LEGAL OBLIGATION (Art 6(1)(c)).
         Document the specific statutory provision.
  NO  -> Proceed to Step 2.

STEP 2 — Is the processing necessary to protect someone's life in an emergency,
          and no other basis can reasonably apply?
  YES -> Lawful basis: VITAL INTERESTS (Art 6(1)(d)).
         Record why no alternative basis was available.
  NO  -> Proceed to Step 3.

STEP 3 — Are you a public authority processing data for your official functions?
  YES -> Lawful basis: PUBLIC TASK (Art 6(1)(e)).
         Identify the specific statutory or common-law function.
  NO  -> Proceed to Step 4.

STEP 4 — Is the processing necessary to perform or enter into a contract with the
          data subject?
  (a) Is there an existing contract with the data subject? Or
  (b) Has the data subject asked you to take pre-contractual steps?
  AND is the processing genuinely necessary for that contract (not merely useful)?
  YES to (a) or (b) AND necessity -> Lawful basis: CONTRACT (Art 6(1)(b)).
  NO  -> Proceed to Step 5.

STEP 5 — Legitimate Interests Assessment (LIA):
  (a) Identify the legitimate interest (yours or a third party's).
  (b) Is the processing necessary to achieve it? (No less intrusive alternative?)
  (c) Balance: do the individual's interests, rights, or freedoms override?
      Consider: nature of data, reasonable expectations, relationship,
      vulnerability, safeguards, impact on individual.
  If (a)+(b) satisfied AND individual rights do NOT override ->
      Lawful basis: LEGITIMATE INTERESTS (Art 6(1)(f)).
      Document the full LIA.
  Otherwise -> Proceed to Step 6.

STEP 6 — CONSENT (Art 6(1)(a)):
  If none of the above apply, or if you want to give the data subject full control:
  - Can consent be freely given (no imbalance of power, no conditionality)?
  - Can you provide granular, specific information about each purpose?
  - Can the individual genuinely refuse or withdraw without detriment?
  YES to all -> Lawful basis: CONSENT. Implement GDPR-compliant consent mechanism.
  NO  -> STOP. You may not have a lawful basis. Seek specialist legal advice.
```

> **ICO Guidance:** See ICO's "Lawful basis interactive guidance tool" at
> ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/lawful-basis/

---

## 3. Special Category Data (Article 9)

Processing **special category data** is prohibited (Art 9(1)) unless:
- A **lawful basis** under Art 6(1) is identified, **AND**
- An **Art 9(2) condition** applies, **AND**
- A **DPA 2018 Schedule 1 condition** is met (where required by UK law).

### The 10 Special Categories (Art 9(1))

1. Racial or ethnic origin
2. Political opinions
3. Religious or philosophical beliefs
4. Trade union membership
5. Genetic data
6. Biometric data (for identification purposes)
7. Health data
8. Sex life
9. Sexual orientation
10. Criminal conviction and offence data (Art 10 — treated similarly; DPA 2018 s11 and Sch 1)

### Common Art 9(2) Conditions

(a) Explicit consent; (b) Employment/social security/social protection law (requires DPA 2018 Sch 1 para 1); (c) Vital interests (subject incapable of consenting); (d) Not-for-profit legitimate activities (members only); (e) Manifestly made public by subject; (f) Legal claims/judicial acts; (g) Substantial public interest (requires Sch 1 Part 2 — 23 specific conditions); (h) Health or social care (health professional; Sch 1 para 2); (i) Public health; (j) Archiving, research, statistics (Sch 1 para 4).

> **DPA 2018 Schedule 1** imposes an "appropriate policy document" requirement for
> conditions (b), (g), (h), and (j). Retain and review the policy document regularly.

---

## 4. Data Subject Rights

Controllers must facilitate the exercise of rights (Art 12). Response deadline: **one calendar month** from receipt, extendable by two further months for complex/numerous requests (Art 12(3)).

| Right | Article | Key points |
|-------|---------|------------|
| **Right of access** (SAR) | Art 15 | Copy of personal data, processing purposes, recipients, retention period, source. Free of charge; may charge reasonable fee for manifestly unfounded/excessive requests. |
| **Right to rectification** | Art 16 | Correct inaccurate data; complete incomplete data (supplementary statement). |
| **Right to erasure** ("right to be forgotten") | Art 17 | Applies where: consent withdrawn, data no longer necessary, objection upheld, unlawful processing, legal obligation to erase, children's online data. Does NOT override legal obligations to retain. |
| **Right to restriction** | Art 18 | "Freeze" processing while accuracy contested, processing unlawful but erasure opposed, controller no longer needs data but subject needs it for legal claims, or pending objection verification. |
| **Right to data portability** | Art 20 | Machine-readable, structured, commonly used format. Only applies where basis is consent or contract AND processing is automated. |
| **Right to object** | Art 21 | Object to processing based on public task (Art 6(1)(e)) or legitimate interests (Art 6(1)(f)). Must stop unless compelling legitimate grounds demonstrated. Absolute right to object to direct marketing — no exceptions. |
| **Automated decision-making** | Art 22 | Right not to be subject to decisions based solely on automated processing (including profiling) producing legal or similarly significant effects. Must provide meaningful information about the logic, significance, and envisaged consequences. |

### SAR Workflow

1. **Verify identity** (Art 12(6)) -> 2. **Log receipt date** (clock starts next day) -> 3. **Clarify scope** if broad (cannot require narrowing) -> 4. **Search** all systems -> 5. **Redact** third-party data -> 6. **Respond** within one calendar month with data, Art 15(1) info, and right to complain to ICO. Extension: notify within first month with reasons.

---

## 5. Breach Notification (Articles 33–34)

A **personal data breach** means a breach of security leading to accidental or unlawful destruction, loss, alteration, unauthorised disclosure of, or access to, personal data (Art 4(12)).

### Notification to the ICO (Art 33)

- **Deadline:** Not later than **72 hours** after becoming aware of the breach.
- **Exception:** Unless the breach is unlikely to result in a risk to individuals' rights and freedoms.
- If notification is delayed beyond 72 hours, provide reasons for the delay.
- **Content** (Art 33(3)): Nature of breach, categories and approximate number of subjects and records, DPO or contact point, likely consequences, measures taken or proposed.
- Report via the ICO's online breach reporting tool at ico.org.uk.

### Notification to Data Subjects (Art 34)

- Without undue delay where breach is likely to result in **high risk** to rights and freedoms.
- **Exceptions** (Art 34(3)): data rendered unintelligible (encryption), subsequent measures eliminate high risk, or disproportionate effort (use public communication).
- Clear plain language: nature of breach, DPO contact, consequences, measures taken.

### Breach Assessment Workflow

```
STEP 1 — Confirm: Is this a personal data breach?
  - Was there unauthorised access, loss, destruction, alteration, or disclosure of personal data?
  YES -> Continue. NO -> Not a reportable breach (but document the incident).

STEP 2 — Assess risk to individuals:
  Consider: type of data (special category? financial? children?), volume,
  identifiability, severity of consequences, special characteristics of subjects.
  (a) Unlikely to result in risk     -> Document internally (Art 33(5)). No ICO report required.
  (b) Risk to rights and freedoms    -> Report to ICO within 72 hours (Step 3).
  (c) HIGH risk to rights and freedoms -> Report to ICO (Step 3) AND notify data subjects (Step 4).

STEP 3 — Notify ICO (within 72 hours of awareness):
  Use ico.org.uk online reporting tool. Provide all Art 33(3) information.
  If you cannot provide full details, make a phased report.

STEP 4 — Notify data subjects (without undue delay):
  Plain-language communication. Include: nature, DPO contact, consequences, mitigation steps.
  Check if any Art 34(3) exception applies.

STEP 5 — Document everything:
  Maintain a breach register recording: facts, effects, remedial action taken (Art 33(5)).
  This register is subject to ICO audit.
```

---

## 6. Data Protection Impact Assessments (Article 35)

A DPIA is **mandatory** before processing that is likely to result in a **high risk** to individuals.

### When Is a DPIA Required?

A DPIA is required where processing involves (Art 35(3)):
- (a) Systematic and extensive profiling with significant effects;
- (b) Large-scale processing of special category data or criminal offence data;
- (c) Systematic monitoring of a publicly accessible area on a large scale.

The ICO's published list of processing operations requiring a DPIA (Art 35(4)) includes: innovative technology combined with any Art 35(3) criterion; denial-of-service decisions; large-scale profiling; biometric or genetic data processing; data matching/combining from multiple sources; invisible processing (data from third parties); tracking location or behaviour; targeting children or vulnerable individuals; risk of physical harm if data misused.

### Mandatory DPIA Content (Art 35(7))

1. Systematic description of the processing operations and purposes;
2. Assessment of necessity and proportionality in relation to the purposes;
3. Assessment of risks to rights and freedoms of data subjects;
4. Measures to address the risks (safeguards, security, mechanisms for compliance).

### ICO Screening Checklist

Answer the following — **two or more "yes" answers** strongly indicate a DPIA is required:

1. Evaluation/scoring of individuals? 2. Automated decision-making with legal/significant effects? 3. Systematic monitoring? 4. Special category or criminal offence data? 5. Large-scale processing? 6. Datasets matched or combined? 7. Vulnerable data subjects (children, employees, patients)? 8. Innovative technology? 9. International transfers? 10. Processing that prevents subjects exercising a right or using a service?

Document your screening decision either way.

> **Consultation:** If residual high risk remains after mitigation, you must consult the ICO
> before processing (Art 36 — prior consultation).

---

## 7. International Transfers (Chapter V, Arts 44–49)

Transferring personal data outside the UK requires a **transfer mechanism** unless the destination has an **adequacy decision**.

### Adequacy Decisions (Art 45)

The UK Secretary of State may determine that a third country ensures an adequate level of protection. As of the UK GDPR's retained form, the following jurisdictions have UK adequacy regulations:
- The EEA (EU/EEA member states)
- Specific additional countries assessed by the UK government (see current list at ico.org.uk)

Adequacy decisions are reviewed periodically.

### International Data Transfer Agreement (IDTA)

- The **UK IDTA** came into effect on **21 March 2022** (laid before Parliament under DPA 2018 s119A).
- It replaces the old EU SCCs for UK transfers.
- Available as a standalone agreement or as a **UK Addendum** to the EU SCCs.
- Must be completed with the specific details of each transfer (Annex tables).

### Other Transfer Mechanisms

- **UK IDTA / UK Addendum to EU SCCs** (Art 46(2)(c)) — standard mechanism for most commercial transfers.
- **Binding Corporate Rules** (Art 47) — intra-group transfers; requires ICO approval.
- **Approved code of conduct** (Art 46(2)(e)) or **certification** (Art 46(2)(f)) — with binding commitments.
- **Derogations** (Art 49) — explicit consent, contract necessity, public interest, legal claims, vital interests. Strictly interpreted; not for routine transfers.

### Post-Brexit Position

- The UK is an independent jurisdiction; **not** bound by EU adequacy decisions.
- EU granted the UK a time-limited adequacy decision (28 June 2021). UK-to-EU transfers rely on UK adequacy regulations recognising the EEA.
- The **UK Extension to the EU-US Data Privacy Framework** covers transfers to certified US organisations.
- Even with an IDTA, conduct a **Transfer Risk Assessment (TRA)** of the destination country's laws.

---

## 8. PECR 2003 (Privacy and Electronic Communications Regulations)

The Privacy and Electronic Communications (EC Directive) Regulations 2003 (SI 2003/2426) sit alongside the UK GDPR and govern electronic communications.

### Cookies and Similar Technologies (Reg 6)

- **Prior informed consent** required before placing non-essential cookies. Pre-ticked boxes are insufficient.
- **Strictly necessary** cookies (shopping basket, authentication, security) are exempt.
- Consent must meet UK GDPR standard: freely given, specific, informed, unambiguous affirmative action.
- Provide clear information: what cookies, purpose, who sets them, how to manage/withdraw consent.

### Electronic Marketing (Regs 21–24)

| Type | Rule | Detail |
|------|------|--------|
| **Email/SMS/MMS to individuals** | Opt-in required (Reg 22) | Prior consent before sending unsolicited direct marketing. |
| **Soft opt-in exception** | Reg 22(3) | Existing customers who gave their details during a sale/negotiation, marketing is for similar products/services, given a simple opt-out at collection and in every message. |
| **Email/SMS to corporate subscribers** | No prior consent needed | But must identify the sender and provide an opt-out. |
| **Telephone marketing to individuals** | Opt-out via TPS (Reg 21) | Do not call numbers on the Telephone Preference Service register unless you have specific consent. |
| **Automated calling systems** | Opt-in required (Reg 19) | Prior consent mandatory. |
| **Fax marketing to individuals** | Opt-in required (Reg 20) | Prior consent; also check the Fax Preference Service. |

> **Enforcement:** PECR breaches are enforced by the ICO. Maximum penalty for PECR breaches
> is £500,000 under the current PECR fine regime (as amended by SI 2011/1208).

---

## 9. Children's Code (Age Appropriate Design Code)

The **Age Appropriate Design Code** (also known as the Children's Code) is a statutory code of practice under DPA 2018 s123. It came into force on **2 September 2021**.

### Scope

- Applies to **Information Society Services** (online services) likely to be accessed by children (under 18 in the UK).
- Includes apps, games, social media, online marketplaces, streaming services, educational websites, connected toys, and news sites.

### The 15 Standards

| # | Standard | Requirement |
|---|----------|-------------|
| 1 | Best interests of the child | Make the best interests of the child a primary consideration in design. |
| 2 | Data protection impact assessments | Undertake a DPIA for any service likely to be accessed by children. |
| 3 | Age-appropriate application | Consider the ages of your users and apply the standards to the age ranges you serve. |
| 4 | Transparency | Provide privacy information in age-appropriate language, using formats children understand (e.g., visuals, audio). |
| 5 | Detrimental use of data | Do not use children's personal data in ways detrimental to their health or wellbeing. |
| 6 | Policies and community standards | Uphold published terms, policies, and community standards. |
| 7 | Default settings | **High privacy by default.** Settings must be high privacy unless there is a compelling reason otherwise, taking account of the best interests of the child. |
| 8 | Data minimisation | Collect and retain only the minimum amount of personal data needed. |
| 9 | Data sharing | Do not disclose children's data unless there is a compelling reason to do so. |
| 10 | Geolocation | Switch geolocation off by default. Provide an obvious sign when location tracking is active. |
| 11 | Parental controls | If you provide parental controls, give the child age-appropriate information about them. |
| 12 | Profiling | Switch off profiling by default, unless there is a compelling reason. |
| 13 | Nudge techniques | Do not use nudge techniques to lead children to provide unnecessary personal data or weaken privacy protections. |
| 14 | Connected toys and devices | If a connected toy or device, apply these standards and provide effective conformity tools. |
| 15 | Online tools | Provide prominent, accessible tools to help children exercise their data protection rights and report concerns. |

> **ICO Enforcement:** The Children's Code is enforceable by the ICO under
> its full range of DPA 2018 / UK GDPR powers, including fines up to £17.5M or 4% of
> worldwide turnover.

---

## 10. ICO Enforcement Powers

The Information Commissioner's Office (ICO) is the UK's independent supervisory authority for data protection (DPA 2018 s114).

### Monetary Penalties (DPA 2018 s155–s157; UK GDPR Art 83)

| Tier | Maximum | Applies to |
|------|---------|------------|
| **Higher maximum** | **£17,500,000** or **4% of total annual worldwide turnover** (whichever is higher) | Infringements of processing principles, lawful basis conditions, data subject rights, international transfer rules. |
| **Standard maximum** | **£8,700,000** or **2% of total annual worldwide turnover** (whichever is higher) | Infringements of controller/processor obligations, certification body obligations, monitoring body obligations. |

### Other Enforcement Tools

- **Information notice** (s142) — compel provision of information to the ICO.
- **Assessment notice** (s146) — authorise ICO compliance assessment.
- **Enforcement notice** (s149) — require specified compliance steps.
- **Penalty notice** (s155) — impose monetary penalty.
- **Reprimand** (Art 58(2)(b)) — formal censure without fine.
- **Criminal offences** (ss170-173) — unlawful obtaining/disclosing (s170), re-identification (s171), alteration to prevent SAR disclosure (s173).
- **Undertakings** — voluntary commitments to remedial action.

> **Appeals:** Penalty and enforcement notices may be appealed to the
> First-tier Tribunal (General Regulatory Chamber) (DPA 2018 s162).

---

## 11. Records of Processing Activities (Article 30)

### Who Must Maintain Records?

Article 30 records (ROPA) are mandatory for:
- Organisations with **250 or more employees**; **OR**
- **Any** organisation (regardless of size) where processing:
  - Is not occasional, **OR**
  - Includes special category data (Art 9(1)) or criminal offence data (Art 10), **OR**
  - Is likely to result in a risk to the rights and freedoms of data subjects.

In practice, the ICO recommends **all** organisations maintain a ROPA.

### Controller Records Must Include (Art 30(1))

1. Name and contact details of the controller (and DPO, if applicable);
2. Purposes of the processing;
3. Categories of data subjects and categories of personal data;
4. Categories of recipients (including in third countries or international organisations);
5. Transfers to third countries (including documentation of safeguards);
6. Envisaged time limits for erasure (retention periods);
7. General description of technical and organisational security measures (Art 32(1)).

### Processor Records Must Include (Art 30(2))

1. Name and contact details of the processor(s) and each controller on whose behalf they act;
2. Categories of processing carried out on behalf of each controller;
3. Transfers to third countries (with safeguards documentation);
4. General description of technical and organisational security measures.

---

## Data Processor Obligations — Summary

Processors have direct statutory obligations under Art 28(3), Art 30(2), Art 32, Art 33(2), Art 37, and Art 27. Key duties: process only on documented controller instructions (Art 28(3)(a)); ensure personnel confidentiality; implement appropriate security (Art 32); obtain prior authorisation for sub-processors with equivalent contractual terms (Art 28(2),(4)); assist with DSR requests, DPIAs, and prior consultation; delete or return data at contract end; permit audits; notify controller of breaches without undue delay; maintain Art 30(2) records; appoint a DPO where required; designate a UK representative if established outside the UK.

> **Contractual requirement:** Art 28(3) mandates a written contract covering subject-matter,
> duration, nature, purpose, data types, categories of data subjects, and controller rights.

---

## Key Legislative References

- **UK GDPR** — Regulation (EU) 2016/679 as retained and amended by DPPEC Regulations 2019
- **Data Protection Act 2018** — 2018 c. 12
- **PECR 2003** — SI 2003/2426, as amended
- **IDTA** — under DPA 2018 s119A; effective 21 March 2022
- **UK Addendum to EU SCCs** — effective 21 March 2022
- **Age Appropriate Design Code** — DPA 2018 s123; in force 2 September 2021

> **Sources:** [legislation.gov.uk](https://www.legislation.gov.uk), [ico.org.uk](https://ico.org.uk)
