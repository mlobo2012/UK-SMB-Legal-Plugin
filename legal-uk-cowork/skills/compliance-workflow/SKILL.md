---
name: compliance-workflow
description: UK GDPR / DPA 2018 compliance workflow with ICO-specific steps, DPIA, DSAR, breach notification, international transfers, PECR direct marketing, and Children's Code
---

# UK Data Protection Compliance Workflow

> **SRA Regulatory Notice**: This skill provides general legal information about UK data protection law for educational purposes only. It does not constitute legal advice, and no solicitor-client relationship is created. Data protection compliance involves fact-specific assessments that require professional judgement. **You should instruct a solicitor or qualified data protection practitioner before making compliance decisions that could expose your business to ICO enforcement action.** The information reflects the law of England & Wales. Where the Data Protection and Digital Information Act 2024 (DPDIA 2024) may affect a requirement, this is noted — verify commencement status of specific DPDIA provisions before relying on them.

---

## 1. Workflow Overview

This workflow guides UK SMB owners through data protection compliance under the **UK GDPR** and the **Data Protection Act 2018 (DPA 2018)**, with ICO-specific steps rather than generic EU GDPR guidance.

### 1.1 When to Use This Workflow

- Setting up a new business that processes personal data
- Launching a new product, service, or marketing campaign involving personal data
- Responding to a data subject access request (DSAR)
- Handling a personal data breach
- Transferring personal data outside the UK
- Reviewing whether your existing practices comply with current requirements
- Preparing for an ICO audit or responding to an ICO enquiry

### 1.2 UK GDPR vs EU GDPR — Key Differences

The UK GDPR is the retained version of EU Regulation 2016/679, as amended by SI 2019/419. Key differences:

| Area | UK GDPR | EU GDPR |
|------|---------|---------|
| Supervisory authority | ICO (sole UK authority) | National DPAs + EDPB |
| Maximum fines | £17.5 million / 4% of turnover | €20 million / 4% of turnover |
| Lower-tier fines | £8.7 million / 2% of turnover | €10 million / 2% of turnover |
| Transfer mechanisms | UK IDTA / UK Addendum to EU SCCs | EU SCCs |
| Age of consent (ISS) | 13 (DPA 2018 s.9) | 16 (Member State discretion to 13) |
| UK representative | Required for non-UK controllers targeting UK data subjects (Art.27) | EU representative required |
| UK-specific exemptions | Immigration, national security, intelligence services (DPA 2018) | Member State derogations |

*Citation*: UK GDPR Art.8(1) (as modified by DPA 2018 s.9); SI 2019/419.

---

## 2. Compliance Assessment Workflow

Follow these steps in order. Each step includes the regulatory basis, what you need to do, and the ICO resource to use.

### Step 1: ICO Registration

**Requirement**: Most organisations processing personal data must pay an annual data protection fee to the ICO under the Data Protection (Charges and Information) Regulations 2018 (SI 2018/480).

**Fee tiers**:

| Tier | Annual Fee | Eligibility |
|------|-----------|-------------|
| Tier 1 | £40 | Turnover ≤ £632,000 AND ≤ 10 staff (or charity ≤ 10 staff) |
| Tier 2 | £60 | Turnover ≤ £36 million AND ≤ 250 staff (or charity ≤ 250 staff) |
| Tier 3 | £2,900 | Turnover > £36 million OR > 250 staff |

**Exemptions**: Individuals processing for personal/family/household purposes; organisations processing only for staff administration (payroll, pensions); elected representatives for constituency purposes.

**Penalty for non-registration**: Failure to pay is a criminal offence (DPA 2018 s.108). The ICO can issue a fixed penalty notice of £400 (reduced to £320 if paid within 28 days).

**Action**: Register at the ICO registration portal (ico.org.uk). Keep your registration number on file and set a calendar reminder for annual renewal.

*Citation*: SI 2018/480; DPA 2018 s.108; ICO, "Register with the ICO" (ico.org.uk).

---

### Step 2: Appoint a Data Protection Lead or DPO

**When a DPO is mandatory** (UK GDPR Art.37):
- You are a public authority or body
- Your core activities involve regular and systematic monitoring of data subjects on a large scale
- Your core activities involve large-scale processing of special category data (Art.9) or criminal offence data (Art.10)

**ICO guidance on "core activities"**: Primary business activities, not ancillary functions. A hospital's core activity is healthcare (DPO required). An office managing HR data — that's ancillary (DPO may not be required solely on that basis).

**ICO guidance on "large scale"**: Assessed by number of data subjects, volume of data, range of data items, duration, and geographical extent. No specific numerical threshold set by the ICO.

**For most SMBs**: A formal DPO is not legally required, but the ICO strongly recommends designating someone with responsibility for data protection compliance. This person should:
- Understand the UK GDPR requirements relevant to your business
- Have authority to make or escalate data protection decisions
- Be the point of contact for DSARs and breach procedures

**DPDIA 2024 note**: The Act introduces a "senior responsible individual" requirement, potentially replacing the DPO obligation for some organisations. Verify commencement status.

*Citation*: UK GDPR Arts.37–39; ICO, "Data protection officers" (ico.org.uk).

---

### Step 3: Map Your Processing Activities (ROPA)

**Requirement**: UK GDPR Article 30 requires written Records of Processing Activities (ROPA). Controllers with fewer than 250 employees must maintain ROPA if processing is not occasional, is likely to result in a risk to rights and freedoms, or involves special category or criminal offence data. **In practice, the ICO recommends all organisations maintain ROPA regardless of size.**

**Your ROPA must include** (Art.30(1)):
1. Name and contact details of the controller (and joint controller, representative, DPO where applicable)
2. Purposes of processing
3. Categories of data subjects and categories of personal data
4. Categories of recipients (including recipients in third countries)
5. Transfers to third countries (including the country and transfer mechanism)
6. Envisaged time limits for erasure of different data categories (where possible)
7. General description of technical and organisational security measures (where possible)

**Action**: Create a spreadsheet or use the ICO's ROPA template. For each processing activity, document:
- What personal data you collect
- Why you collect it (the purpose)
- Who you share it with
- How long you keep it
- How you protect it

**Review frequency**: At least annually, or whenever processing activities change.

*Citation*: UK GDPR Art.30; ICO, "Documentation" (ico.org.uk).

---

### Step 4: Identify Lawful Bases (UK GDPR Art.6)

For each processing activity in your ROPA, identify and document at least one lawful basis from Article 6(1):

**The six lawful bases**:

1. **Consent** (Art.6(1)(a)): Must be freely given, specific, informed, and unambiguous. Requires a clear affirmative act — silence, pre-ticked boxes, or inactivity do not count. You must be able to demonstrate consent was given. Withdrawal must be as easy as giving consent. **ICO warning**: Consent is unlikely to be appropriate for most employee data processing due to the power imbalance.

2. **Contract** (Art.6(1)(b)): Processing necessary for performing a contract with the data subject or taking pre-contractual steps at their request. Must be genuinely "necessary" — not merely useful. Cannot cover processing that merely serves your broader commercial interests.

3. **Legal obligation** (Art.6(1)(c)): Processing necessary to comply with a UK legal obligation (not merely a contractual obligation). Examples: PAYE obligations, anti-money laundering checks, Companies Act filings.

4. **Vital interests** (Art.6(1)(d)): Limited to life-or-death situations or serious threats to health.

5. **Public task** (Art.6(1)(e)): Primarily for public authorities. Private sector organisations may rely on this only if carrying out a specific public interest task set out in law.

6. **Legitimate interests** (Art.6(1)(f)): Most flexible basis but requires a Legitimate Interest Assessment (LIA) — see Step 10.

**Special category data** (Art.9): Processing data revealing racial/ethnic origin, political opinions, religious/philosophical beliefs, trade union membership, genetic data, biometric data for ID, health data, or sex life/sexual orientation requires BOTH an Art.9(2) condition AND a DPA 2018 Schedule 1 condition. Common conditions include explicit consent (Art.9(2)(a)), employment law (Art.9(2)(b)), and substantial public interest (Art.9(2)(g) + Schedule 1 Part 2).

**Criminal offence data** (Art.10; DPA 2018 s.10): May only be processed under official authority control or when authorised by UK law (DPA 2018 Schedule 1).

**Action**: For each row in your ROPA, record the lawful basis and your justification. If relying on consent, document how consent is obtained. If relying on legitimate interests, conduct a LIA (Step 10).

*Citation*: UK GDPR Arts.6, 9, 10; DPA 2018, s.10, Schedule 1; ICO, "Lawful basis for processing" (ico.org.uk).

---

### Step 5: Publish Privacy Notices (Arts.12–14)

**Requirement**: You must provide data subjects with information about your processing in a concise, transparent, intelligible, and easily accessible form.

**When data is collected from the data subject** (Art.13), your notice must include:
- Your identity and contact details (and DPO where applicable)
- The purposes and lawful basis for processing
- Legitimate interests relied upon (if applicable)
- Recipients or categories of recipients
- Details of any international transfers and the safeguards used
- Retention periods (or criteria for determining them)
- Data subject rights (access, rectification, erasure, restriction, portability, objection)
- Right to withdraw consent (if consent is the lawful basis)
- Right to complain to the ICO
- Whether provision of data is a statutory/contractual requirement
- Information about automated decision-making (if applicable)

**When data is not obtained directly from the data subject** (Art.14), additionally include: the categories of data and the source of the data.

**Action**: Draft or update privacy notices for your website, employment contracts, customer-facing communications, and any other data collection points.

**Review frequency**: At least annually, or when processing purposes change.

*Citation*: UK GDPR Arts.12–14; ICO, "Right to be informed" (ico.org.uk).

---

### Step 6: Implement Data Subject Rights Procedures

The UK GDPR grants data subjects the following rights. You need documented procedures for handling each:

| Right | Legal Basis | Response Time | Extension | Key Points |
|-------|------------|---------------|-----------|------------|
| Access (DSAR) | Art.15 | 1 calendar month | +2 months if complex/numerous | No fee unless manifestly unfounded/excessive. May request ID verification. DPA 2018 Sch.2 exemptions: legal privilege, self-incrimination, management forecasts, negotiations, exam scripts, confidential references |
| Rectification | Art.16 | Without undue delay (max 1 month) | +2 months if complex | Covers inaccurate and incomplete data |
| Erasure | Art.17 | Without undue delay (max 1 month) | +2 months if complex | Does not apply where processing is necessary for: freedom of expression, legal obligation, public health, archiving/research, or legal claims |
| Restriction | Art.18 | Without undue delay (max 1 month) | +2 months if complex | Applies when accuracy contested, processing unlawful, data needed for legal claims, or objection pending |
| Data portability | Art.20 | 1 calendar month | +2 months if complex | Only applies to data processed by consent or contract AND by automated means |
| Object | Art.21 | Without undue delay | N/A | Absolute right to object to direct marketing — no balancing test |
| Automated decisions | Art.22 | Proactive obligation | N/A | Right not to be subject to solely automated decisions with legal/significant effects |

**Action**: Create a DSAR response procedure including: how to receive requests (any channel — verbal, written, email), ID verification process, search and retrieval steps, review for exemptions, response template, and escalation path. Train staff who may receive requests.

**DPDIA 2024 note**: The Act replaces "manifestly unfounded or excessive" with "vexatious or excessive" for DSARs. Verify commencement status.

*Citation*: UK GDPR Arts.12–22; DPA 2018, Schedule 2; ICO, "Individual rights" (ico.org.uk).

---

### Step 7: Establish Data Breach Procedures

**What is a personal data breach?** (Art.4(12)): A breach of security leading to accidental or unlawful destruction, loss, alteration, unauthorised disclosure of, or access to personal data. This includes:
- Unauthorised third-party access
- Sending data to the wrong recipient
- Lost or stolen devices containing personal data
- Ransomware encrypting personal data (loss of availability)
- Deliberate or accidental action/inaction by controller or processor

### 7.1 Notification to the ICO (Art.33)

**Deadline**: Without undue delay and, where feasible, **not later than 72 hours** after becoming aware of the breach — unless the breach is unlikely to result in a risk to rights and freedoms.

**The notification must include**:
1. Nature of the breach (categories and approximate numbers of data subjects and records affected)
2. DPO or contact point name and details
3. Likely consequences of the breach
4. Measures taken or proposed to address the breach and mitigate effects

Information may be provided in phases if not all available at once.

**How to report**: Use the ICO's online breach reporting tool (ico.org.uk), which generates a reference number.

### 7.2 Notification to Data Subjects (Art.34)

**When required**: Where the breach is likely to result in a **high risk** to rights and freedoms.

**Must describe** (in clear, plain language):
- Nature of the breach
- DPO/contact point details
- Likely consequences
- Measures taken or proposed

**Not required where**:
- You've implemented measures rendering the data unintelligible (e.g., encryption)
- Subsequent measures ensure the high risk is no longer likely to materialise
- It would involve disproportionate effort (use public communication instead)

### 7.3 Breach Record-Keeping (Art.33(5))

**All breaches must be documented** regardless of whether reported to the ICO. Record: the facts, effects, and remedial action taken.

**Action**: Create a breach response plan including: internal reporting chain, assessment criteria (risk to individuals), 72-hour ICO notification procedure, data subject notification template, breach log template. Test the procedure at least annually.

*Citation*: UK GDPR Arts.4(12), 33, 34; ICO, "Personal data breaches" (ico.org.uk).

---

### Step 8: Conduct DPIAs for High-Risk Processing

**When mandatory** (Art.35(1)): Where processing is "likely to result in a high risk to the rights and freedoms of natural persons."

**Art.35(3) situations requiring a DPIA**:
1. Systematic and extensive automated evaluation of personal aspects (including profiling) on which decisions producing legal or similarly significant effects are based
2. Large-scale processing of special category data (Art.9) or criminal offence data (Art.10)
3. Systematic monitoring of a publicly accessible area on a large scale

**ICO's additional DPIA triggers**:
- Innovative technology combined with EDPB criteria
- Profiling to decide access to services
- Large-scale profiling
- Biometric data for identification
- Genetic data processing (beyond individual patient care)
- Matching data from multiple sources
- Processing without direct privacy notice + another criterion
- Location/behaviour tracking (including online via cookies)
- Targeting children for marketing, profiling, or automated decisions
- Data posing physical harm risk if misused

### DPIA Process (ICO Recommended)

1. **Screen**: Use the ICO's DPIA screening checklist to determine if a DPIA is required
2. **Describe the processing**: Nature, scope, context, purposes, data categories, lawful basis, retention, sharing
3. **Consult**: Seek views of data subjects where appropriate; consult DPO if appointed
4. **Assess necessity and proportionality**: Why is this processing necessary? Could less data or less intrusive processing achieve the purpose?
5. **Identify and assess risks**: Risks to individuals' rights and freedoms — assess likelihood and severity
6. **Identify mitigations**: Technical measures (encryption, pseudonymisation, access controls), organisational measures (policies, training), contractual measures (data processing agreements)
7. **Record outcome**: Document the DPIA and decision; sign off at appropriate level
8. **Prior consultation with ICO** (Art.36): If residual risks remain high despite mitigations, you must consult the ICO before proceeding. The ICO has 8 weeks to respond (extendable by 6 weeks for complex cases)
9. **Review and update**: When processing changes or new risks emerge

**Review frequency**: At least annually for high-risk processing, or when processing changes.

**DPDIA 2024 note**: DPIAs may be renamed "assessments of high risk processing." The core requirement remains.

*Citation*: UK GDPR Arts.35–36; ICO, "Data Protection Impact Assessments" (ico.org.uk).

---

### Step 9: Review International Data Transfers

**Framework**: UK GDPR Chapter V (Arts.44–49) governs transfers of personal data outside the UK.

**Transfer mechanisms hierarchy** (use the highest applicable mechanism):

1. **UK adequacy decision** (Art.45): If the destination country has a UK adequacy decision, no additional safeguards required. Countries include: EU/EEA member states, Japan, South Korea, Canada (commercial organisations), New Zealand, Switzerland, Israel, Argentina, Uruguay, Guernsey, Jersey, Isle of Man, and others.

   **Important**: The EU-UK adequacy decision was originally set to expire on 27 June 2025. Verify current status and any extension/renewal.

2. **UK IDTA or UK Addendum to EU SCCs**: For transfers to non-adequate countries:
   - **UK International Data Transfer Agreement (IDTA)**: Standalone UK mechanism, mandatory-form contract from the ICO (effective 21 March 2022). Covers C2C, C2P, P2C, P2P transfers.
   - **UK Addendum to EU SCCs**: Can be added to existing EU Standard Contractual Clauses to extend them for UK transfers.

3. **Binding Corporate Rules (BCRs)**: For intra-group transfers, approved by the ICO.

4. **Art.49 derogations**: Last resort — explicit consent, contractual necessity, important public interest, legal claims, vital interests, public register. Limited in scope; not suitable for routine transfers.

**Transfer Risk Assessment (TRA)**: Before relying on IDTA or UK Addendum, assess whether the destination country's laws provide adequate protection. Use the ICO's TRA tool.

**Action**: For each international transfer in your ROPA, identify the destination country, confirm whether a UK adequacy decision exists, and if not, implement the appropriate transfer mechanism. Conduct a TRA where required.

**Review frequency**: When transfer arrangements change; when adequacy decisions are renewed or revoked.

*Citation*: UK GDPR Arts.44–49; ICO, "International data transfer agreement and guidance" (ico.org.uk).

---

### Step 10: Conduct Legitimate Interest Assessments (LIAs)

**When required**: Every time you rely on legitimate interests (Art.6(1)(f)) as your lawful basis.

**ICO three-part test**:

**1. Purpose test** — Identify the legitimate interest:
- Is the interest lawful, specific, and real (not speculative)?
- Examples recognised by the ICO: fraud prevention, network/information security, direct marketing (subject to PECR), intra-group administration, reporting criminal acts
- The interest cannot be vague (e.g., "improving our business" is insufficient)

**2. Necessity test** — Is the processing necessary for that purpose?
- Could the purpose be achieved by other, less intrusive means?
- "Necessary" means more than helpful or desirable — the processing must be targeted and proportionate
- If the purpose could reasonably be achieved without the processing (or with less data), the test fails

**3. Balancing test** — Do the data subject's interests override yours?
Consider:
- Nature of the data (special category? financial? location?)
- Reasonable expectations (would data subjects expect this processing?)
- Potential impact (could it cause damage, distress, or harm?)
- Status of data subjects (children or vulnerable individuals?)
- Safeguards available (anonymisation, pseudonymisation, opt-out)
- Nature of the relationship between you and the data subject

The more intrusive the processing and the more significant the potential impact, the more compelling your legitimate interest must be.

**Action**: Use the ICO's downloadable LIA template. Document the three-part test and outcome. Retain as part of your accountability records (Art.5(2)).

**Review frequency**: At least annually, or when circumstances change.

**DPDIA 2024 note**: The Act introduces "recognised legitimate interests" (new Art.6(1)(ea)) allowing processing without a balancing test for specified purposes (national security, public security, emergencies, crime prevention, safeguarding). This is a significant change. Verify commencement status.

*Citation*: UK GDPR Art.6(1)(f), Recitals 47–49; ICO, "Legitimate interests" (ico.org.uk).

---

### Step 11: Review Direct Marketing Compliance (PECR)

The Privacy and Electronic Communications Regulations 2003 (PECR) (SI 2003/2426) impose additional rules on electronic marketing alongside the UK GDPR.

**Consent requirements by channel**:

| Channel | Consent Required? | Exception |
|---------|------------------|-----------|
| Email/SMS/MMS to individuals | Yes (prior consent) | Soft opt-in (Reg.22(3)) |
| Email/SMS to corporate subscribers | No PECR consent needed | UK GDPR still applies to personal data in the communication |
| Live telephone calls | Not if calling non-TPS numbers | Must not call TPS/CTPS-registered numbers without specific consent |
| Automated calls (recorded message) | Yes (prior consent) | No exceptions |
| Fax to individuals | Yes (prior consent) | — |
| Cookies/similar technologies | Yes (prior consent) | Strictly necessary cookies exempt |

**Soft opt-in** (Reg.22(3)) — consent not required where ALL of:
1. Contact details obtained in the course of a sale or negotiations for a sale
2. Marketing relates to your own similar products or services
3. Recipient given a clear and simple opt-out opportunity at collection AND in every subsequent communication
4. Recipient has not opted out

**Penalties**: The ICO can impose fines up to £500,000 for PECR breaches.

**Action**: Audit your marketing channels. For each, confirm you have the appropriate consent or exception. Maintain contemporaneous records of consent. Review at least annually.

**DPDIA 2024 note**: The Act extends the soft opt-in to charities/non-commercial organisations and may permit analytics cookies without consent. Verify commencement status.

*Citation*: PECR, Regs.6, 19, 20, 21, 22; DPA 2018 s.155; ICO, "Direct marketing" (ico.org.uk).

---

### Step 12: Assess Children's Code Compliance

**Scope**: The Age Appropriate Design Code (Children's Code) applies to "information society services" (online services) that are "likely to be accessed by children" (persons under 18). A service is in scope if a significant number of children use or are likely to use it, even if not specifically targeted at children.

**The 15 standards**:

1. **Best interests of the child** — Primary consideration in design
2. **DPIAs** — Assess and mitigate risks to children by age group
3. **Age-appropriate application** — Risk-based age recognition
4. **Transparency** — Child-friendly privacy information
5. **Detrimental use** — Do not use children's data in harmful ways
6. **Policies and community standards** — Uphold published terms
7. **Default settings** — High privacy by default
8. **Data minimisation** — Collect only what's needed
9. **Data sharing** — Do not disclose unless compelling reason
10. **Geolocation** — Off by default; visible indicator when active
11. **Parental controls** — Inform child when monitored
12. **Profiling** — Off by default; protect from harmful content
13. **Nudge techniques** — Do not nudge children to weaken privacy
14. **Connected toys/devices** — Include tools for Code conformance
15. **Online tools** — Prominent tools to exercise rights and report concerns

**Action**: If your online service is likely to be accessed by children, conduct a Children's Code conformance assessment. Focus on default settings (high privacy), data minimisation, and transparency.

**Review frequency**: When services change; at least annually.

*Citation*: DPA 2018 s.123; ICO, "Age appropriate design: a code of practice for online services" (ico.org.uk).

---

### Step 13: Implement Security Measures (Art.32)

**Requirement**: Implement appropriate technical and organisational measures to ensure a level of security appropriate to the risk.

**Art.32 measures** (as appropriate):
- Pseudonymisation and encryption of personal data
- Ability to ensure ongoing confidentiality, integrity, availability, and resilience
- Ability to restore availability and access to personal data in a timely manner following an incident
- Process for regularly testing, assessing, and evaluating effectiveness of measures

**Practical steps for SMBs**:
- Use strong passwords and multi-factor authentication
- Encrypt personal data at rest and in transit
- Maintain regular backups (tested for restoration)
- Keep software and systems up to date (patching)
- Restrict access to personal data on a need-to-know basis
- Train staff on data protection and security awareness
- Have an acceptable use policy for devices and systems
- Use secure disposal methods for data and hardware

*Citation*: UK GDPR Art.32; ICO, "Security outcomes" (ico.org.uk).

---

### Step 14: Review Data Processing Agreements (Art.28)

**Requirement**: Where you use a processor (any third party processing personal data on your behalf), you must have a written contract (data processing agreement) in place containing the mandatory provisions of Art.28(3).

**Mandatory provisions include**:
- Processing only on your documented instructions
- Confidentiality obligations on processor staff
- Appropriate security measures
- Conditions for engaging sub-processors (prior specific or general written authorisation)
- Assistance with data subject rights
- Assistance with breach notification
- Deletion or return of data on termination
- Audit rights

**Action**: Review all contracts with suppliers, SaaS providers, and other third parties who process personal data on your behalf. Ensure Art.28-compliant data processing agreements are in place.

**Review frequency**: When contracts are renewed or new processors are engaged.

*Citation*: UK GDPR Art.28; ICO, "Controllers and processors" (ico.org.uk).

---

### Step 15: Staff Training

**Requirement**: The ICO expects organisations to provide regular data protection training to all staff who handle personal data, proportionate to their role.

**Training should cover**:
- What personal data is and the data protection principles
- Your organisation's specific processing activities and policies
- How to recognise and respond to DSARs
- How to recognise and report a data breach
- Security practices (passwords, phishing, device security)
- Role-specific training for staff in data-intensive roles

**Frequency**: At least annually for all staff; enhanced training for new starters and staff changing roles.

*Citation*: ICO, "Accountability and governance" (ico.org.uk).

---

## 3. Data Protection and Digital Information Act 2024

The DPDIA 2024 received Royal Assent on 24 October 2024 and amends the UK GDPR/DPA 2018 framework. **Many provisions require commencement orders — verify which are in force.**

Key changes relevant to SMBs:

| Change | Effect | Status |
|--------|--------|--------|
| Recognised legitimate interests (new Art.6(1)(ea)) | Processing without balancing test for specified purposes (national security, crime prevention, safeguarding) | Verify commencement |
| ROPA reform | Focus on "high risk" processing — may reduce burden on smaller organisations | Verify commencement |
| DPIAs renamed | "Assessments of high risk processing" — core requirement unchanged | Verify commencement |
| DSAR threshold | "Vexatious or excessive" replaces "manifestly unfounded or excessive" | Verify commencement |
| Soft opt-in for charities | Extended to non-commercial organisations | Verify commencement |
| Analytics cookies | May be permitted without consent (subject to secondary legislation) | Verify commencement |
| Automated decisions | Restrictions apply only to "significant" decisions | Verify commencement |
| Senior responsible individual | May replace DPO requirement for some organisations | Verify commencement |
| ICO reformed | Becomes "Information Commission" with board governance | Verify commencement |

*Citation*: Data Protection and Digital Information Act 2024; ICO implementation plan and transition guidance (ico.org.uk).

---

## 4. Ongoing Compliance Schedule

| Activity | Frequency |
|----------|-----------|
| ICO registration renewal | Annually |
| ROPA review and update | At least annually, or when processing changes |
| Privacy notice review | At least annually, or when purposes change |
| DPIA review | At least annually for high-risk processing, or when processing changes |
| Data breach procedure testing | At least annually |
| Staff training | At least annually; enhanced for data-intensive roles |
| LIA review | At least annually, or when circumstances change |
| International transfer mechanism review | When arrangements change; when adequacy decisions are renewed/revoked |
| Processor agreement review | When contracts renewed or new processors engaged |
| Children's Code conformance assessment | When services change; at least annually |
| Security measures review | At least annually; more frequently for high-risk processing |
| PECR consent records review | At least annually |

---

## 5. Quick Reference: ICO Enforcement Powers

| Power | Maximum Penalty | Legal Basis |
|-------|----------------|-------------|
| UK GDPR fine (higher tier) | £17.5 million or 4% of annual worldwide turnover (whichever higher) | UK GDPR Art.83(5) |
| UK GDPR fine (lower tier) | £8.7 million or 2% of annual worldwide turnover (whichever higher) | UK GDPR Art.83(4) |
| PECR fine | £500,000 | DPA 2018 s.155 (as applied by PECR Reg.31) |
| ICO registration failure | £400 fixed penalty (£320 if paid in 28 days) + criminal offence | DPA 2018 s.108 |
| Information notice non-compliance | Criminal offence | DPA 2018 s.144 |
| Assessment notice (compulsory audit) | Issued by ICO; non-compliance is contempt | DPA 2018 ss.146–147 |
| Enforcement notice | Remedial action required; non-compliance is criminal offence | DPA 2018 s.149 |

---

## 6. Response Constraints

When using this workflow to assess compliance:

1. **Always specify the UK GDPR / DPA 2018** — never refer generically to "GDPR" without the UK prefix
2. **Reference the ICO** as the supervisory authority — not EU DPAs or the EDPB
3. **Use sterling (£)** for fine thresholds — not euros
4. **Cite specific articles and sections** — e.g., "UK GDPR Art.6(1)(f)" not "legitimate interests provision"
5. **Flag DPDIA 2024 changes** where relevant, with a note to verify commencement status
6. **Recommend professional advice** for: high-risk DPIAs requiring ICO prior consultation, complex international transfers, response to ICO enforcement action, and any processing of special category data at scale
7. **Use the ICO's terminology** — "data protection fee" not "registration fee"; "personal data breach" not "data breach"; "data subject access request" not "subject access request"
8. **Note the distinction between UK GDPR and PECR** — they are separate legal instruments with different penalty regimes
9. **Never suggest compliance is a one-off exercise** — emphasise the ongoing review cycle

### Output Format

Structure your compliance assessment as:

```
## UK GDPR / DPA 2018 Compliance Assessment

**Business**: [Name]
**Date**: [Date]
**Assessed by**: [AI-assisted — not a substitute for professional advice]

### Compliance Status by Area

| Area | Status | Priority | Notes |
|------|--------|----------|-------|
| ICO Registration | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| DPO/Data Protection Lead | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| ROPA | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| Lawful Bases | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| Privacy Notices | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| Data Subject Rights | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| Breach Procedures | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| DPIAs | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| International Transfers | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| PECR / Marketing | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| Children's Code | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| Security Measures | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| Processor Agreements | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |
| Staff Training | [✅/⚠️/❌] | [High/Medium/Low] | [Details] |

### Priority Actions
1. [Highest-priority gap]
2. [Second-priority gap]
3. [Third-priority gap]

### Recommended Next Steps
- [Specific, actionable recommendations]

### When to Instruct a Solicitor
- [List specific situations from this assessment that require professional advice]

⚠️ This assessment is AI-generated and does not constitute legal advice.
A qualified data protection practitioner should review your compliance
programme, particularly for high-risk processing activities.
```

---

## 7. Key Legislation Reference

| Legislation | Citation | Key Provisions |
|-------------|----------|----------------|
| UK GDPR | Retained EU Regulation 2016/679, as amended by SI 2019/419 | Data protection principles, lawful bases, rights, breach notification, transfers |
| Data Protection Act 2018 | DPA 2018 | Schedules 1–2 (special category conditions, exemptions), ICO powers, criminal offences |
| PECR | SI 2003/2426 | Electronic marketing, cookies, telephone preference service |
| Data Protection (Charges and Information) Regulations 2018 | SI 2018/480 | ICO registration fees |
| Data Protection and Digital Information Act 2024 | DPDIA 2024 | Reforms to UK GDPR framework (verify commencement) |
| UK International Data Transfer Agreement | ICO-approved, effective 21 March 2022 | Standard transfer mechanism for non-adequate countries |
| UK Addendum to EU SCCs | ICO-approved | Adapts EU SCCs for UK transfers |
