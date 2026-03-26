# UK SMB Legal Plugin

A comprehensive UK legal assistant plugin primarily designed for [Cowork](https://claude.com/product/cowork), Anthropic's agentic desktop application — though it also works in Claude Code. Covers 15 practice areas and workflow skills across England & Wales with section-level statute citations, interactive calculators, and SRA-compliant disclaimers.

Built for **SMBs, founders, in-house teams, and legal professionals** operating in England & Wales.

> **Recommended model**: For best results, use the latest **Claude Opus** model. The plugin's skills involve complex legal reasoning across multiple statutes, nuanced case law application, and multi-step regulatory logic that benefit significantly from Opus-level reasoning. Sonnet will work for simpler queries but may produce less reliable outputs on edge cases like TUPE applicability, IR35 assessments, or Part 36 cost consequences.

> **Important**: This plugin provides legal information for England & Wales only. It does not constitute legal advice and is not a substitute for instruction of a qualified solicitor regulated by the Solicitors Regulation Authority (SRA). All outputs should be verified against current legislation on legislation.gov.uk. Rates and thresholds reflect the position as at April 2025.

**Built by [AI Heroes](https://www.ai-heroes.co)** — AI automation for UK businesses. Visit us for expert implementation, training, and bespoke AI solutions.

## Installation

```bash
claude plugins add UK-SMB-Legal-Plugin/legal-uk
```

## Commands

| Command | Description |
|---------|-------------|
| `/contract-review` | **NEW v1.1.0** — Playbook-based clause-by-clause contract review + full contract law reference (UCTA 1977, CRA 2015, MA 1967, LA 1980) |
| `/nda-triage` | **NEW v1.1.0** — GREEN/YELLOW/RED NDA screening with UK-specific clause analysis |
| `/legal-risk-assessment` | **NEW v1.1.0** — 5×5 severity × likelihood risk matrix with UK regulatory enforcement landscape |
| `/compliance-workflow` | **NEW v1.1.0** — UK GDPR/DPA 2018 compliance workflow with ICO-specific steps, DPIA, DSAR, breach notification |
| `/employment-law` | Unfair dismissal, redundancy, discrimination (EA 2010), working time, NLW/NMW rates, TUPE, flexible working, IR35, and Employment Tribunal procedure with ET time limit calculator |
| `/data-protection` | UK GDPR, DPA 2018, ICO enforcement, lawful basis selector, breach notification (72hr), DPIAs, international transfers (IDTA), PECR cookie consent, and Children's Code |
| `/company-law` | Directors' duties (ss.171–177 CA 2006), company formation, small/micro-entity regimes, ECCTA 2023, insolvency procedures, and Companies House filing obligations |
| `/intellectual-property` | Copyright (CDPA 1988), trade marks (TMA 1994), patents (PA 1977), designs, employee IP ownership, and post-Brexit UK/EU design divergence |
| `/property-law` | Freehold/leasehold (LPA 1925), land registration (LRA 2002), business tenancies (LTA 1954), Renters' Rights Act 2025, SDLT calculator with reliefs, and Land Registry forms |
| `/financial-services` | FSMA 2000, FCA Handbook, Consumer Duty PS22/9, financial promotion gateway, Payment Services Regulations 2017, SM&CR, and FSM Act 2023 crypto provisions |
| `/competition-law` | Competition Act 1998 (Ch I/II), Enterprise Act 2002 mergers, CMA enforcement, cartel offence, and DMCC Act 2024 (digital markets, consumer enforcement) |
| `/consumer-law` | Consumer Rights Act 2015 (goods, digital content, services), 14-day cooling-off (CCR 2013), unfair trading (CPRs 2008), and DMCC Act 2024 subscription traps |
| `/litigation-procedure` | CPR 1998, pre-action protocols, Part 36 offers, costs, fixed recoverable costs, disclosure (PD 57AD), court forms, MCOL, and full court fee table |
| `/tax-law` | Corporation tax (25%/19%/marginal relief calculator), income tax 2025/26, VAT (MTD), CGT, IHT, R&D credits, PAYE/RTI, CIS, SDLT, and HMRC investigations |
| `/regulatory-bodies` | ICO, FCA, PRA, CMA, SRA, BSB, HSE, TPR, FRC — enforcement powers, complaint routes, auto-enrolment calculator, retained EU law tracker, and IR35 status indicator |

## Skills

All 15 skills are user-invocable and provide deep, practice-area-specific guidance with full statute citations.

| Skill | Key Legislation | Interactive Features |
|-------|----------------|---------------------|
| `contract-review` | UCTA 1977, CRA 2015, MA 1967, LA 1980, LP(MP)A 1989 | Playbook-based review + contract law reference |
| `nda-triage` | Confidentiality, UCTA 1977, Competition Act 1998 | GREEN/YELLOW/RED clause screening |
| `legal-risk-assessment` | CA 2006, IA 1986, ECCTA 2023, various | 5×5 risk matrix, regulatory penalty reference |
| `compliance-workflow` | UK GDPR, DPA 2018, PECR 2003, DPDIA 2024 | 15-step compliance assessment workflow |
| `employment-law` | ERA 1996, EA 2010, WTR 1998, TUPE 2006, ITEPA 2003 | ET time limit calculator, TUPE checker, IR35 indicator |
| `data-protection` | UK GDPR, DPA 2018, PECR 2003 | Lawful basis selector, breach assessment workflow |
| `company-law` | CA 2006, ECCTA 2023, IA 1986 | Filing deadline tracker, size classification |
| `intellectual-property` | CDPA 1988, TMA 1994, PA 1977 | Duration calculator, employee IP assessment |
| `property-law` | LPA 1925, LRA 2002, LTA 1954, RRA 2025 | SDLT calculator with reliefs |
| `financial-services` | FSMA 2000, FCA Handbook, PSR 2017 | Authorisation checker, Consumer Duty assessment |
| `competition-law` | CA 1998, EA 2002, DMCC 2024 | Merger threshold checker |
| `consumer-law` | CRA 2015, CCR 2013, CPRs 2008 | Remedy hierarchy, cooling-off assessment |
| `litigation-procedure` | CPR 1998, PD 57AD | Court fee calculator, track allocation |
| `tax-law` | CTA 2009/10, ITA 2007, VATA 1994, TCGA 1992, IHTA 1984 | CT marginal relief calculator, SDLT calculator |
| `regulatory-bodies` | Various | Auto-enrolment calculator, retained EU law tracker |

## Example Workflows

### Employment Dispute Assessment

1. Run `/employment-law unfair-dismissal` to assess whether dismissal is potentially unfair
2. Run `/employment-law tribunal` to calculate the ET filing deadline (3 months minus one day)
3. Run `/employment-law discrimination` to check if any protected characteristics are engaged
4. Run `/litigation-procedure pre-action` to identify the applicable pre-action protocol

### Commercial Contract Review

1. Run `/contract-review` with the contract text to get a clause-by-clause playbook-based review
2. Run `/legal-risk-assessment` to assess overall risk profile of the contract
3. Run `/nda-triage` if the contract includes confidentiality provisions or is an NDA
4. Run `/intellectual-property licensing` to review any IP licensing provisions

### Property Transaction

1. Run `/property-law sdlt` to calculate Stamp Duty Land Tax liability with applicable reliefs
2. Run `/property-law registration` to identify Land Registry forms required (AP1, TR1, OS1)
3. Run `/property-law business-tenancy` to assess LTA 1954 Part II security of tenure
4. Run `/tax-law cgt` to calculate potential CGT exposure on disposal

### Company Formation & Compliance

1. Run `/company-law formation` to understand incorporation requirements
2. Run `/company-law directors-duties` to review ss.171–177 duties
3. Run `/tax-law corporation-tax` to calculate CT liability with marginal relief
4. Run `/regulatory-bodies auto-enrolment` to assess pension auto-enrolment duties

### Data Breach Response

1. Run `/compliance-workflow` to assess your overall data protection compliance posture
2. Run `/data-protection breach` to assess severity and ICO notification obligation (72hr)
3. Run `/data-protection rights` to understand data subject notification requirements
4. Run `/regulatory-bodies ico` to understand ICO enforcement powers and penalty framework

### HMRC Tax Planning

1. Run `/tax-law corporation-tax` to model CT liability with marginal relief calculator
2. Run `/tax-law vat` to check VAT registration threshold and scheme options
3. Run `/tax-law rd-credits` to assess R&D tax credit eligibility (merged scheme)
4. Run `/tax-law cgt` to plan disposals with Business Asset Disposal Relief

## UK-Specific Interactive Features

| Feature | Description |
|---------|-------------|
| **ET Time Limit Calculator** | Calculates exact ET1 filing deadline including ACAS early conciliation clock-stop |
| **SDLT Calculator** | Full SDLT computation with first-time buyer relief, additional dwelling surcharge (5%), and non-residential rates |
| **CT Marginal Relief Calculator** | Corporation tax with marginal relief for the £50k–£250k band (fraction 3/200) |
| **UK GDPR Lawful Basis Selector** | Guided workflow to select the appropriate lawful basis under Article 6(1) |
| **TUPE Applicability Checker** | Determines if TUPE 2006 applies and identifies employer obligations |
| **IR35 Status Indicator** | Guided assessment of off-payroll working status (ITEPA 2003 Chapter 10) |
| **Auto-Enrolment Calculator** | TPR pension duties, qualifying earnings, and minimum contributions |
| **Retained EU Law Tracker** | Status of assimilated law post-REUL Act 2023 |
| **Breach Assessment Workflow** | ICO notification assessment with 72-hour timeline |
| **Court Fee Calculator** | Full HMCTS court fee table for claims from £0 to £500k+ |

## MCP Integration

> If you see unfamiliar placeholders or need to check which tools are connected, see [CONNECTORS.md](CONNECTORS.md).

This plugin works best when connected to UK legal data sources via MCP servers. Add relevant servers to your `.mcp.json`:

### Companies House API
Connect to look up company details, director information, PSC register, filing history, and charges. Free API key from developer.company-information.service.gov.uk.

### HMRC MTD API
Connect to check VAT obligations, submit returns, and manage ITSA quarterly updates. OAuth 2.0 authentication via developer.service.hmrc.gov.uk.

### HM Land Registry
Connect for title searches, ownership records, and property data via Business Gateway.

### legislation.gov.uk
Connect to retrieve full text of UK Acts and Statutory Instruments.

### FCA Financial Services Register
Connect to check firm/individual authorisation and regulatory permissions.

### Practice Management
Connect Clio, LEAP, Smokeball, or PracticeEvolve for matter management and time recording.

> **Note:** The plugin works without any MCP connections — describe your scenario or paste documents directly. MCP connections enhance the experience by providing live data lookup.

## Key Rates & Thresholds (2025/26)

| Rate | Value |
|------|-------|
| Corporation Tax (main) | 25% (profits > £250k) |
| Corporation Tax (small profits) | 19% (profits ≤ £50k) |
| National Living Wage (21+) | £12.21/hr |
| VAT standard rate | 20% |
| VAT registration threshold | £90,000 |
| ET time limit | 3 months minus one day |
| ICO maximum fine | £17.5M or 4% worldwide turnover |
| CMA penalty cap | 10% worldwide turnover |
| SDLT additional dwelling surcharge | 5% (from Oct 2024) |
| IHT nil-rate band | £325,000 |
| CGT annual exempt amount | £3,000 |
| Auto-enrolment trigger | £10,000/yr earnings |

## Practice Areas Covered

| Area | Jurisdiction |
|------|-------------|
| **Contract Law** | England & Wales |
| **Employment Law** | England & Wales (some UK-wide elements) |
| **Data Protection & Privacy** | UK-wide (UK GDPR) |
| **Company Law** | England & Wales (Companies Act 2006 UK-wide) |
| **Intellectual Property** | UK-wide |
| **Property Law** | England & Wales |
| **Financial Services & FCA** | UK-wide |
| **Competition Law** | UK-wide |
| **Consumer Law** | England & Wales (some UK-wide) |
| **Litigation & Civil Procedure** | England & Wales |
| **Tax Law (HMRC)** | UK-wide (with E&W/Scotland differences noted) |
| **Regulatory Bodies** | UK-wide |

## Supported User Types

| Type | Typical Use Cases |
|------|------------------|
| **SMB owners & founders** | Contract review, employment disputes, company compliance, tax planning |
| **In-house legal teams** | Research, drafting, regulatory compliance, litigation support |
| **Sole practitioners** | Client matter research, document preparation, court procedure |
| **Accountants & tax advisers** | Tax law queries, Companies House compliance, HMRC procedures |
| **HR professionals** | Employment law, TUPE, discrimination, tribunal procedure |
| **Property professionals** | Conveyancing, business tenancies, SDLT, Land Registry |

## License

[Apache 2.0 + Commons Clause](LICENSE) — free for private and internal business use. Commercial resale is not permitted.
