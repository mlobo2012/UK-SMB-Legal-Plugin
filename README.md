# UK SMB Legal Plugin for Claude Code

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code Compatible](https://img.shields.io/badge/Claude%20Code-Compatible-blueviolet)](https://claude.ai)

A comprehensive AI-powered UK legal assistant for small and medium-sized businesses, built as a plugin for [Claude Code](https://claude.ai). Covers 12 practice areas across England & Wales with section-level statute citations, interactive calculators, and SRA-compliant disclaimers. Also includes a [Cowork](https://claude.com/product/cowork) variant for Anthropic's agentic desktop application.

> **Disclaimer:** This plugin provides legal information for England & Wales only. It does not constitute legal advice and is not a substitute for instruction of a qualified solicitor regulated by the Solicitors Regulation Authority (SRA). All outputs should be verified against current legislation on [legislation.gov.uk](https://www.legislation.gov.uk/). Rates and thresholds reflect the position as at April 2025.

---

## Built by AI Heroes

This plugin was created by **[AI Heroes](https://www.ai-heroes.co)** — AI automation for UK businesses. Visit us for expert implementation, training, and bespoke AI solutions.

---

## 12 Practice Areas

| # | Practice Area | Jurisdiction | Key Legislation |
|---|---------------|-------------|-----------------|
| 1 | Contract Law | England & Wales | UCTA 1977, CRA 2015, MA 1967, LA 1980 |
| 2 | Employment Law | England & Wales (some UK-wide) | ERA 1996, EA 2010, WTR 1998, TUPE 2006 |
| 3 | Data Protection | UK-wide | UK GDPR, DPA 2018, PECR 2003 |
| 4 | Company Law | England & Wales (CA 2006 UK-wide) | CA 2006, ECCTA 2023, IA 1986 |
| 5 | Intellectual Property | UK-wide | CDPA 1988, TMA 1994, PA 1977 |
| 6 | Property Law | England & Wales | LPA 1925, LRA 2002, LTA 1954, RRA 2025 |
| 7 | Financial Services | UK-wide | FSMA 2000, FCA Handbook, PSR 2017 |
| 8 | Competition Law | UK-wide | CA 1998, EA 2002, DMCC 2024 |
| 9 | Consumer Law | England & Wales (some UK-wide) | CRA 2015, CCR 2013, CPRs 2008 |
| 10 | Litigation & Civil Procedure | England & Wales | CPR 1998, PD 57AD |
| 11 | Tax Law | UK-wide | CTA 2009/10, ITA 2007, VATA 1994, TCGA 1992 |
| 12 | Regulatory Bodies | UK-wide | Various (ICO, FCA, CMA, SRA, HSE, TPR) |

## 10+ Interactive Calculators & Checkers

| # | Calculator / Checker | Skill |
|---|---------------------|-------|
| 1 | ET Time Limit Calculator (including ACAS clock-stop) | Employment Law |
| 2 | SDLT Calculator (first-time buyer relief, additional dwelling surcharge) | Property Law |
| 3 | CT Marginal Relief Calculator (£50k–£250k band) | Tax Law |
| 4 | UK GDPR Lawful Basis Selector (Article 6(1) guidance) | Data Protection |
| 5 | TUPE Applicability Checker | Employment Law |
| 6 | IR35 Status Indicator (off-payroll working assessment) | Employment Law |
| 7 | Auto-Enrolment Calculator (TPR pension duties) | Regulatory Bodies |
| 8 | Retained EU Law Tracker (post-REUL Act 2023) | Regulatory Bodies |
| 9 | ICO Breach Assessment Workflow (72-hour timeline) | Data Protection |
| 10 | Court Fee Calculator (HMCTS fees £0–£500k+) | Litigation Procedure |

## Commands

| Command | Description |
|---------|-------------|
| `/contract-law` | Contract formation, terms, breach, remedies, limitation periods, unfair terms (UCTA 1977, CRA 2015), misrepresentation (MA 1967) |
| `/employment-law` | Unfair dismissal, redundancy, discrimination (EA 2010), TUPE, IR35, ET procedure with time limit calculator |
| `/data-protection` | UK GDPR, DPA 2018, ICO enforcement, lawful basis selector, breach notification, DPIAs, international transfers |
| `/company-law` | Directors' duties (ss.171–177 CA 2006), formation, ECCTA 2023, insolvency, Companies House filings |
| `/intellectual-property` | Copyright (CDPA 1988), trade marks (TMA 1994), patents (PA 1977), designs, employee IP ownership |
| `/property-law` | Freehold/leasehold, land registration, business tenancies (LTA 1954), SDLT calculator with reliefs |
| `/financial-services` | FSMA 2000, FCA Handbook, Consumer Duty, financial promotions, SM&CR, crypto provisions |
| `/competition-law` | Competition Act 1998, Enterprise Act 2002 mergers, CMA enforcement, DMCC Act 2024 |
| `/consumer-law` | Consumer Rights Act 2015, 14-day cooling-off, unfair trading, DMCC Act 2024 subscription traps |
| `/litigation-procedure` | CPR 1998, pre-action protocols, Part 36 offers, costs, court forms, MCOL, court fee table |
| `/tax-law` | Corporation tax, income tax, VAT (MTD), CGT, IHT, R&D credits, PAYE/RTI, CIS, SDLT |
| `/regulatory-bodies` | ICO, FCA, PRA, CMA, SRA, BSB, HSE, TPR, FRC — enforcement powers, complaint routes |

## Installation

### Option 1: Claude Code Plugin (recommended)

```bash
claude plugins add UK-SMB-Legal-Plugin/legal-uk
```

### Option 2: Drag and Drop

Download this repository and drag the `legal-uk` folder into your Claude Code workspace.

### Option 3: Git Clone

```bash
git clone https://github.com/mlobo2012/UK-SMB-Legal-Plugin.git
cd UK-SMB-Legal-Plugin
claude plugins add legal-uk
```

### Cowork Variant

For use with Anthropic's [Cowork](https://claude.com/product/cowork) desktop application, install the `legal-uk-cowork` variant instead:

```bash
claude plugins add UK-SMB-Legal-Plugin/legal-uk-cowork
```

## File Structure

```
UK-SMB-Legal-Plugin/
├── README.md
├── legal-uk/                          # Claude Code variant
│   ├── .claude-plugin/plugin.json
│   ├── .mcp.json
│   ├── CONNECTORS.md
│   ├── LICENSE
│   ├── README.md
│   └── skills/
│       ├── contract-law/SKILL.md
│       ├── employment-law/SKILL.md
│       ├── data-protection/SKILL.md
│       ├── company-law/SKILL.md
│       ├── intellectual-property/SKILL.md
│       ├── property-law/SKILL.md
│       ├── financial-services/SKILL.md
│       ├── competition-law/SKILL.md
│       ├── consumer-law/SKILL.md
│       ├── litigation-procedure/SKILL.md
│       ├── tax-law/SKILL.md
│       └── regulatory-bodies/SKILL.md
└── legal-uk-cowork/                   # Cowork variant
    ├── .claude-plugin/plugin.json
    ├── .mcp.json
    ├── CONNECTORS.md
    ├── LICENSE
    ├── README.md
    └── skills/
        └── (same 12 practice areas)
```

## MCP Integration

The plugin connects to UK legal data sources through MCP (Model Context Protocol) servers:

| Category | Examples | Purpose |
|----------|----------|---------|
| Companies House | Companies House API | Company details, directors, PSC register, filing history |
| HMRC | MTD API | VAT obligations, returns, ITSA quarterly updates |
| Land Registry | HM Land Registry | Title searches, ownership records, property data |
| Legislation | legislation.gov.uk | Full text of UK Acts and Statutory Instruments |
| FCA | Financial Services Register | Firm/individual authorisation, regulatory permissions |
| Practice Management | Clio, LEAP, Smokeball | Matter management, time recording |

> **Note:** The plugin works without any MCP connections — describe your scenario or paste documents directly. MCP connections enhance the experience by providing live data lookup. See [CONNECTORS.md](legal-uk/CONNECTORS.md) for the full list of supported integrations.

## Legal Accuracy

- All statutory references cite the official Act by name and section (s., ss.)
- All monetary thresholds and tax rates reflect the position as at **April 2025**
- English legal terminology is used throughout, with statutory references to legislation.gov.uk
- Every skill includes a mandatory **SRA-compliant disclaimer**
- Jurisdictional scope (England & Wales vs UK-wide) is clearly stated per practice area

## Contributing

Contributions are welcome. Please ensure all legal content is accurate and up-to-date with current English law and UK-wide legislation where applicable.

## License

This project is licensed under the MIT License — see the [LICENSE](legal-uk/LICENSE) file for details.

---

**Built by [AI Heroes](https://www.ai-heroes.co)** | MIT License | Claude Code Compatible
