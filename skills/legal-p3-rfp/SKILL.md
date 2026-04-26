---
name: legal-p3-rfp
description: "Use this skill when reviewing, drafting, or analyzing Public-Private Partnership (P3) RFP documents, RFQ responses, development agreements, ground leases within P3 structures, or any municipal procurement document governed by Texas Chapter 2267. Triggers include: any mention of P3, public-private partnership, design-build-finance, DBF, Chapter 2267, CTL financing, Credit Tenant Lease, ground lease for public facility, city hall, municipal building, or requests to review an RFP from a developer/proposer perspective. Do NOT use for standard commercial leases, residential leases, or private-sector-only development agreements — use legal-lease-commercial or legal-dev-agreement for those."
version: "1.0"
---

# /legal p3-rfp — P3 RFP & Development Agreement Review

## Command
```
/legal p3-rfp <file>
```

## Purpose
Specialized review of P3 procurement documents, RFPs, RFQs, and development agreements from the **developer/proposer perspective** under Texas Chapter 2267. Designed for Design-Build-Finance (DBF) opportunities with Texas municipalities, with specific emphasis on CTL financing compatibility, risk allocation, and proposal compliance requirements.

---

## What It Returns

### 1. P3 Feasibility Score (0–100)
- **A (85–100):** Highly structured, CTL-compatible, clear risk allocation
- **B (70–84):** Viable with identified gaps — addressable in proposal
- **C (55–69):** Material ambiguities — requires clarification requests before proposing
- **D (<55):** Poorly structured — significant legal/financial risk to developer

### 2. Chapter 2267 Compliance Check
Verifies the RFP/procurement process conforms to Texas Government Code Chapter 2267:
- Qualifying Project determination
- Responsible Governmental Entity (RGE) authority confirmation
- Comprehensive Agreement requirements present
- Public notice and competitive process compliance
- Required provisions: audit rights, step-in rights, termination structure
- Revenue sharing and fee structure disclosure

### 3. CTL Financing Compatibility Analysis
Critical for Design-Build-Finance structures with JLL or similar placement agents:

| CTL Factor | RFP Language | Compatible? | Issue |
|---|---|---|---|
| Lease term (min 20yr) | Found / Not found | Yes / No | |
| Tenant credit quality | Municipality identified | Yes / No | |
| Absolute NNN structure | Present / Absent | Yes / No | |
| Assignment to lender | Permitted / Restricted | Yes / No | |
| SNDA / Lender protections | Present / Absent | Yes / No | |
| Appropriations risk | Annual / Multi-year | Risk / OK | |
| Termination for convenience | Present / Absent | Risk / OK | |

### 4. Risk Allocation Dashboard

| Risk Category | Allocated To | Market Standard | Flag |
|---|---|---|---|
| Design & construction | Developer / Municipality | Developer | |
| Cost overrun | Developer / Shared | Developer | |
| Schedule delay | Developer / Shared | Shared | |
| Force majeure | Developer / Shared / Neutral | Neutral | |
| Permitting & entitlements | Developer / Municipality | Municipality | |
| Environmental | Developer / Municipality | Shared | |
| Operating cost post-delivery | Municipality / Developer | Municipality | |
| Financing rate risk | Developer | Developer | |

### 5. Clause-by-Clause Analysis
For each major section: plain English summary → developer risk score (1–10) → recommended action or clarification request.

**Sections reviewed:**
- Project Scope & Specifications
- Qualifying Project Determination
- Proposer Qualifications & Experience Requirements
- Proposal Submission Requirements
- Evaluation Criteria & Weighting
- Comprehensive Agreement Terms
- Ground Lease Structure (if applicable)
- Lease Term, Rent, and Escalation
- Design-Build Requirements & Performance Standards
- Financing Plan Requirements
- Construction Timeline & Milestones
- Commissioning & Acceptance
- Operations & Maintenance Obligations (if any)
- Lender/Investor Protections
- Step-In Rights
- Default, Cure, and Termination
- Revenue Sharing or Availability Payments
- Intellectual Property & Data Rights
- Dispute Resolution
- Governing Law & Venue

### 6. Proposal Compliance Checklist
Line-by-line checklist of every submission requirement in the RFP — confirms what must be included in the proposal response and flags missing items.

| Requirement | Section | Required By | Status |
|---|---|---|---|
| Qualifications narrative | 3.1 | Mandatory | ✅ / ❌ |
| Financial statements | 3.4 | Mandatory | ✅ / ❌ |
| Financing commitment letter | 4.2 | Mandatory | ✅ / ❌ |
| Design concept | 5.1 | Mandatory | ✅ / ❌ |
| DBE/HUB participation plan | 6.0 | Mandatory | ✅ / ❌ |

### 7. Missing Protections (Developer Perspective)
Protections that should be present but are absent:
- Lender step-in rights / cure period before termination
- Non-disturbance agreement for lender
- Independent cost verification process
- Change order dispute resolution mechanism
- Force majeure definition broad enough to cover financing market disruption
- Developer right to cure municipal default
- Buyout / termination payment formula favoring developer recovery of sunk costs
- Appropriations covenant (multi-year funding commitment)

### 8. Clarification Questions to Submit
Ranked list of questions to submit during the RFP Q&A period, ordered by impact on deal feasibility.

### 9. Deal Structure Recommendation
Based on RFP analysis, recommends optimal deal structure:
- Ground lease vs. installment sale
- DBF vs. DBFOM
- CTL vs. conventional construction financing
- Recommended Comprehensive Agreement negotiation priorities

---

## Agents (Parallel Execution)

| Agent | File | Role | Weight |
|---|---|---|---|
| Clause Analyst | `agents/legal-clauses.md` | Identifies and categorizes every clause | 15% |
| Risk Assessor | `agents/legal-risks.md` | Scores each clause for developer risk | 20% |
| Compliance Checker | `agents/legal-compliance.md` | Chapter 2267 and Texas procurement compliance | 25% |
| CTL Specialist | `agents/p3-ctl.md` | CTL financing compatibility analysis | 25% |
| Recommendations Engine | `agents/legal-recommendations.md` | Generates clarification questions and fix language | 15% |

---

## Texas Governance & Legal Context

### Primary Statutes
- **Texas Government Code Chapter 2267** — Public and Private Facilities and Infrastructure; Qualifying Projects
- **Texas Government Code Chapter 2166** — State Facilities Construction (for state-level projects)
- **Texas Local Government Code Chapter 271** — Municipal purchasing and contracting authority
- **Texas Property Code Chapter 64** — Ground lease structures for public facilities
- **Texas Constitution Article III § 52** — Prohibition on lending credit; public purpose doctrine

### CTL Market Standards (DFW)
- Lease term: 20–30 years minimum for CTL execution
- Tenant: Investment-grade municipality or backed by appropriations covenant
- Structure: Absolute NNN with no landlord obligations post-delivery
- Financing: 65–75% LTV typical on CTL; JLL and similar place with life insurance companies
- Rate environment: Spread over 10-yr Treasury; lock timing is critical
- SNDA: Lender requires subordination, non-disturbance, and attornment from tenant

### Chapter 2267 Key Requirements
- RGE must make Qualifying Project finding before soliciting proposals
- Comprehensive Agreement required — cannot be waived
- Developer must demonstrate financing capability
- Public notice required — minimum 45 days for proposals
- Revenue sharing terms must be disclosed in RFP
- Step-in rights for lenders must be negotiated into Comprehensive Agreement

### Spectrum / iBOS Deal Context
- **Active deal:** City of Lancaster — ~30,000 SF city hall, ~$28M, DBF structure
- **Secondary target:** Dallas City Hall relocation
- **Financing partner:** JLL for CTL placement
- Flag any RFP language that would prevent CTL execution or lender assignment
- Flag any appropriations risk language — annual appropriations = CTL killer

---

## Usage Examples

```
/legal p3-rfp lancaster-city-hall-rfp.pdf
/legal p3-rfp dallas-municipal-rfp.pdf
/legal p3-rfp development-agreement-draft.pdf
```

---

## Output Format
Returns structured markdown report. Pair with `/legal report-pdf` for ownership presentation or lender submission package.

---

## Related Commands
| Command | Use When |
|---|---|
| `/legal lease-commercial <file>` | Ground lease component of a P3 deal |
| `/legal compare <file1> <file2>` | Comparing RFP versions or Comprehensive Agreement redlines |
| `/legal negotiate <file>` | Generating counter-language for Comprehensive Agreement |
| `/legal missing <file>` | Quick scan for absent developer protections only |
| `/legal compliance <url>` | Municipal website compliance audit for P3 eligibility |
| `/legal report-pdf` | Generate PDF for ownership or lender submission |
