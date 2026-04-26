---
name: legal-ground-lease-improvement-lease-structure
description: Reference for the two-document leasehold architecture used to deliver a privately developed, leased-back facility — a Ground Lease (covering the land) paired with an Improvement Lease (covering the building) executed simultaneously between a landowner, a developer/SPE, and a tenant. Use this whenever the user is reviewing, drafting, negotiating, or analyzing a transaction that splits land and improvements ownership across two leases, regardless of the underlying transaction type — Texas Chapter 2267 P3 implementations, federal GSA build-to-suits, university or hospital build-to-suits, corporate sale-leasebacks, sale-leaseback-with-development structures, and any deal where a private developer constructs a facility on land it does not own and leases it to a creditworthy occupant. Trigger this skill on phrases like "ground lease," "improvement lease," "two-lease structure," "ground lease + sublease," "developer-built leased-back," "leasehold mortgage," "ground-lease build-to-suit," "P3 lease structure," "fee subordination," "leasehold reversion," or any review of a long-term lease where the lessee is a special-purpose entity and the lessor is the landowner. Trigger even when the user only mentions one of the two leases, because the structural questions almost always require analyzing both. This skill addresses the lease architecture only — the statutory P3 framework (Texas Chapter 2267) and CTL financing mechanics have their own skills.
---

# Ground Lease + Improvement Lease Structural Reference

The two-lease architecture is the dominant implementation pattern for transactions that split land ownership from improvements ownership and lease the resulting building back to a creditworthy occupant. The Ground Lease puts the land under the developer/SPE for a long term; the Improvement Lease puts the finished building under the occupant. The two leases sign simultaneously and operate as a coordinated unit.

This skill addresses the lease architecture itself. It applies whether the deal is a Texas Chapter 2267 P3, a corporate sale-leaseback, a federal GSA build-to-suit, or a private institutional BTS. The statutory P3 framework and the CTL loan that typically finances the structure are addressed in sibling skills.

## Why the architecture exists

A two-lease structure does four things that no single document can do as cleanly:

1. **Splits ownership cleanly.** Landowner keeps the fee; developer/SPE owns the leasehold and the improvements during the term; occupant has possession during the rent-paying period. Each party's interest is held in its own document, with its own rules.
2. **Supports CTL financing.** The Improvement Lease is the bondable lease that the CTL loan underwrites; the Ground Lease provides the leasehold estate that the CTL lender mortgages. Without the split, neither piece works as well.
3. **Preserves federal tax depreciation at the SPE level.** The SPE's equitable ownership of the improvements during the term is what supports MACRS depreciation, true-lease characterization, and §179D-type deduction eligibility (where applicable). A single combined instrument muddies this.
4. **Manages property tax exposure.** In governmental contexts, the split lets the public landowner retain fee ownership for exemption purposes (e.g., Texas Tax Code §11.11) while the SPE holds a leasehold that may or may not trigger a taxable leasehold interest analysis (e.g., §25.07). The drafting of each lease drives the outcome.

If the deal in front of you doesn't need at least two of these four, ask whether a two-lease structure is actually warranted. It adds complexity that should be paid for by structural benefits.

## The Ground Lease — core terms

The Ground Lease runs from the landowner (lessor) to the developer/SPE (lessee). Its job is to give the SPE enough leasehold tenure to develop, finance, lease back, and operate the building for the full Improvement Lease term, with margin on each end.

### Term layering

The Ground Lease term is **longer** than the Improvement Lease term. The standard layering:

- **Development Period.** Ground Lease begins; SPE designs and constructs the building. Typically 1–3 years. Improvement Lease is executed at the same time but its rent-paying period does not start until certificate of occupancy.
- **Rent-Paying Period.** Improvement Lease rent commences at CO and runs the negotiated term — commonly 25–30 years for institutional CTL deals.
- **Lender Tail.** The Ground Lease extends 1–5 years past the Improvement Lease's scheduled termination, giving the CTL lender time to relet or work out the asset on a default scenario near maturity.

A Ground Lease term equal to the Improvement Lease term is a structural error — it leaves the lender with no tail and the SPE with no operating runway after improvement-lease default. Confirm both leases' term diagrams line up.

### Rent

Ground rent is deal-specific. Three common patterns:

- **Nominal ground rent ($1/year or similar)** — when the landowner is also the underlying tenant (e.g., a city ground-leasing to the SPE that will then improvement-lease back to the same city). The economics flow through the Improvement Lease.
- **Market ground rent** — arm's-length deals where the landowner expects an income return on the land.
- **Stepped or escalating rent** — hybrid; sometimes used to align with Improvement Lease escalators or to protect the landowner against long-term inflation.

### Permitted use and use restrictions

The Ground Lease should expressly authorize: (a) construction of the specified improvements, (b) sublease to the occupant via the Improvement Lease, and (c) leasehold mortgage to a CTL lender. Anything broader than necessary creates inadvertent flexibility the landowner may not want; anything narrower threatens financeability.

### Leasehold mortgage authorization

This is the structural hinge. The Ground Lease must:

- **Expressly authorize** a leasehold mortgage to one or more institutional lenders.
- **Run notice of default** to the leasehold mortgagee whenever the SPE is in default under the Ground Lease, with copies of every notice the SPE receives.
- **Give the leasehold mortgagee a cure period** at least as long as the SPE's, plus reasonable extension if cure requires possession or remedies.
- **Provide a new-lease option** if the Ground Lease is rejected in the SPE's bankruptcy — the leasehold mortgagee can step into a new ground lease on the same terms for the remaining term.
- **Permit assignment of the leasehold mortgage** to a successor lender or to a foreclosure purchaser without ground lessor consent (or with consent not unreasonably withheld).
- **Survive estoppels and recognition agreements** — the ground lessor signs estoppels and a recognition/non-disturbance agreement to the leasehold mortgagee at lender's request.

A Ground Lease without these protections is unfinanceable. If the landowner is a governmental body, expect resistance to some of these — work each through with the lender's checklist in hand.

### Reversion and surrender

At Ground Lease termination (scheduled or earlier), the improvements revert to the landowner. The reversion mechanism must be operative — typically a quitclaim or special warranty deed conveying the SPE's leasehold and improvements interest — not just a recital that "improvements shall revert." Surrender condition is typically as-is at termination, subject to maintenance covenants during the term.

## The Improvement Lease — core terms

The Improvement Lease runs from the SPE (landlord) to the occupant (tenant). Its job is to deliver the building to the occupant on terms that (a) the occupant can accept, (b) support CTL financing, and (c) preserve true-lease characterization.

### Term

Commences at certificate of occupancy. Commonly 25–30 years for institutional CTL deals; shorter for corporate BTS, longer for some public-sector deals. The non-cancelable term must be long enough to amortize the CTL debt with margin.

### Rent and payment structure

Economic rent calibrated to debt service + return + (in some structures) operating costs. The Improvement Lease must be **absolute net** — see the CTL skill for the bondable-lease attributes that drive this.

For governmental tenants, payment must be **use-based abatement, not annual appropriation**. The constitutional debt analysis under the applicable state's framework drives this; in Texas, Tex. Const. Art. III §49 and Art. XI §5 are the operative provisions. Annual appropriation walk-aways defeat CTL execution.

### Use restrictions

Defined and exclusive. The occupant uses the building for its specified purpose. Changes of use require landlord and lender consent.

### Abatement and termination triggers

Abatement should be limited to:

- **Total casualty or condemnation** with insurance/condemnation proceeds prepaying the CTL debt.
- **For governmental tenants only — actual vacation and surrender of beneficial use** as the use-based abatement trigger satisfying the constitutional debt test.

Anything broader (rent abatement during repair, partial-condemnation abatement, repair-and-deduct, offset for landlord defaults) is inconsistent with bondable-lease requirements and must be either eliminated, narrowed, or backed by insurance.

### Default and cure

Tenant default: standard rent and covenant defaults with cure periods. Landlord default: limited, because the Improvement Lease should impose minimal landlord obligations once the building is delivered (consistent with absolute-net structure).

### Assignment and sublet

Limited. Tenant cannot transfer to a non-credit party without landlord and lender consent — the lender underwrote the credit, and changing it changes the loan.

### Reversion and surrender

At Improvement Lease termination, the building reverts to the ground lessor (typically through the operation of the Ground Lease) or, in non-ground-lease structures, to the fee owner. The mechanic must be operative.

## Allocation of rights between the two leases

The two leases govern overlapping subject matter. Drafting needs to assign each topic clearly to one lease, with cross-references where coordination is required.

| Topic | Lease that controls |
|---|---|
| Land use, environmental, surface rights | Ground Lease |
| Building occupancy, operations, interior maintenance | Improvement Lease |
| Leasehold mortgage and lender protections | Ground Lease (primary); Improvement Lease references and SNDA |
| Construction obligations and standards | Ground Lease (during Development Period); Improvement Lease for tenant build-out if any |
| Casualty / condemnation of land | Ground Lease |
| Casualty / condemnation of building | Improvement Lease (with cross-reference to Ground Lease) |
| Insurance — property | Improvement Lease (tenant obligation in absolute-net structures) |
| Insurance — liability | Improvement Lease primarily; Ground Lease for ground lessor's interests |
| Reversion of improvements | Ground Lease (operative mechanism); Improvement Lease references |
| Cross-default | Both leases (each lease defaulted by default of the other) |

Cross-defaults are typical and appropriate — the two leases are economically a unit, and a default under one should be capable of being treated as a default under both. Bound the cross-default to material defaults to avoid cascading remedies on minor breaches.

## Equitable ownership for federal tax purposes

The federal tax outcome depends on which party is treated as equitable owner of the improvements during the term:

- **SPE as equitable owner (the goal).** SPE depreciates the improvements (typically 39-year straight-line for nonresidential commercial under MACRS, with cost segregation as a complementary strategy). Tenant deducts rent. SPE retains residual value subject to reversion. Lease characterized as a true lease (Rev. Rul. 55-540; Rev. Proc. 2001-28; Rev. Proc. 2001-29).
- **Tenant as equitable owner (catastrophic).** Tax-recharacterized installment sale. SPE loses depreciation. Tenant loses rent deductions. Both parties have to redo the deal.

Three drafting points preserve SPE equitable ownership:

1. **No tenant purchase option** — especially no bargain or fixed-price option. Reversion at termination is the public-side ownership pathway, not an option. (See the CTL skill for the full multi-pillar argument against options.)
2. **SPE retains meaningful residual.** The improvements must have real value at lease end, and the SPE must be at risk on it. A lease term equal to the building's useful life with no residual is an installment-sale signal.
3. **No "rent" payments that build tenant equity.** Rent must look like rent, not principal amortization disguised as rent.

Get a true-lease tax opinion at closing whenever the deal has any installment-sale-adjacent feature.

## Property tax analysis (Texas as the primary illustration)

The two-lease structure interacts with state property tax law in ways that drive significant economic outcomes. Using Texas as the primary example — the structural pattern translates to other states with their own statutory frameworks.

### Texas Tax Code §11.11 — public property exemption

Property owned by a political subdivision and used for public purposes is exempt from ad valorem taxation. The exemption requires:

- **Public ownership** — the political subdivision must hold the fee.
- **Public purpose use** — the property must be used by the political subdivision for public purposes.

In a two-lease P3 where the city is fee owner (ground lessor) and ultimate occupant (improvement lessee), the §11.11 analysis turns on whether the city holds sufficient equitable interest in the improvements to qualify them as "publicly owned" for exemption purposes. This is a structural drafting question: the leases must give the city enough equitable indicia (reversion, control, public-purpose use) to support the exemption while not so much that they collapse SPE equitable ownership for federal tax. The line is real but navigable.

### Texas Tax Code §25.07 — taxable leasehold interests

Where the fee is exempt, a private leasehold interest in the property may be separately taxable if it has independent value and meets the §25.07 criteria. The risk in a two-lease structure is that the SPE's leasehold under the Ground Lease is taxed even though the underlying fee is exempt under §11.11.

Mitigation strategies:

- **Calibrate the leasehold's terms** so it does not have independent ascertainable value beyond the rent obligation.
- **Use absolute-net pass-through structures** so that any §25.07 tax flows to the tenant rather than the SPE.
- **Confirm with the local appraisal district** in advance — many district practices treat structured P3 leaseholds favorably.

### Other states

Most states have analogous frameworks (public property exemption + taxable leasehold interest doctrine). The structural pattern is the same — preserve the public exemption on the fee while managing leasehold tax exposure. Confirm with local counsel on each transaction; do not generalize Texas analysis to other jurisdictions.

## Reversion vs. purchase option — the public ownership pathway

Public landowners frequently want a path to ultimate ownership of the improvements. The structurally sound path is **reversion at Ground Lease termination**, not a tenant purchase option.

| Reversion at termination | Tenant purchase option |
|---|---|
| Operates by passage of time and existing contract | Operates by tenant election |
| No future financial commitment by public party | Creates future financial commitment — constitutional debt risk |
| Preserves true-lease characterization | Triggers installment-sale recharacterization risk |
| Compatible with CTL prepayment restrictions | Generally prohibited by CTL lender (forced prepayment) |
| Already in the leases | Adds risk for no benefit (the public party already gets the building at term) |

The CTL skill develops this argument at length. For the two-lease drafting question, the upshot is: **build reversion mechanics into the Ground Lease and reject any purchase option, however framed.** "Right of first refusal," "right of first offer," and similar variants share most of the option's structural problems and should be rejected on the same grounds unless drafted very narrowly to avoid the recharacterization triggers.

## Lender protections — coordinating with the CTL loan

The CTL skill specifies what the lender needs from the lease and the borrower. In the two-lease architecture, those protections are spread across both leases:

**In the Ground Lease (primary).**

- Leasehold mortgage authorization
- Notice of default to leasehold mortgagee
- Cure period for leasehold mortgagee
- New-lease option on bankruptcy rejection
- Assignment / foreclosure permitted
- Recognition of leasehold mortgagee's successor

**In the Improvement Lease.**

- SNDA from the tenant in lender's favor
- Estoppel from the tenant
- No modification of the Improvement Lease without lender consent
- Lease assignment to lender on default
- Direct payment to lender on default (lockbox or assignment of rents)

These provisions must be drafted as a coordinated package. A robust Ground Lease leasehold mortgagee protection clause is useless if the Improvement Lease lets the tenant terminate for casualty without lender consent.

## Casualty and condemnation

The two-lease structure handles casualty and condemnation events separately for land and building.

- **Total casualty (building destroyed)** — Improvement Lease typically continues with rebuild obligation (insurance proceeds escrowed and disbursed) OR terminates with insurance proceeds prepaying CTL debt. Bondable-lease drafting prefers continuation.
- **Partial casualty** — rebuild obligation; rent typically continues; insurance proceeds applied to repair.
- **Total condemnation** — both leases terminate; condemnation proceeds prepay CTL debt; surplus to ground lessor and SPE per a defined waterfall.
- **Partial condemnation** — leases continue with rent abatement on lost area only; condemnation proceeds applied to restoration or to debt amortization.

Casualty and condemnation provisions are heavily lender-driven. Confirm the language matches the lender's term sheet before circulating drafts.

## Insurance

In an absolute-net Improvement Lease, the tenant carries property and liability insurance covering the building, with the SPE/landlord and the CTL lender as additional insureds and loss payees. The Ground Lease addresses ground lessor's liability protection. Builders risk during the Development Period is the SPE/developer's responsibility. Rent loss / business interruption insurance is matched to the CTL debt service term.

## Common drafting traps

Recurring problems in two-lease structures:

- **Term mismatch** — Ground Lease term equal to Improvement Lease term, no lender tail. Restructure.
- **Reversion language without operative mechanism** — "shall revert" with no deed or transfer mechanic. Add the operative provision.
- **Inadequate leasehold mortgagee protections** in the Ground Lease. Compare against the CTL lender's checklist.
- **Property tax exemption analysis missing or assumed.** Run §11.11 / §25.07 (or local equivalents) explicitly.
- **Cross-default not bilateral or overbroad.** Bound to material defaults under either lease.
- **"Limited landlord obligations" not actually limited** in the Improvement Lease — every landlord obligation is a CTL exception.
- **Annual appropriation language anywhere** in the Improvement Lease. Replace with use-based abatement.
- **Purchase option in any form** — option, ROFR, ROFO, fixed-price exercise window, contingent option. Reject and route to reversion.
- **Simultaneity not memorialized.** Both leases must be expressed to sign simultaneously and to operate as a unit; cross-references and recitals should make this explicit.

## Review checklist

When applying this skill to a two-lease deal:

1. Confirm the **two leases sign simultaneously** and are expressed as a coordinated unit.
2. Confirm **term layering**: Development Period + Improvement Lease rent-paying period + Lender Tail. Diagram the timeline.
3. Confirm **reversion** (not purchase option) is the ownership-transfer mechanism, with operative deed/transfer mechanic.
4. Confirm **federal tax equitable ownership** rests with the SPE — no purchase option, meaningful residual, true-lease characterization.
5. Confirm **property tax analysis** under the applicable state framework — public exemption preserved, leasehold tax exposure managed.
6. Confirm **leasehold mortgagee protections** in the Ground Lease match the CTL lender's checklist.
7. Confirm **absolute-net structure** and **use-based abatement** (governmental tenants) in the Improvement Lease, consistent with CTL bondable-lease requirements.
8. Confirm **cross-defaults** are bilateral, bounded to material defaults, and operationally executable.
9. Confirm **casualty and condemnation** mechanics match the lender's term sheet.
10. **Rank issues.** Structural disqualifiers > tax/financing exposure > drafting cleanup. Don't list issues without ranking them.

## What this skill does NOT cover

- **Statutory P3 framework** (Texas Chapter 2267, mandatory CA terms, public-interest protections, P3 Guidelines) — separate skill.
- **CTL loan terms and lender mechanics** (bondable-lease attributes, tenant credit analysis, prepayment, capital markets execution) — separate skill.
- **Detailed federal tax structuring** (cost segregation, §179D, §48E, §30C, tax credits and incentives) — separate analysis with tax counsel.
- **Detailed state-specific property tax law** beyond Texas illustration — local counsel.
- **Equity / SPE governance** (operating agreement, member protections, depreciation allocation, refinancing triggers among equity holders) — separate analysis.
- **Construction documents** (design-build contract, GMP, schedule, completion guarantees) — separate.

When any of these intersects the two-lease drafting work, name the gap explicitly and pull the relevant skill or counsel in.

## Composition with sibling skills

A typical deal review uses this skill alongside:

- **`chapter-2267-comprehensive-agreement`** — for Texas governmental P3 transactions, the statutory umbrella that authorizes the lease structure.
- **`ctl-loan`** — the financing overlay that drives many of the lease drafting decisions (absolute net, term, payment structure, lender protections).

Apply only the skills the deal actually triggers. A corporate ground-lease build-to-suit triggers this skill and the CTL skill but not the Chapter 2267 skill. A Chapter 2267 deal implemented as a single concession agreement triggers the Chapter 2267 and CTL skills but not this one. A Chapter 2267 deal with a two-lease implementation and CTL financing triggers all three.
