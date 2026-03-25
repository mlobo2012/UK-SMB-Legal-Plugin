---
name: competition-law
description: UK competition law — Competition Act 1998 (Chapter I/II prohibitions), Enterprise Act 2002 merger control, CMA enforcement, cartel offence, and Digital Markets Competition and Consumers Act 2024.
user-invocable: true
argument-hint: "<topic> — topics: agreements, dominance, mergers, cartels, cma, dmcc, digital-markets"
allowed-tools: [Read, Glob, Grep]
---

# UK Competition Law

> **Disclaimer** — This skill provides legal information based on UK statutes, CMA guidance, and case law current as of March 2025. It is not legal advice. Competition law carries severe penalties including criminal sanctions for individuals. Users must consult a qualified competition solicitor before acting on any content. Legislation and CMA guidance may have been updated after the knowledge cut-off date.

## Arguments

The user invoked this skill with: `$ARGUMENTS`

Interpret the argument to identify the relevant topic (agreements, dominance, mergers, cartels, cma, dmcc, digital-markets) and focus your response on that area. If no argument is provided, give an overview of the UK competition law framework.

## Response Constraints

To ensure safe, accurate outputs:

1. **Cite only verified sources**: Only cite statutes, sections, and cases that appear in this skill document. Do not invent or generate case citations. If a relevant case is not in this skill, say: *"Case law generally supports this position — verify on BAILII or Westlaw UK."*
2. **Flag uncertainty explicitly**: If you are not certain about a threshold, rate, or procedural rule, say so. Use phrases like *"as at April 2025"* or *"verify the current figure on legislation.gov.uk."*
3. **Issue-spotting, not advice**: Frame all outputs as issue identification to help the user prepare for professional consultation — not as definitive legal advice.
4. **Scope boundaries**: If a query falls outside England & Wales, or involves devolved Scottish/Northern Irish law, say so clearly and refer the user to appropriate jurisdiction-specific resources.
5. **No fabricated citations**: If asked for a case or authority you cannot verify from this skill's content, explicitly say: *"I don't have a verified citation for that — please check BAILII (bailii.org) or instruct a solicitor."*

---

## 1. The UK Competition Regime — Overview

### Key Legislation

| Statute | Primary Role |
|---------|-------------|
| Competition Act 1998 (CA 1998) | Anti-competitive agreements (Chapter I); abuse of dominance (Chapter II) |
| Enterprise Act 2002 (EA 2002) | Merger control; market investigations; cartel criminal offence |
| Enterprise and Regulatory Reform Act 2013 (ERRA 2013) | Amended cartel offence; CMA creation |
| Digital Markets, Competition and Consumers Act 2024 (DMCC 2024) | Digital markets regime; enhanced CMA powers; consumer enforcement reform |

### Enforcement Authority

The **Competition and Markets Authority (CMA)** is the UK's primary competition enforcer (established by ERRA 2013 s.25, replacing the OFT and Competition Commission). Concurrent powers are held by sectoral regulators:
- Ofcom (telecommunications, broadcasting).
- Ofgem (energy).
- Ofwat (water).
- FCA (financial services).
- Monitor/NHS England (healthcare).
- ORR (railways).
- CAA (aviation).

---

## 2. Chapter I Prohibition — Anti-Competitive Agreements (s.2 CA 1998)

### The Prohibition

Section 2(1) prohibits agreements between undertakings, decisions by associations of undertakings, and concerted practices which:
- May affect trade within the United Kingdom; AND
- Have as their object or effect the prevention, restriction, or distortion of competition within the United Kingdom.

### Hard-Core Restrictions (s.2(2))

The following are specifically identified:
- **(a)** Price-fixing — directly or indirectly fixing purchase or selling prices.
- **(b)** Output limitation — limiting or controlling production, markets, technical development, or investment.
- **(c)** Market sharing — sharing markets or sources of supply.
- **(d)** Discriminatory conditions — applying dissimilar conditions to equivalent transactions.
- **(e)** Tying — making contracts subject to supplementary obligations unconnected with the subject.

### Object vs Effect

- **Object restrictions** (e.g., price-fixing, market sharing) are presumed anti-competitive; no need to prove actual market effects (Argos Ltd v OFT [2006] EWCA Civ 1318).
- **Effect restrictions** require analysis of actual or potential effects on competition in the relevant market.

### Exemptions

| Route | Basis | Key Requirements |
|-------|-------|-----------------|
| Individual exemption (s.9 CA 1998) | Self-assessment by parties (no prior notification) | Four conditions: efficiency gains; fair share to consumers; indispensable restrictions; no elimination of competition |
| Block exemptions (s.6 CA 1998) | UK block exemption orders, retained EU block exemptions | E.g., vertical agreements (VABEO 2022 SI 2022/516), technology transfer, R&D, specialisation |
| Small agreements (s.39 CA 1998) | Combined turnover of parties ≤£20m | Immunity from financial penalties only (not from unenforceability or injunctions); does not apply to price-fixing |

### Vertical Agreements Block Exemption Order 2022 (SI 2022/516)

- Replaced the retained EU Vertical Agreements Block Exemption on 1 June 2022.
- Exempts vertical agreements where supplier's market share ≤30% and buyer's market share ≤30%.
- Hard-core restrictions exclude the benefit: RPM (resale price maintenance), territorial/customer restrictions (subject to exceptions), selective distribution restrictions.
- CMA can withdraw the exemption in individual cases.

### Penalties for Breach

- **Financial penalties**: up to **10% of worldwide turnover** in each year of infringement, capped at the duration of infringement (s.36 CA 1998; CMA Guidance CMA73).
- **Unenforceability**: agreements caught by Chapter I are void (s.2(4) CA 1998).
- **Director disqualification**: Competition Disqualification Order (CDO) for up to 15 years (s.9A EA 2002).
- **Private damages**: right of action for any person who has suffered loss (s.47A CA 1998; opt-out collective proceedings s.47B).

---

## 3. Chapter II Prohibition — Abuse of Dominant Position (s.18 CA 1998)

### The Prohibition

Section 18(1) prohibits conduct by one or more undertakings which amounts to an abuse of a dominant position in a market, if it may affect trade within the United Kingdom.

### Dominance

- Market share is the starting point; shares above **40%** raise a presumption of dominance; shares above **50%** create a strong presumption (AKZO Chemie BV v Commission [1991] ECR I-3359, applied in UK).
- Other factors: barriers to entry, countervailing buyer power, vertical integration, access to financial resources.
- Relevant market: product market (demand-side and supply-side substitutability) and geographic market.

### Types of Abuse (s.18(2))

| Abuse | Description | Example |
|-------|-------------|---------|
| **(a)** Unfair prices or trading conditions | Imposing unfair purchase/selling prices or trading conditions | Excessive pricing (Pfizer/Flynn [2020] EWCA Civ 339) |
| **(b)** Limiting production/markets/technical development | Restricting output to prejudice of consumers | Withholding supply to foreclose competitors |
| **(c)** Discriminatory conditions | Dissimilar conditions for equivalent transactions | Selective rebates to favoured customers |
| **(d)** Tying | Making contracts subject to unrelated supplementary obligations | Bundling unrelated products |

Additional categories recognised in case law:
- **Predatory pricing**: pricing below cost to eliminate competitors (s.18(2)(a)).
- **Margin squeeze**: dominant vertically-integrated firm sets wholesale and retail prices so downstream competitors cannot compete profitably.
- **Refusal to supply**: especially where the input is an essential facility.
- **Exclusive dealing**: long-term exclusive contracts foreclosing the market.

### Penalties

Same as Chapter I: up to 10% of worldwide turnover per year of infringement.

---

## 4. Merger Control (Enterprise Act 2002 Part 3)

### Jurisdictional Thresholds

The CMA may investigate a merger (a "relevant merger situation" — s.23 EA 2002) if:

| Test | Threshold | Section |
|------|-----------|---------|
| **Turnover test** | UK turnover of target ≥**£70 million** | s.23(1)(b) |
| **Share of supply test** | Merged entity supplies or acquires **≥25%** of goods/services of any description in the UK (or a substantial part), and the merger results in an increment to that share | s.23(2)-(4) |

Only one test need be met. The CMA may also have jurisdiction over anticipated mergers (s.33).

### Notification

- UK merger control is **voluntary** — no mandatory pre-notification.
- However, the CMA can and does call in completed mergers for investigation.
- Informal guidance: CMA may provide confidential informal advice pre-notification.
- Formal notification: Merger Notice form, filing fee applies.

### Phase 1 Investigation

- Duration: **40 working days** from confirmation of a complete notification (extendable).
- Test: does the merger create a "realistic prospect" of a substantial lessening of competition (SLC)? (s.33(1) for anticipated; s.22(1) for completed).
- Outcomes:
  - **Clearance**: no SLC concerns.
  - **Undertakings in lieu (UIL)**: CMA accepts remedies offered by the parties to resolve concerns without Phase 2 (s.73).
  - **Reference to Phase 2**: if realistic prospect of SLC and UIL not appropriate.

### Phase 2 Investigation

- Conducted by an independent inquiry group of CMA panel members.
- Duration: **24 weeks** (extendable by 8 weeks) (s.39(1)).
- Test: would the merger result, or be expected to result, in an SLC (on the "balance of probabilities" — higher standard than Phase 1).
- Remedies: structural (divestiture) or behavioural; CMA has wide discretion.
- Blocking/unwinding: CMA can prohibit anticipated mergers or require divestiture of completed mergers.

### Filing Fees (SI 2003/1592, as amended)

| UK Turnover of Target | Fee |
|----------------------|-----|
| Up to £20m | £0 (no fee) |
| £20m - £70m | £40,000 |
| £70m - £120m | £80,000 |
| Over £120m | £160,000 |

---

## 5. The Cartel Offence (s.188 Enterprise Act 2002)

### The Offence

An individual commits an offence if they agree with one or more other persons to make or implement, or cause to be made or implemented, arrangements involving:
- **Price-fixing** (s.188(2)(a)).
- **Limitation of supply or production** (s.188(2)(b)).
- **Market sharing** (s.188(2)(c)).
- **Bid-rigging** (s.188(2)(d)).

### Key Features

| Feature | Detail |
|---------|--------|
| **Who can be guilty** | Individuals only (not companies); but usually prosecuted alongside company civil enforcement |
| **Mens rea** | Originally required proof of "dishonesty"; dishonesty requirement **removed by ERRA 2013 s.47** from 1 April 2014 |
| **Defences** | (1) Arrangements notified to CMA before making (s.188A(1)); (2) Arrangements published in London Gazette/prescribed manner (s.188A(2)); (3) Arrangements made to comply with legal requirement (s.188A(3)) |
| **Maximum penalty** | **5 years' imprisonment** and/or unlimited fine (s.190(1)) |
| **Statute of limitations** | None for indictable offences; summary prosecution within 6 months |
| **Prosecuting authority** | CMA (s.190(2)) or SFO (s.190(4)) |

### Leniency Policy (CMA Guidance OFT1495)

| Type | Benefit | Conditions |
|------|---------|------------|
| Type A immunity (civil) | Total immunity from financial penalties for undertaking | First to report; no coercion of others to participate; continuous cooperation |
| Type B leniency (civil) | Reduction of up to 100% of penalties | First or subsequent to report; provides added value; did not coerce others |
| Type C leniency (civil) | Reduction of up to 50% | Subsequent reporters providing added value |
| Criminal immunity (no-action letters) | Immunity from criminal prosecution for individuals | Cooperating individual; provides evidence; usually as part of corporate leniency application |

Leniency applications are made orally to the CMA Cartels and Criminal Group; a "marker" can be placed while evidence is gathered.

---

## 6. Digital Markets, Competition and Consumers Act 2024 (DMCC 2024)

### Part 1 — Digital Markets (from 1 January 2025)

#### Strategic Market Status (SMS) Designation

- The CMA's Digital Markets Unit (DMU) can designate undertakings (or groups) with **Strategic Market Status** in relation to a specific digital activity if (s.2 DMCC):
  - The undertaking has **substantial and entrenched market power** in the relevant digital activity.
  - The undertaking holds a **position of strategic significance** (gateway or gatekeeper role).
- Thresholds: global turnover >**£25 billion** or UK turnover >**£1 billion** (s.3).
- Designation lasts **5 years** (s.15); can be reviewed/varied/revoked.

#### Conduct Requirements (ss.19-29)

The CMA can impose conduct requirements on SMS firms, including:
- **Fair dealing** (s.20): trade on fair and reasonable terms.
- **Open choices** (s.21): allow users to switch/multi-home freely.
- **Trust and transparency** (s.22): provide clear information about terms and algorithmic decision-making.

#### Pro-Competition Interventions (ss.46-58)

- CMA can impose PCIs to address adverse effects on competition (s.46).
- May include interoperability requirements, data access mandates, separation of activities.
- SMS firms must comply within timeframes specified.

#### Penalties for Breach

- Financial penalty: up to **10% of global turnover** (s.85(3)).
- Daily penalty for continuing breach: up to **5% of daily worldwide turnover** (s.85(4)).

### Part 2 — Competition (from 1 January 2025)

- Enhanced CMA merger investigation powers: ability to accept binding commitments during investigations (s.108).
- CMA can require information during market studies (not just market investigations) (s.140A-140B EA 2002 as amended).
- Review of CMA decisions: move from full merits review to **judicial review standard** for penalty appeals at the Competition Appeal Tribunal (s.103).

### Part 3 — Consumer Protection (from 6 April 2025)

- CMA gains **direct enforcement powers** for consumer law (no longer needs to apply to court for enforcement orders in most cases) (s.149+).
- CMA can impose financial penalties of up to **10% of global turnover** for consumer law breaches (s.167).
- Turnover penalty: calculated on turnover in the relevant period; minimum penalty provisions.
- Enhanced investigation powers: CMA can require information, enter premises, interview individuals.

### Part 4 — Consumer Protection (Unfair Commercial Practices) (from 6 April 2025)

Key new prohibitions and amendments to the CPRs 2008:
- **Fake reviews**: new specific prohibition on commissioning, publishing, or facilitating fake reviews; offering or advertising to submit fake reviews (Sch.19 para 31A-31C).
- **Drip pricing**: hidden fees and charges that are not included in the headline price and are revealed later in the purchasing process are banned (Sch.19 para 6A).
- **Subscription traps**: enhanced requirements on subscription contracts (see Consumer Law skill for detail).
- Penalties: CMA can impose up to 10% of global turnover.

---

## 7. Market Investigations (EA 2002 Part 4)

### Process

| Stage | Duration | Outcome |
|-------|----------|---------|
| Market study (s.130A) | Up to 12 months | CMA may publish report; make recommendations; accept undertakings; or make a market investigation reference |
| Market investigation (s.131) | Up to 18 months (extendable by 6 months) | CMA determines whether features of the market prevent, restrict, or distort competition (Adverse Effect on Competition — AEC) |

### Remedies

If AEC is found, the CMA may:
- Accept undertakings from market participants (s.154).
- Make an order (s.161) — may include price controls, divestiture requirements, behavioural obligations.
- Recommend government action (e.g., legislative change).

---

## 8. Private Enforcement

### Competition Appeal Tribunal (CAT)

- Specialist tribunal for competition disputes.
- Jurisdiction:
  - Appeals from CMA infringement decisions and penalty calculations (s.46 CA 1998).
  - Follow-on damages claims based on CMA infringement decision (s.47A CA 1998).
  - Stand-alone damages claims (s.47A, as amended by Consumer Rights Act 2015 Sch.8).
  - Collective proceedings (opt-in or opt-out) (s.47B CA 1998).

### Damages Claims

| Type | Basis | Limitation |
|------|-------|-----------|
| Follow-on | CMA/European Commission infringement decision is binding | 2 years from infringement decision becoming final |
| Stand-alone | Claimant proves infringement | 6 years from cause of action (Limitation Act 1980 s.2) |
| Collective proceedings | Representative brings claim on behalf of a class | As above; CAT must certify the class |

### Landmark UK Cases

| Case | Year | Significance |
|------|------|-------------|
| Merricks v Mastercard | 2020-2023 | First opt-out collective proceedings certified; interchange fees |
| Argos/Littlewoods (Hasbro) | 2003-2006 | Toy price-fixing; Chapter I infringement; director disqualification |
| Pfizer/Flynn (Phenytoin) | 2020 | Court of Appeal framework for excessive pricing abuse |
| BritNed v ABB | 2018 | Follow-on damages for cable cartel; £85m damages |

---

## 9. Compliance Essentials for SMBs

### Red Flags — When to Seek Competition Advice

1. Any direct or indirect contact with competitors about prices, costs, margins, or commercial strategy.
2. Agreements with competitors to divide customers, territories, or tenders.
3. Receiving or sharing competitively sensitive information at trade association meetings.
4. Proposed joint ventures or cooperation agreements with competitors.
5. Acquiring a business where combined market share may exceed 25% or target UK turnover may exceed £70m.
6. If your company holds a market share above 40% and you intend to change pricing, exclusive dealing, or tying practices.

### Practical Steps

- Implement a written competition law compliance policy.
- Train staff (especially sales and procurement teams) on identifying cartel behaviour.
- Establish a protocol for trade association meetings — no discussion of prices, output, customers.
- Record all meetings with competitors; ensure legal review of any cooperation agreements.
- If you discover a potential infringement: seek legal advice immediately; consider leniency.

---

## Key Statutory References

- Competition Act 1998 (c.41)
- Enterprise Act 2002 (c.40)
- Enterprise and Regulatory Reform Act 2013 (c.24)
- Digital Markets, Competition and Consumers Act 2024 (c.XX)
- Competition Act 1998 (Small Agreements and Conduct of Limited Immunity) Regulations 2000 (SI 2000/262)
- The Competition Act 1998 (Vertical Agreements Block Exemption) Order 2022 (SI 2022/516)
- CMA Guidance: Penalties (CMA73); Mergers (CMA2 revised); Market investigations (CMA3)
- CMA Guidance: Leniency and no-action (OFT1495)
