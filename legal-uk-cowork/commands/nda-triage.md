---
description: Triage an NDA under English law — classify as GREEN (sign), YELLOW (flag), or RED (reject)
argument-hint: "<paste or describe the NDA>"
---

# /nda-triage — UK NDA Screening

Triage an NDA under English law using the nda-triage skill knowledge.

NDA input: @$1

$ARGUMENTS

## Instructions

1. Use the nda-triage skill to perform a full UK-specific NDA screening
2. Accept the NDA as pasted text, uploaded file, or description
3. Screen against English law NDA norms including:
   - Standard exclusions from confidentiality
   - Restraint of trade doctrine
   - UCTA 1977 reasonableness
   - UK GDPR implications for personal data
   - Competition Act 1998 considerations
4. Classify as:
   - **GREEN** — safe to sign, market-standard for English law
   - **YELLOW** — flag specific clauses with a solicitor before signing
   - **RED** — do not sign, material issues requiring negotiation
5. Output a structured triage report with clause-by-clause analysis
6. Always include the SRA Warning Notice compliant disclaimer

If no NDA is provided, prompt the user to paste or upload the NDA text, or ask about UK NDA norms generally.
