---
name: tax-law
description: UK tax law and HMRC compliance — corporation tax (25%/19%/marginal relief), income tax bands 2025/26, VAT (registration £90k, MTD), CGT (18%/24%), IHT (NRB £325k), R&D tax credits, PAYE/RTI, CIS, and SDLT rates.
user-invocable: true
argument-hint: "<topic> — topics: corporation-tax, income-tax, vat, cgt, iht, rd-credits, paye, cis, sdlt, investigations"
allowed-tools: [Read, Glob, Grep]
---

> **DISCLAIMER** This skill provides general information about UK tax law. It is not
> tax advice and must not be relied upon as such. Tax legislation and HMRC guidance
> change frequently. Always consult a qualified tax adviser or accountant before
> making decisions based on this information. Verify all rates, thresholds, and
> deadlines against current HMRC guidance at gov.uk.

---

# UK Tax Law and HMRC Compliance

---

## 1. Corporation Tax

**Primary legislation:** Corporation Tax Act 2009 (CTA 2009), Corporation Tax Act 2010
(CTA 2010), Finance Act 2021 s.6 (rate changes from April 2023).

### Rates from 1 April 2023

| Taxable Profits | Rate | Notes |
|---|---|---|
| ≤£50,000 | **19%** (small profits rate) | Lower limit |
| £50,001–£250,000 | **Marginal relief applies** | Effective rate between 19% and 25% |
| >£250,000 | **25%** (main rate) | Upper limit |

**Associated companies:** The £50,000 and £250,000 thresholds are divided by the
number of associated companies + 1 (CTA 2010 s.24). Example: a company with one
associated company has thresholds of £25,000 and £125,000.

### Marginal Relief Calculator Workflow

The marginal relief formula (Finance Act 2021):

```
Marginal Relief = Fraction × (Upper Limit − Profits) × (Taxable Profits / Profits)

Where:
  Fraction      = 3/200
  Upper Limit   = £250,000 (divided by associated companies + 1)
  Profits       = Taxable total profits + franked investment income
  Taxable Profits = Taxable total profits
```

**Step-by-step calculation:**

```
Step 1: Determine number of associated companies (N)
Step 2: Adjusted Upper Limit = £250,000 / (N + 1)
Step 3: Adjusted Lower Limit = £50,000 / (N + 1)
Step 4: If Profits ≤ Adjusted Lower Limit → tax at 19%
Step 5: If Profits > Adjusted Upper Limit → tax at 25%
Step 6: Otherwise, calculate:
        Tax = Profits × 25%
        Less Marginal Relief = 3/200 × (Adjusted Upper Limit − Profits)
                               × (Taxable Profits / Profits)
        CT Liability = Tax − Marginal Relief

EXAMPLE: Company with no associated companies, taxable profits £150,000
  Tax at 25%:         £150,000 × 25% = £37,500
  Marginal Relief:    3/200 × (£250,000 − £150,000) × (£150,000 / £150,000)
                      = 3/200 × £100,000 × 1 = £1,500
  CT Liability:       £37,500 − £1,500 = £36,000
  Effective rate:     24%
```

### Key Deadlines

- CT return (CT600): 12 months after end of accounting period
- Payment: 9 months and 1 day after end of accounting period
- Quarterly instalment payments: required where CT liability exceeds £10,000 and
  profits exceed £1.5m (divided by associated companies + 1)

---

## 2. Income Tax 2025/26 (England, Wales, and Northern Ireland)

**Primary legislation:** Income Tax Act 2007 (ITA 2007), Income Tax (Earnings and
Pensions) Act 2003 (ITEPA 2003).

### Tax Bands

| Band | Taxable Income | Rate |
|---|---|---|
| Personal Allowance | £0–£12,570 | **0%** |
| Basic rate | £12,571–£50,270 | **20%** |
| Higher rate | £50,271–£125,140 | **40%** |
| Additional rate | Over £125,140 | **45%** |

### Personal Allowance Taper

The Personal Allowance (PA) is reduced by £1 for every £2 of adjusted net income
above **£100,000** (ITA 2007 s.35). The PA is fully withdrawn at **£125,140**.

**Effective 60% tax band:** Between £100,000 and £125,140, the combined effect of
losing the PA (at £1 per £2) and paying 40% tax creates an effective marginal rate
of **60%**.

```
On £1 of income between £100,000 and £125,140:
  40% tax on the £1 of income                    = £0.40
  Loss of 50p PA → 40% tax on that 50p           = £0.20
  Total tax on £1                                 = £0.60
  Effective rate                                  = 60%
```

### National Insurance Contributions 2025/26

| Class | Who Pays | Rate |
|---|---|---|
| Class 1 (employee) | Employees | 8% on £12,570–£50,270; 2% above £50,270 |
| Class 1 (employer) | Employers | 15% above £5,000 (from April 2025) |
| Class 1A | Employers | 15% on benefits in kind |
| Class 2 | Self-employed | Abolished from April 2024 |
| Class 4 | Self-employed | 6% on £12,570–£50,270; 2% above £50,270 |

Employment Allowance: £10,500 off employer NIC liability (from April 2025).

### Scottish Income Tax 2025/26

Scotland sets its own income tax rates for non-savings, non-dividend income:

| Band | Taxable Income | Rate |
|---|---|---|
| Starter | £12,571–£14,876 | 19% |
| Basic | £14,877–£26,561 | 20% |
| Intermediate | £26,562–£43,662 | 21% |
| Higher | £43,663–£75,000 | 42% |
| Advanced | £75,001–£125,140 | 45% |
| Top | Over £125,140 | 48% |

### Dividend Tax 2025/26

- Dividend allowance: £500
- Basic rate: 8.75%
- Higher rate: 33.75%
- Additional rate: 39.35%

---

## 3. Value Added Tax (VAT)

**Primary legislation:** Value Added Tax Act 1994 (VATA 1994).

### Rates

| Rate | Percentage | Examples |
|---|---|---|
| Standard | **20%** | Most goods and services |
| Reduced | **5%** | Domestic fuel, child car seats, energy-saving materials |
| Zero | **0%** | Food (most), children's clothing, books, newspapers, public transport |
| Exempt | N/A | Financial services, insurance, education, health, land (option to tax available) |

### Registration and Deregistration

| Threshold | Amount | Effective Date |
|---|---|---|
| **Compulsory registration** | Taxable turnover exceeds **£90,000** in preceding 12 months | From 1 April 2024 |
| **Forward look** | Taxable turnover expected to exceed £90,000 in next 30 days alone | Immediate registration |
| **Voluntary registration** | Any level of taxable turnover | Available at any time |
| **Deregistration** | Taxable turnover falls below **£88,000** | Application to HMRC |

### Making Tax Digital (MTD) for VAT

Mandatory for **all** VAT-registered businesses (from April 2022):
- Keep digital records of all VAT transactions
- Submit VAT returns using MTD-compatible software
- Digital links required between software — no manual transposition
- Quarterly returns; Annual Accounting Scheme available for turnover ≤£1.35m

### VAT Schemes for SMBs

| Scheme | Eligibility | Benefit |
|---|---|---|
| Flat Rate Scheme | Turnover ≤£150,000 | Pay fixed % of gross turnover; simpler accounting |
| Cash Accounting | Turnover ≤£1.35m | Account for VAT on cash received/paid, not invoices |
| Annual Accounting | Turnover ≤£1.35m | One annual return instead of four; interim payments |

---

## 4. Capital Gains Tax (CGT)

**Primary legislation:** Taxation of Chargeable Gains Act 1992 (TCGA 1992).

### Rates from 30 October 2024

| Asset Type | Basic Rate Taxpayer | Higher/Additional Rate Taxpayer |
|---|---|---|
| Standard assets | **18%** | **24%** |
| Residential property (non-PPR) | **18%** | **24%** |

### Business Asset Disposal Relief (BADR) — formerly Entrepreneurs' Relief

TCGA 1992 s.169H–169S, as amended by Finance Act 2025.

| Period | BADR Rate | Lifetime Limit |
|---|---|---|
| To 5 April 2025 | **10%** | £1,000,000 |
| 6 April 2025 – 5 April 2026 | **14%** | £1,000,000 |
| From 6 April 2026 | **18%** | £1,000,000 |

**Qualifying conditions** (held for at least 2 years before disposal):
- Trading company or holding company of a trading group
- Individual holds ≥5% of ordinary shares and voting rights
- Individual is officer or employee of the company

### Annual Exempt Amount 2025/26

**£3,000** per individual (reduced from £6,000 in 2023/24 and £3,000 from 2024/25).

### Investors' Relief

Rate: 10% on qualifying shares in unlisted trading companies; lifetime limit £10m.

---

## 5. Inheritance Tax (IHT)

**Primary legislation:** Inheritance Tax Act 1984 (IHTA 1984).

### Nil-Rate Bands and Rates

| Element | Amount | Notes |
|---|---|---|
| **Nil-Rate Band (NRB)** | £325,000 | Frozen since 2009; frozen until at least April 2028 |
| **Residence Nil-Rate Band (RNRB)** | £175,000 | Available when residence passes to direct descendants |
| **Combined NRB + RNRB** | £500,000 | Per individual; £1m for married couple/civil partners |
| **IHT Rate** | **40%** | On estate above nil-rate bands |
| **Reduced Rate** | **36%** | If 10% or more of net estate left to charity |

### Transferable Nil-Rate Band

On second death, any unused NRB and RNRB from the first spouse/civil partner
can be transferred (IHTA 1984 s.8A). This effectively doubles the available
allowances for surviving spouses.

### Taper Relief on Lifetime Gifts (Potentially Exempt Transfers)

| Years Before Death | Tax Reduction |
|---|---|
| 0–3 years | 0% (full 40%) |
| 3–4 years | 20% reduction (effective 32%) |
| 4–5 years | 40% reduction (effective 24%) |
| 5–6 years | 60% reduction (effective 16%) |
| 6–7 years | 80% reduction (effective 8%) |
| 7+ years | Exempt |

### Business Property Relief (BPR) — IHTA 1984 ss.103–114

| Asset | Relief Rate | Notes |
|---|---|---|
| Unquoted shares / business interest | **100%** | Must be held 2 years; from April 2026, capped at first £1m at 100%, then 50% |
| Controlling holding in quoted company | **50%** | |
| Land/buildings/machinery used by partnership/company | **50%** | Controlled company or partnership of which transferor is a partner |

### Agricultural Property Relief (APR) — IHTA 1984 ss.115–124C

Similar structure to BPR. From April 2026, 100% relief capped at first £1m of
combined APR and BPR qualifying assets, with 50% relief on the excess.

---

## 6. R&D Tax Credits

**Primary legislation:** CTA 2009 Part 13 (merged scheme from April 2024).

### Merged R&D Scheme (Accounting Periods Beginning On or After 1 April 2024)

Replaced the former SME and RDEC schemes:

- **Above-the-line credit:** **20%** of qualifying R&D expenditure
- Taxable credit: effectively reduces net cost of R&D
- For profit-making companies: net benefit depends on CT rate
- For loss-making companies: payable credit available (subject to PAYE/NIC cap)

### Enhanced R&D Intensive Support (ERIS)

For loss-making companies where qualifying R&D expenditure is **30% or more** of
total expenditure:
- Enhanced deduction of 86% on qualifying expenditure (total deduction 186%)
- Payable credit at 14.5% of surrenderable loss
- Must be loss-making and R&D-intensive in the claim period

### Qualifying Expenditure

- Staff costs (gross pay, employer NIC, pension contributions)
- Externally provided workers (65% of payment)
- Consumables and materials
- Software directly used in R&D
- Relevant payments to clinical trial volunteers
- Cloud computing and data licence costs (from April 2023)

### Key Compliance Points

- Claims made via CT600 with additional information form submitted to HMRC
- Claim notification required for first-time or lapsed claimants (within 6 months of
  period end)
- Advance Assurance available for first 3 accounting periods
- Named senior officer must endorse the claim

---

## 7. PAYE and Real Time Information (RTI)

**Primary legislation:** ITEPA 2003, Income Tax (PAYE) Regulations 2003 (SI 2003/2682).

### RTI Obligations

| Submission | Deadline | Content |
|---|---|---|
| **Full Payment Submission (FPS)** | On or before each payday | Employee pay details, tax, NIC, student loan deductions |
| **Employer Payment Summary (EPS)** | By **19th** of the following tax month | Recoverable amounts (SMP, SPP, SAP, ShPP), CIS deductions suffered, Employment Allowance claim |
| **Earlier Year Update (EYU)** | Before 19 April following tax year | Corrections to previous year FPS/EPS (being phased out in favour of FPS corrections) |

### Key Dates

- Tax month: 6th to 5th of following month
- Payment to HMRC: **22nd** of following month (electronic) or **19th** (cheque)
- P60: issued to employees by **31 May** following end of tax year
- P11D (benefits in kind): filed by **6 July** following end of tax year
- Class 1A NIC on benefits: paid by **22 July** (electronic)

### Penalties for Late Filing

- 1 day late: £100 per 50 employees (monthly)
- 3 months late: additional £100 per 50 employees
- 6 months late: additional 5% of tax/NIC due
- 12 months late: additional 5% of tax/NIC due (or 100% if deliberate withholding)

---

## 8. Construction Industry Scheme (CIS)

**Primary legislation:** Finance Act 2004 ss.57–77, Income Tax (CIS) Regulations 2005 (SI 2005/2045).

### How CIS Works

1. **Contractor** verifies **subcontractor** with HMRC
2. Contractor makes deductions from payments to subcontractor
3. Contractor submits monthly CIS return to HMRC by **19th** of following month
4. Subcontractor offsets deductions against their own tax liability

### Deduction Rates

| Status | Rate | Requirement |
|---|---|---|
| **Gross payment** | **0%** | Registered, meets turnover test (£30,000/yr), compliance test, business test |
| **Net payment** | **20%** | Registered with HMRC |
| **Unregistered** | **30%** | Not registered or verification fails |

### Who Must Operate CIS

Any **contractor** (spending >£3m/yr on construction in 3 years, or a mainstream
contractor) who pays **subcontractors** for construction operations within the UK.

---

## 9. Stamp Duty Land Tax (SDLT)

**Primary legislation:** Finance Act 2003 Part 4.

### Residential Rates (England and Northern Ireland, from 1 April 2025)

| Portion of Purchase Price | Rate |
|---|---|
| Up to £125,000 | **0%** |
| £125,001–£250,000 | **2%** |
| £250,001–£925,000 | **5%** |
| £925,001–£1,500,000 | **10%** |
| Over £1,500,000 | **12%** |

**First-time buyers (purchases ≤£625,000):**
- 0% on the first £300,000
- 5% on £300,001–£500,000

**Higher rates for additional dwellings:** +5% surcharge on each band (from
31 October 2024, increased from +3%).

### Non-Residential and Mixed-Use Rates

| Portion of Purchase Price | Rate |
|---|---|
| Up to £150,000 | **0%** |
| £150,001–£250,000 | **2%** |
| Over £250,000 | **5%** |

### Filing and Payment

- File SDLT return and pay within **14 days** of completion
- Filed online via HMRC's SDLT service
- Penalties for late filing: £100 (immediate), £200 (3+ months), daily penalties (12+ months)

---

## 10. HMRC Investigations and Enquiries

**Primary legislation:** Taxes Management Act 1970 (TMA 1970).

### Types of Enquiry

| Type | Legislation | Scope | Time Limit |
|---|---|---|---|
| **Enquiry into return** | TMA 1970 s.9A (individuals) / Sch 18 para 24 FA 1998 (companies) | Full or aspect enquiry | **12 months** from filing date |
| **Discovery assessment** | TMA 1970 s.29 | HMRC discovers loss of tax | 4 years (ordinary), 6 years (careless), **20 years** (deliberate) |
| **COP 8** | Code of Practice 8 | Tax avoidance (no fraud suspected) | Negotiated settlement |
| **COP 9** | Code of Practice 9 | Suspected tax fraud — **Contractual Disclosure Facility (CDF)** | Opportunity to disclose fully; immunity from criminal prosecution if accepted |

### Discovery Assessment Time Limits (TMA 1970 s.36)

| Behaviour | Time Limit from End of Tax Year |
|---|---|
| Reasonable care | **4 years** |
| Careless | **6 years** |
| Deliberate | **20 years** |

### Penalties for Inaccuracies (Sch 24 FA 2007)

| Behaviour | Minimum Penalty | Maximum Penalty |
|---|---|---|
| Careless | 0% (unprompted disclosure) | 30% |
| Deliberate but not concealed | 20% (unprompted) | 70% |
| Deliberate and concealed | 30% (unprompted) | 100% |

Reductions apply for telling, helping, and giving access to records.

---

## Key Statutory References

- Corporation Tax Act 2009 / Corporation Tax Act 2010
- Income Tax Act 2007 / Income Tax (Earnings and Pensions) Act 2003
- Taxation of Chargeable Gains Act 1992
- Inheritance Tax Act 1984
- Value Added Tax Act 1994
- Finance Act 2003 (SDLT) / Finance Act 2004 (CIS)
- Taxes Management Act 1970
- Finance Act 2007 Sch 24 (Penalties)
- Finance Act 2021 s.6 (CT rates from April 2023)

---

*Last reviewed: March 2026. Tax rates, thresholds, and reliefs change regularly.
Always verify against current HMRC guidance at gov.uk and relevant Finance Acts.*
