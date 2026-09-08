# CMW Strata Requirements Template

## Feature Information

**Feature name:** CMW Strata  
**Product:** Commercial Strata  
**Line of business:** [Enter applicable line of business]  
**Jurisdiction:** [Enter province / territory]  
**Transaction type:** [New Business / Renewal / Policy Change]  
**Target release or effective date:** [Enter date]  
**Business owner:** [Enter owner]

## Business Objective

[Describe the business need for quoting and managing CMW Strata risks, including the strata corporation, building, units, common property, exposures, and insurance requirements affected.]

## User Story

As an insurance product user,  
I want to quote and manage CMW Strata coverage using the configured product and underwriting rules,  
so that the strata risk receives accurate protection, pricing, documentation, and policy processing.

## Scope

### In Scope

- Strata corporation, building, unit, and common-area information
- Property, liability, equipment, and optional strata coverage configuration
- Eligibility, underwriting referral, rating, and document behavior
- Save, quote, bind, and issue workflow

### Out of Scope

- [Excluded product, building type, or jurisdiction]
- [Excluded transaction or coverage]
- [Known limitation]

## Requirements

**R1. Product Availability**  
The CMW Strata product must be available for eligible strata risks, jurisdictions, building types, and transaction types.

**R2. Strata and Building Information**  
The system must allow the user to capture the strata corporation, building address, construction, occupancy, age, number of units, and common-property information required for underwriting.

**R3. Exposure Information**  
The system must allow the user to capture applicable property values, replacement cost, unit and common-area exposures, amenities, parking, utilities, and loss-prevention details.

**R4. Coverage Configuration**  
The user must be able to select permitted property, liability, equipment breakdown, directors and officers, and other optional strata coverages, limits, deductibles, exclusions, and endorsements.

**R5. Eligibility and Underwriting**  
The system must apply configured CMW Strata eligibility and underwriting rules and create a referral or decline outcome when configured conditions are met.

**R6. Rating and Premium**  
The system must calculate and display the premium, applicable charges, and total premium using the configured building, exposure, coverage, location, and risk factors.

**R7. Validation**  
The system must display clear validation errors for missing, invalid, or inconsistent strata and building information before the policy can proceed.

**R8. Forms and Documents**  
The system must attach and generate the required CMW Strata forms, schedules, endorsements, disclosures, and supporting documents based on coverage, jurisdiction, transaction, and effective date.

**R9. Policy Workflow**  
The user must be able to save, quote, bind, and issue the policy after all required validations, referrals, and approvals are complete.

**R10. Auditability**  
The system must retain strata details, building exposures, coverage selections, rating inputs, referrals, approvals, document versions, and relevant changes for audit purposes.

## Data Requirements

| Data Element | Required | Type / Format | Validation / Notes |
|---|---|---|---|
| Strata corporation name | Yes | [Text] | [Enter rule] |
| Building address and jurisdiction | Yes | [Address] | [Enter territory rule] |
| Building type and construction | Yes | [Dropdown] | [Enter allowed values] |
| Year built or last major update | Yes | [Year] | [Enter range] |
| Number of units | Yes | [Number] | [Enter minimum / maximum] |
| Occupancy and unit mix | Yes | [Text / number] | [Enter eligible values] |
| Building replacement cost | Yes | [Currency] | [Enter valuation rule] |
| Common property and amenities | [Yes/No] | [Checkbox / text] | [Enter conditional rule] |
| Property coverage limit | Yes | [Currency / dropdown] | [Enter allowed limits] |
| Liability coverage limit | Yes | [Currency / dropdown] | [Enter allowed limits] |
| Deductible | [Yes/No] | [Currency / dropdown] | [Enter allowed deductibles] |
| Claims or loss history | Yes | [Yes/No and details] | [Enter referral rule] |
| Effective date | Yes | [Date] | [Enter date constraints] |

## Acceptance Criteria

1. Given an eligible strata risk, jurisdiction, building type, and transaction type, when the user starts a CMW Strata transaction, then the product is available.
2. Given the product is available, when the user enters valid strata corporation, building, unit, and common-property information, then the system accepts and saves the information.
3. Given required or inconsistent strata information is missing or invalid, when the user attempts to continue, then the system displays field-level validation messages and blocks progression.
4. Given valid exposure information, when the user selects permitted strata coverages, limits, deductibles, exclusions, or endorsements, then the system accepts the selections and applies the configured rules.
5. Given valid building, exposure, and coverage information, when the user requests a quote, then the system calculates and displays the correct premium and applicable charges.
6. Given the strata risk meets an underwriting referral or decline condition, when the user attempts to quote or bind, then the system creates the configured outcome and prevents completion until the required action is resolved.
7. Given the selected coverage and transaction are eligible for documents, when the policy is quoted or issued, then the required CMW Strata forms and documents are attached with the correct version and effective date.
8. Given all validations and approvals are complete, when the user binds and issues the policy, then the policy status, strata details, building exposures, and coverage selections are saved correctly.
9. Given a saved transaction, when an authorized user reviews the history, then the relevant changes, rating inputs, referrals, approvals, and documents are available for audit.

## Business Rules and Configuration

- Eligible strata corporations, building types, operations, and jurisdictions: [TBD]
- Construction, occupancy, unit-count, and building-age rules: [TBD]
- Replacement-cost and valuation rules: [TBD]
- Property, liability, equipment, and optional coverage rules: [TBD]
- Coverage limits, deductibles, exclusions, and endorsements: [TBD]
- Amenities, parking, commercial-unit, and common-property rules: [TBD]
- Claims, loss-history, risk, and underwriting referral rules: [TBD]
- Decline conditions and referral messages: [TBD]
- Rating factors and premium calculation: [TBD]
- Forms, document versions, and effective dates: [TBD]
- Transaction-specific behavior: [New Business / Renewal / Policy Change]

## Integrations and Dependencies

| Component | Required Change / Dependency | Owner | Status |
|---|---|---|---|
| Product model | [CMW Strata product and coverage configuration] | [Team] | [TBD] |
| Rating engine | [Building, exposure, and coverage rating] | [Team] | [TBD] |
| Underwriting rules | [Eligibility, referral, and decline rules] | [Team] | [TBD] |
| Property valuation data | [Replacement-cost source, if applicable] | [Team] | [TBD] |
| Document service | [CMW Strata forms and schedules] | [Team] | [TBD] |
| Audit service | [Change and approval history] | [Team] | [TBD] |

## Open Questions

- What does CMW represent, and which strata risks and jurisdictions are supported?
- Which building types, construction types, occupancy types, and unit counts are eligible?
- Which building, unit, common-property, amenities, and exposure fields are mandatory or conditional?
- What valuation method and replacement-cost rules apply?
- Which property, liability, equipment, and optional coverages are available?
- Which risk conditions trigger referral, decline, or manual underwriting review?
- What rating factors and premium calculations apply?
- Which forms and document editions must be attached for each transaction and effective date?
- What are the required validation messages and policy status transitions?
