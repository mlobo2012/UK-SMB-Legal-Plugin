---
name: contract-law
description: UK contract law guidance for England & Wales — formation, terms, remedies, limitation periods, unfair terms (UCTA 1977, CRA 2015 Part 2), and force majeure. Cites statutes by section with legislation.gov.uk references.
user-invocable: true
argument-hint: "<topic> — topics: formation, terms, breach, remedies, limitation, unfair-terms, force-majeure, misrepresentation"
allowed-tools: [Read, Glob, Grep]
---

# Contract Law — /contract-law

> **DISCLAIMER:** This skill provides legal information for England & Wales only. It does not constitute legal advice and is not a substitute for instruction of a qualified solicitor regulated by the SRA. Verify all citations on [legislation.gov.uk](https://www.legislation.gov.uk). Law stated as at April 2025.

## Arguments

The user invoked this with: **$ARGUMENTS**

Parse the arguments to route to the relevant topic below. If no argument is supplied, provide a summary of all topics with cross-references. Accepted topics:

| Keyword | Section |
|---|---|
| `formation` | 1 — Contract Formation |
| `formal-requirements` | 2 — Formal Requirements |
| `terms` | 3 — Terms & Classification |
| `unfair-terms` | 4 — Unfair Terms (UCTA 1977 / CRA 2015) |
| `misrepresentation` | 5 — Misrepresentation |
| `breach` or `remedies` | 6 — Breach & Remedies |
| `limitation` | 7 — Limitation Periods |
| `force-majeure` | 8 — Force Majeure & Frustration |
| `third-party` | 9 — Third Party Rights |
| `nom` or `oral-modification` | 10 — No Oral Modification Clauses |

## Response Constraints

To ensure safe, accurate outputs:

1. **Cite only verified sources**: Only cite statutes, sections, and cases that appear in this skill document. Do not invent or generate case citations. If a relevant case is not in this skill, say: *"Case law generally supports this position — verify on BAILII or Westlaw UK."*
2. **Flag uncertainty explicitly**: If you are not certain about a threshold, rate, or procedural rule, say so. Use phrases like *"as at April 2025"* or *"verify the current figure on legislation.gov.uk."*
3. **Issue-spotting, not advice**: Frame all outputs as issue identification to help the user prepare for professional consultation — not as definitive legal advice.
4. **Scope boundaries**: If a query falls outside England & Wales, or involves devolved Scottish/Northern Irish law, say so clearly and refer the user to appropriate jurisdiction-specific resources.
5. **No fabricated citations**: If asked for a case or authority you cannot verify from this skill's content, explicitly say: *"I don't have a verified citation for that — please check BAILII (bailii.org) or instruct a solicitor."*

---

## 1. Contract Formation

A valid contract under English law requires five elements:

### 1.1 Offer

An offer is an expression of willingness to contract on stated terms, made with the intention that it will become binding once accepted. Distinguish from an **invitation to treat**:

- **Display of goods in a shop** is an invitation to treat, not an offer: *Pharmaceutical Society of Great Britain v Boots Cash Chemists (Southern) Ltd* [1953] 1 QB 401.
- **Display of goods with a unilateral promise** may constitute an offer: *Carlill v Carbolic Smoke Ball Company* [1893] 1 QB 256 (CA).
- **Display of priced goods in a shop window** is an invitation to treat: *Fisher v Bell* [1961] 1 QB 394.
- **Advertisements** are generally invitations to treat unless they amount to a unilateral offer (*Carlill*).
- **Tenders** are generally invitations to treat; submission of a tender is the offer.

An offer may be revoked at any time before acceptance, provided revocation is communicated to the offeree: *Byrne & Co v Leon Van Tienhoven & Co* (1880) 5 CPD 344.

### 1.2 Acceptance

Acceptance must be unqualified and communicated to the offeror. A counter-offer destroys the original offer: *Hyde v Wrench* (1840) 3 Beav 334. The **postal rule** provides that acceptance by post takes effect on posting: *Adams v Lindsell* (1818) 1 B & Ald 681. The postal rule does not apply to instantaneous communications (*Entores Ltd v Miles Far East Corporation* [1955] 2 QB 327) nor, generally, to email.

### 1.3 Consideration

Consideration must be sufficient but need not be adequate: *Chappell & Co Ltd v Nestle Co Ltd* [1960] AC 87. Past consideration is not good consideration: *Re McArdle* [1951] Ch 669. Performance of an existing contractual duty is generally not good consideration (*Stilk v Myrick* (1809) 2 Camp 317), but a **practical benefit** can suffice: *Williams v Roffey Bros & Nicholls (Contractors) Ltd* [1991] 1 QB 1 (CA).

### 1.4 Intention to Create Legal Relations

Presumed present in commercial agreements: *Edwards v Skyways Ltd* [1964] 1 WLR 349. Presumed absent in domestic/social arrangements: *Balfour v Balfour* [1919] 2 KB 571 (CA). Both presumptions are rebuttable.

### 1.5 Capacity

Minors (under 18): contracts for necessaries are binding (Sale of Goods Act 1979, s.3); contracts of employment/apprenticeship are binding if substantially for the minor's benefit. Other contracts are voidable at the minor's option. Companies contract through their officers; capacity is governed by the Companies Act 2006, s.39 (power of directors to bind the company) and s.40 (third-party protection).

### 1.6 Deeds

A contract by deed requires no consideration. Requirements under **Law of Property (Miscellaneous Provisions) Act 1989, s.1**:

- The document must make clear on its face that it is intended to be a deed (s.1(2)(a)).
- It must be signed by the person making it in the presence of a witness who attests the signature, or at the maker's direction in the presence of two witnesses (s.1(3)).
- It must be delivered as a deed (s.1(3)(b)).

Ref: [LP(MP)A 1989, s.1](https://www.legislation.gov.uk/ukpga/1989/34/section/1)

---

## 2. Formal Requirements

Most contracts need not be in any particular form. Exceptions:

| Contract Type | Requirement | Authority |
|---|---|---|
| Sale or disposition of an interest in land | Must be in writing, signed by both parties, incorporating all expressly agreed terms in one document | LP(MP)A 1989, [s.2](https://www.legislation.gov.uk/ukpga/1989/34/section/2) |
| Guarantee (promise to answer for another's debt) | Must be evidenced in writing and signed by the guarantor | Statute of Frauds 1677, [s.4](https://www.legislation.gov.uk/aep/Cha2/29/3/section/IV) |
| Regulated consumer credit agreements | Must be in prescribed form, signed by the debtor; failure to comply renders the agreement improperly executed | Consumer Credit Act 1974, [ss.60-65](https://www.legislation.gov.uk/ukpga/1974/39/section/60) |
| Assignment of IP rights (copyright) | Must be in writing, signed by or on behalf of the assignor | Copyright, Designs and Patents Act 1988, [s.90(3)](https://www.legislation.gov.uk/ukpga/1988/48/section/90) |
| Lease for more than three years | Must be made by deed | Law of Property Act 1925, [s.52](https://www.legislation.gov.uk/ukpga/Geo5/15-16/20/section/52) |

---

## 3. Terms & Classification

### 3.1 Classification of Terms

- **Condition**: A fundamental term, breach of which entitles the innocent party to terminate and claim damages.
- **Warranty**: A lesser term, breach of which gives rise to damages only — no right to terminate.
- **Innominate term**: Classification depends on the consequences of the breach. If the breach deprives the innocent party of substantially the whole benefit, it may be treated as a breach of condition: *Hong Kong Fir Shipping Co Ltd v Kawasaki Kisen Kaisha Ltd* [1962] 2 QB 26 (CA).

### 3.2 Implied Terms — Sale of Goods

The **Sale of Goods Act 1979** (as amended) implies terms into contracts for the sale of goods:

| Section | Implied Term |
|---|---|
| [s.12](https://www.legislation.gov.uk/ukpga/1979/54/section/12) | Right to sell / quiet possession |
| [s.13](https://www.legislation.gov.uk/ukpga/1979/54/section/13) | Correspondence with description |
| [s.14(2)](https://www.legislation.gov.uk/ukpga/1979/54/section/14) | Satisfactory quality |
| [s.14(3)](https://www.legislation.gov.uk/ukpga/1979/54/section/14) | Fitness for particular purpose |
| [s.15](https://www.legislation.gov.uk/ukpga/1979/54/section/15) | Correspondence with sample |

For B2C sales, these implied terms are now superseded by **Consumer Rights Act 2015, Part 1** (goods: ss.9-18).

### 3.3 Implied Terms — Supply of Services

The **Supply of Goods and Services Act 1982** implies into B2B service contracts:

- **s.13**: Reasonable care and skill.
- **s.14**: Reasonable time for performance (where not fixed).
- **s.15**: Reasonable charge (where not determined).

For B2C service contracts, see **CRA 2015, ss.49-52**.

### 3.4 Entire Agreement Clauses

An entire agreement clause limits the contractual terms to those in the written document. It does not, by itself, exclude liability for misrepresentation: *AXA Sun Life Services plc v Campbell Martin Ltd* [2011] EWCA Civ 133. A separate non-reliance clause or explicit exclusion of misrepresentation liability is needed, subject to the reasonableness test under s.3 of the Misrepresentation Act 1967 (as substituted by UCTA 1977, s.8).

---

## 4. Unfair Terms

### 4.1 B2B Contracts — Unfair Contract Terms Act 1977 (UCTA)

UCTA applies to **exclusion and limitation clauses** in B2B contracts. Key provisions:

| Section | Rule |
|---|---|
| [s.2(1)](https://www.legislation.gov.uk/ukpga/1977/50/section/2) | **Cannot** exclude or restrict liability for death or personal injury resulting from negligence. Void. |
| [s.2(2)](https://www.legislation.gov.uk/ukpga/1977/50/section/2) | Exclusion of liability for other loss from negligence is subject to the **reasonableness test**. |
| [s.3](https://www.legislation.gov.uk/ukpga/1977/50/section/3) | Where one party deals on the other's written standard terms, exclusion of liability for breach and the right to render contractual performance substantially different or no performance at all are subject to reasonableness. |
| [s.6](https://www.legislation.gov.uk/ukpga/1977/50/section/6) | Implied terms as to title (SGA 1979, s.12) **cannot** be excluded. Other implied terms (ss.13-15) subject to reasonableness in B2B. |
| [s.7](https://www.legislation.gov.uk/ukpga/1977/50/section/7) | Similar to s.6 but for contracts of hire, exchange, and work-and-materials. |
| [s.11](https://www.legislation.gov.uk/ukpga/1977/50/section/11) | The **reasonableness test**: the term must be fair and reasonable having regard to the circumstances known or contemplated at the time of contracting. Schedule 2 provides guidelines. |

Practical guidance on Schedule 2 reasonableness factors: relative bargaining positions, whether the customer received an inducement, whether goods were specially made, whether the customer knew or ought to have known of the term.

### 4.2 B2C Contracts — Consumer Rights Act 2015, Part 2

CRA 2015, Part 2 ([ss.61-76](https://www.legislation.gov.uk/ukpga/2015/15/part/2)) replaces UCTA and UTCCR 1999 for consumer contracts:

- **Fairness test** (s.62): A term is unfair if, contrary to the requirement of good faith, it causes a significant imbalance in the parties' rights and obligations to the detriment of the consumer.
- **Core terms exemption** (s.64): Terms relating to the main subject matter or the price are exempt from the fairness assessment **only if** they are transparent and prominent.
- **Transparency** (s.68): Terms must be expressed in plain and intelligible language and be legible.
- **Grey list** (Schedule 2): An indicative list of terms that may be regarded as unfair — including terms giving the trader sole discretion on interpretation, requiring disproportionate sums on breach, permitting unilateral variation, and imposing excessive early-termination charges.
- **Effect of unfairness** (s.67): An unfair term is not binding on the consumer. The contract continues to exist so far as practicable without the unfair term.
- **Enforcement** (s.70): The Competition and Markets Authority (CMA) and sector regulators may take action against unfair terms.

### 4.3 Key Restrictions Applying to Both Regimes

A term that purports to exclude liability for death or personal injury caused by negligence is void (UCTA 1977, s.2(1); CRA 2015, s.65).

---

## 5. Misrepresentation

A misrepresentation is an unambiguous false statement of fact (not opinion, unless the opinion-holder has special knowledge: *Esso Petroleum Co Ltd v Mardon* [1976] QB 801) made by one party to induce the other to enter the contract.

### 5.1 Categories

| Type | Mental Element | Authority | Damages Measure |
|---|---|---|---|
| **Fraudulent** | Knowingly false, without belief in truth, or reckless | *Derry v Peek* (1889) 14 App Cas 337 (HL) | Tort: all direct loss, remoteness not applicable |
| **Negligent (common law)** | Failure to exercise reasonable care where a special relationship exists | *Hedley Byrne & Co Ltd v Heller & Partners Ltd* [1964] AC 465 (HL) | Tort: foreseeable loss |
| **Negligent (statutory)** | Representor unable to prove reasonable grounds for belief | Misrepresentation Act 1967, [s.2(1)](https://www.legislation.gov.uk/ukpga/1967/7/section/2) | Fiction of fraud: same measure as fraudulent (*Royscot Trust Ltd v Rogerson* [1991] 2 QB 297) |
| **Innocent** | Representor had reasonable grounds for belief | MA 1967, s.2(1) (by elimination) | Damages in lieu of rescission under MA 1967, [s.2(2)](https://www.legislation.gov.uk/ukpga/1967/7/section/2), at the court's discretion |

### 5.2 Remedies

- **Rescission**: Available for all three types, subject to the bars of affirmation, lapse of time, third-party rights, and impossibility of restitution.
- **Damages**: Available as of right for fraudulent and negligent (statutory) misrepresentation; at the court's discretion in lieu of rescission for innocent misrepresentation (MA 1967, s.2(2)).
- **Exclusion of liability**: Any clause excluding or restricting liability for misrepresentation is subject to the reasonableness test: MA 1967, s.3 (as substituted by UCTA 1977, s.8). In B2C contracts, such a clause is subject to the CRA 2015 fairness test.

---

## 6. Breach & Remedies

### 6.1 Types of Breach

- **Actual breach**: A party fails to perform an obligation when it falls due.
- **Anticipatory breach**: A party indicates, before performance is due, that they will not perform. The innocent party may accept the repudiation and sue immediately or affirm the contract and wait: *White & Carter (Councils) Ltd v McGregor* [1962] AC 413 (HL).

### 6.2 Damages

The fundamental principle is that damages place the innocent party in the position they would have been in had the contract been performed (the **expectation measure**): *Robinson v Harman* (1848) 1 Ex 850.

**Remoteness**: Damages are recoverable only for loss arising naturally from the breach (limb 1) or loss within the reasonable contemplation of the parties at the time of contracting (limb 2): *Hadley v Baxendale* (1854) 9 Ex 341. The test was restated in *Transfield Shipping Inc v Mercator Shipping Inc (The Achilleas)* [2008] UKHL 48 — the defendant must have assumed responsibility for the type of loss.

**Mitigation**: The innocent party must take reasonable steps to mitigate their loss: *British Westinghouse Electric and Manufacturing Co Ltd v Underground Electric Railways Co of London Ltd* [1912] AC 673 (HL).

**Contributory negligence**: Does not generally reduce contract damages, unless the claim is in tort concurrently: *Vesta v Butcher* [1989] AC 852.

### 6.3 Penalty Clauses and Liquidated Damages

The Supreme Court reformulated the penalty rule in *Cavendish Square Holding BV v Talal El Makdessi* [2015] UKSC 67:

- A clause is a penalty if it imposes a detriment on the contract-breaker out of all proportion to any legitimate interest of the innocent party in the enforcement of the primary obligation.
- The court will consider whether the innocent party has a **legitimate interest** in performance that extends beyond compensation for the breach.
- If the clause is a secondary obligation triggered by breach and is **extravagant, exorbitant, or unconscionable** relative to that legitimate interest, it is unenforceable.

On liquidated damages for delay, see *Triple Point Technology Inc v PTT Public Company Ltd* [2021] UKSC 29: liquidated damages accrue up to termination; after termination, the employer may claim general damages for the remaining period.

### 6.4 Specific Performance

An equitable remedy, available at the court's discretion where damages are inadequate. Generally available for contracts for the sale of land; generally not available for contracts of personal service. The court will consider whether constant supervision would be required: *Co-operative Insurance Society Ltd v Argyll Stores (Holdings) Ltd* [1998] AC 1 (HL).

### 6.5 Injunctions

An injunction may restrain a party from breaching a negative covenant (e.g., a non-compete obligation). The court will not grant a mandatory injunction that amounts to specific performance of a personal service contract.

---

## 7. Limitation Periods

The **Limitation Act 1980** ([full text](https://www.legislation.gov.uk/ukpga/1980/58/contents)) sets the time limits within which proceedings must be commenced.

### 7.1 Primary Periods

| Cause of Action | Period | Section |
|---|---|---|
| Simple contract (including debt) | **6 years** from accrual | [s.5](https://www.legislation.gov.uk/ukpga/1980/58/section/5) |
| Specialty (deed) | **12 years** from accrual | [s.8](https://www.legislation.gov.uk/ukpga/1980/58/section/8) |
| Tort (general) | **6 years** from accrual | [s.2](https://www.legislation.gov.uk/ukpga/1980/58/section/2) |
| Personal injury (tort or breach of duty) | **3 years** from accrual or date of knowledge | [s.11](https://www.legislation.gov.uk/ukpga/1980/58/section/11) |
| Defective products (CPA 1987) | **3 years** from damage/knowledge; **10-year** long-stop | [s.11A](https://www.legislation.gov.uk/ukpga/1980/58/section/11A) |
| Latent damage (negligence) | **6 years** from accrual **or 3 years** from date of knowledge (whichever expires later); **15-year** long-stop from breach | [s.14A](https://www.legislation.gov.uk/ukpga/1980/58/section/14A) / [s.14B](https://www.legislation.gov.uk/ukpga/1980/58/section/14B) |
| Contribution (Civil Liability (Contribution) Act 1978) | **2 years** from judgment or settlement | [s.10](https://www.legislation.gov.uk/ukpga/1980/58/section/10) |

### 7.2 Postponement and Extension

- **Fraud, concealment, or mistake**: Time does not begin to run until the claimant discovers (or could with reasonable diligence have discovered) the fraud, concealment, or mistake: LA 1980, [s.32](https://www.legislation.gov.uk/ukpga/1980/58/section/32).
- **Disability**: If the claimant is under a disability (minor or lacks mental capacity) when the cause of action accrues, time does not begin to run until the disability ceases: LA 1980, [s.28](https://www.legislation.gov.uk/ukpga/1980/58/section/28).
- **Acknowledgement or part-payment**: Resets the limitation clock: LA 1980, [ss.29-30](https://www.legislation.gov.uk/ukpga/1980/58/section/29).
- **Court discretion for personal injury**: The court may disapply the three-year limit if equitable: LA 1980, [s.33](https://www.legislation.gov.uk/ukpga/1980/58/section/33).

### 7.3 Practical Notes

- Time runs from the date the cause of action **accrues**, not from the date of the contract.
- For breach of contract, accrual is at the date of breach, not the date loss is suffered.
- For tortious negligence, accrual is when damage first occurs (which may differ from the date of the negligent act).
- Contractual limitation clauses that shorten the statutory period are valid in B2B contracts but subject to reasonableness under UCTA 1977, s.11, and in B2C contracts subject to the CRA 2015 fairness test.

---

## 8. Force Majeure & Frustration

### 8.1 Force Majeure

English law does **not** recognise a general doctrine of force majeure. The term has no statutory definition. Force majeure is a purely **contractual** concept: parties must include an express force majeure clause if they wish to be excused from performance on grounds of supervening events.

**Drafting considerations:**

- Define triggering events specifically (war, pandemic, government action, natural disaster, sanctions, etc.).
- State the consequences: suspension, extension of time, or termination.
- Require the affected party to give prompt notice and take reasonable steps to mitigate.
- Include a long-stop provision allowing termination if the force majeure event persists beyond a defined period.
- Address allocation of costs during the force majeure period.

Force majeure clauses are construed **strictly**: *Classic Maritime Inc v Limbungan Makmur Sdn Bhd* [2019] EWCA Civ 1102 (the party must show the event **caused** the failure to perform).

### 8.2 Frustration

Frustration discharges a contract automatically when a supervening event, for which neither party is responsible, renders performance impossible, illegal, or radically different from what was contemplated: *Taylor v Caldwell* (1863) 3 B & S 826; *National Carriers Ltd v Panalpina (Northern) Ltd* [1981] AC 675 (HL).

Frustration does **not** apply where:
- The event was foreseen or foreseeable and could have been provided for.
- The contract allocates the risk (e.g., via a force majeure clause).
- The event is self-induced.
- Performance is merely more expensive or difficult: *Davis Contractors Ltd v Fareham Urban District Council* [1956] AC 696 (HL).

### 8.3 Consequences of Frustration

The **Law Reform (Frustrated Contracts) Act 1943** ([full text](https://www.legislation.gov.uk/ukpga/Geo6/6-7/40/contents)) adjusts the parties' positions:

- **s.1(2)**: Money paid before frustration is recoverable. Money payable ceases to be payable. The court may allow the payee to retain or recover expenses incurred.
- **s.1(3)**: A party who has obtained a valuable benefit (other than money) before frustration may be required to pay a just sum for that benefit.

Note: The 1943 Act does **not** apply to insurance contracts, contracts for the carriage of goods by sea, or contracts for the sale of specific goods that have perished (SGA 1979, s.7).

---

## 9. Third Party Rights

### 9.1 Privity at Common Law

The doctrine of privity provides that only a party to a contract may enforce it: *Dunlop Pneumatic Tyre Co Ltd v Selfridge & Co Ltd* [1915] AC 847 (HL).

### 9.2 Contracts (Rights of Third Parties) Act 1999

The **Contracts (Rights of Third Parties) Act 1999** ([full text](https://www.legislation.gov.uk/ukpga/1999/31/contents)) creates a statutory exception:

- **s.1(1)(a)**: A third party may enforce a contractual term if the contract **expressly provides** that they may.
- **s.1(1)(b)**: A third party may enforce a term that purports to **confer a benefit** on them, unless it appears the parties did not intend the term to be enforceable by the third party (s.1(2)).
- **s.1(3)**: The third party must be **expressly identified** in the contract by name, as a member of a class, or by description (need not be in existence at the time of contracting).
- **s.2**: The contracting parties may not rescind or vary the contract so as to extinguish or alter the third party's entitlement without their consent once the third party has communicated assent, relied on the term, or the promisor is aware of such reliance.
- **s.3**: The promisor may raise against the third party any defence or set-off that would have been available against the promisee.

### 9.3 Excluding the Act

In commercial practice, it is standard to include an express exclusion clause:

> "A person who is not a party to this agreement shall not have any rights under the Contracts (Rights of Third Parties) Act 1999 to enforce any term of this agreement."

This is permitted by the Act (s.1(2) operates as a default, not a mandatory rule).

---

## 10. No Oral Modification Clauses

The Supreme Court in *Rock Advertising Ltd v MWB Business Exchange Centres Ltd* [2018] UKSC 24 held that **no oral modification (NOM) clauses are effective** in English law. A contract that requires variations to be in writing cannot be varied orally, even where both parties agree to the oral variation.

**Practical implications:**

- NOM clauses provide certainty and should be included as standard in commercial contracts.
- A party seeking to enforce an oral variation in the face of a NOM clause may need to rely on **estoppel** (Lord Sumption left this point open in *Rock Advertising*; the Court of Appeal subsequently considered it in *MWB Business Exchange Centres Ltd v Rock Advertising Ltd* [2016] EWCA Civ 553).
- Ensure that NOM clauses cover not just variations but also **waivers** and **consents** if intended.

---

## Quick Reference: Limitation Periods

| Claim | Limitation Period | Statute |
|---|---|---|
| Simple contract | 6 years | LA 1980, s.5 |
| Contract by deed | 12 years | LA 1980, s.8 |
| Tort (general) | 6 years | LA 1980, s.2 |
| Negligence (latent damage) | 6 years or 3 years from knowledge (whichever is later); 15-year long-stop | LA 1980, ss.14A-14B |
| Personal injury | 3 years from accrual or knowledge | LA 1980, s.11 |
| Defective products | 3 years from damage/knowledge; 10-year long-stop | LA 1980, s.11A |
| Contribution | 2 years from judgment/settlement | LA 1980, s.10 |
| Fraud / concealment / mistake | Time runs from discovery | LA 1980, s.32 |
| Acknowledgement / part-payment | Clock resets | LA 1980, ss.29-30 |

---

## Key Statute Reference Table

| Short Title | Citation | Link |
|---|---|---|
| Statute of Frauds 1677 | 29 Cha. 2, c. 3 | [legislation.gov.uk](https://www.legislation.gov.uk/aep/Cha2/29/3) |
| Law of Property Act 1925 | 15 & 16 Geo. 5, c. 20 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/Geo5/15-16/20) |
| Law Reform (Frustrated Contracts) Act 1943 | 6 & 7 Geo. 6, c. 40 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/Geo6/6-7/40) |
| Misrepresentation Act 1967 | c. 7 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1967/7) |
| Consumer Credit Act 1974 | c. 39 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1974/39) |
| Unfair Contract Terms Act 1977 | c. 50 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1977/50) |
| Sale of Goods Act 1979 | c. 54 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1979/54) |
| Limitation Act 1980 | c. 58 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1980/58) |
| Supply of Goods and Services Act 1982 | c. 29 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1982/29) |
| Copyright, Designs and Patents Act 1988 | c. 48 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1988/48) |
| Law of Property (Miscellaneous Provisions) Act 1989 | c. 34 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1989/34) |
| Contracts (Rights of Third Parties) Act 1999 | c. 31 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/1999/31) |
| Consumer Rights Act 2015 | c. 15 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/2015/15) |
| Companies Act 2006 | c. 46 | [legislation.gov.uk](https://www.legislation.gov.uk/ukpga/2006/46) |
