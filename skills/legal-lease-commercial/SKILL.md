---
name: legal-lease-commercial
description: "Use this skill when reviewing commercial leases, retail leases, NNN leases, or mixed-use lease agreements. Triggers include: any mention of CAM reconciliation, percentage rent, co-tenancy, lease renewal options, holdover provisions, or requests to review a lease document from a landlord or asset manager perspective. Also use for compliance analysis of existing tenant leases, redline comparison of lease versions, or identification of missing landlord protections. Do NOT use for residential leases, P3 ground leases, or loan documents — use the appropriate skill for those."
version: "1.0"
---

# /legal lease-commercial — Commercial Lease Review

## Command
```
/legal lease-commercial <file>
```

## Purpose
Specialized commercial lease review from the **landlord/asset manager perspective**. Analyzes NNN, gross, and modified gross lease structures with emphasis on CAM reconciliation, rent escalation, default triggers, and tenant protections that may erode NOI. Built for Spectrum Properties' multifamily-adjacent retail and mixed-use portfolio.

---

## What It Returns

### 1. Lease Safety Score (0–100)
- **A (85–100):** Landlord-favorable, well-structured
- **B (70–84):** Acceptable with minor gaps
- **C (55–69):** Material risks present, negotiate before executing
- **D (<55):** Significant exposure — do not execute without legal review

### 2. Lease Type Classification
- NNN / Modified Gross / Gross / Percentage Rent
- Identifies mismatches between lease label and actual economics

### 3. Financial Exposure Dashboard
| Risk Area | Finding | Severity |
|---|---|---|
| CAM cap structure | Uncapped / capped at X% | HIGH / MED / LOW |
| Rent escalation | Fixed % / CPI / None | |
| Exclusivity clause | Present / Absent / Overly broad | |
| Co-tenancy trigger | Present / Absent | |
| Percentage rent threshold | Natural breakpoint analysis | |
| Personal guarantee | Full / Limited / Absent | |

### 4. Clause-by-Clause Analysis
For each major clause: plain English summary → landlord risk score (1–10) → recommended action.

**Clauses reviewed:**
- Base Rent & Escalation
- CAM / Operating Expense Definitions and Caps
- Percentage Rent & Gross Sales Reporting
- Use Clause (permitted, exclusive, prohibited)
- Assignment & Subletting
- Renewal Options (terms, notice windows, rent reset method)
- Expansion / ROFR / ROFO Rights
- Co-Tenancy Provisions
- Default & Cure Periods
- Holdover Rent
- Landlord Access Rights
- Alterations & Restoration
- Signage Rights
- Personal Guarantee
- Estoppel & SNDA Requirements
- Force Majeure
- Lease Termination / Early Exit Options

### 5. CAM Deep Dive
- Identifies controllable vs. uncontrollable expense definitions
- Flags missing or weak audit rights
- Highlights exclusions that shift costs to landlord
- Checks for gross-up provisions on vacant space
- Reviews cap methodology (base year, cumulative vs. non-cumulative)

### 6. Sales Reporting & Percentage Rent Compliance
- Validates reporting frequency requirements
- Flags audit rights and enforcement mechanisms
- Maps to Spectrum's existing PAL0616-style compliance tracking framework
- Identifies natural breakpoint vs. artificial breakpoint structures

### 7. Missing Protections
Common landlord protections that should be present but are absent:
- Personal guarantee or corporate guarantee
- Estoppel certificate delivery obligation
- SNDA subordination language
- Landlord audit rights for gross sales
- CAM audit rights with time limitations
- Restoration obligation on tenant improvements
- Assignment consent standard (not to be unreasonably withheld — flag if absent)

### 8. Negotiation Priorities
Ranked list of the highest-leverage items to push back on, with suggested replacement language.

### 9. Obligations & Key Dates Timeline
| Event | Trigger | Deadline | Consequence of Miss |
|---|---|---|---|
| Renewal notice | X months before expiration | [Date] | Option lapses |
| CAM audit window | Annual reconciliation | 90 days | Rights waived |
| Sales report due | Monthly / Annual | [Date] | Default |

---

## Agents (Parallel Execution)

| Agent | File | Role | Weight |
|---|---|---|---|
| Clause Analyst | `agents/legal-clauses.md` | Identifies and categorizes every clause | 20% |
| Risk Assessor | `agents/legal-risks.md` | Scores each clause for landlord risk | 25% |
| CAM Specialist | `agents/lease-cam.md` | Deep CAM and operating expense analysis | 20% |
| Compliance Checker | `agents/legal-compliance.md` | Flags Texas landlord-tenant law issues | 15% |
| Recommendations Engine | `agents/legal-recommendations.md` | Generates specific fix language | 20% |

---

## Texas Governance & Legal Context

### Applicable Statutes
- **Texas Property Code Chapter 91** — Landlord-tenant rights, notice requirements
- **Texas Property Code Chapter 93** — Commercial tenancies, lockout and lien rights
- **Texas Business & Commerce Code** — UCC provisions affecting leasehold interests
- **Texas Tax Code § 11.182** — Property tax implications of leasehold arrangements

### Market Standards Reference
- DFW Class B/C retail NNN CAM caps: typically 3–5% annually, non-cumulative
- Personal guarantee standard: 12–24 months of base rent for new tenants
- Holdover: 150% of final month's rent is market standard
- Audit rights window: typically 12 months post-reconciliation statement

### Spectrum-Specific Flags
- **Percentage Rent:** Cross-reference against PAL0616 compliance framework — flag any lease where espresso/food/beverage sales >10% of gross without audit rights
- **Assignment:** Flag any clause that would allow assignment without landlord consent in a mixed-use property context
- **Use Clause:** Confirm use restrictions align with adjacent tenant mix in Spectrum's portfolio

---

## Usage Examples

```
/legal lease-commercial retail-lease-draft.pdf
/legal lease-commercial PAL0616-current-lease.pdf
/legal lease-commercial new-tenant-loi-redline.pdf
```

---

## Output Format
Returns structured markdown report. Pair with `/legal report-pdf` to generate a professional PDF version for ownership review or lender submission.

---

## Related Commands
| Command | Use When |
|---|---|
| `/legal compare <file1> <file2>` | Comparing redline versions of the same lease |
| `/legal negotiate <file>` | Need counter-proposal language for specific clauses |
| `/legal missing <file>` | Quick scan for absent landlord protections only |
| `/legal report-pdf` | Generate PDF version of this analysis |
| `/legal p3-rfp <file>` | For ground leases within P3 development structures |
