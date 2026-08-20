# CDSPI Medical Malpractice Requirements Template

## Feature Information

**Feature name:** CDSPI Medical Malpractice  
**Product:** Medical Malpractice  
**Line of business:** [Enter applicable line of business]  
**Jurisdiction:** [Enter province / territory]  
**Target release:** [Enter release or effective date]  
**Business owner:** [Enter owner]

## Business Objective

[Describe the business need for the CDSPI Medical Malpractice product or change, including the customers, practitioners, or risks affected.]

## User Story

As an insurance product user,  
I want to quote and manage CDSPI Medical Malpractice coverage using the configured product rules,  
so that eligible risks receive accurate coverage, pricing, documentation, and policy processing.

## Scope

### In Scope

- [Coverage, endorsement, or workflow included]
- [User role or transaction type included]
- [Form, document, or integration included]

### Out of Scope

- [Excluded product, jurisdiction, or transaction]
- [Known limitation]

## Requirements

**R1. Product Availability**  
The CDSPI Medical Malpractice product must be available for [eligible user / jurisdiction / transaction] when the configured eligibility conditions are met.

**R2. Applicant and Risk Information**  
The system must allow the user to capture the required applicant, practitioner, practice, and risk information.

**R3. Eligibility and Underwriting**  
The system must validate the submitted information against the configured CDSPI Medical Malpractice eligibility and underwriting rules.

**R4. Coverage Selection**  
The user must be able to select the applicable coverage, limits, deductibles, endorsements, and optional protections permitted for the risk.

**R5. Rating and Premium**  
The system must calculate the premium using the configured rating factors and display the resulting premium and applicable charges accurately.

**R6. Validation and Referral**  
The system must display clear validation errors for invalid or incomplete information and refer risks requiring underwriting review according to the configured rules.

**R7. Forms and Documents**  
The system must attach and generate the required CDSPI Medical Malpractice forms and documents based on the selected coverage, jurisdiction, transaction, and effective date.

**R8. Policy Workflow**  
The user must be able to save, quote, bind, issue, or otherwise process the policy when all required validations and approvals are complete.

**R9. Auditability**  
The system must retain the selected coverage, rating inputs, referrals, approvals, generated documents, and relevant changes for audit purposes.

## Data Requirements

| Data Element | Required | Type / Format | Validation / Notes |
|---|---|---|---|
| Applicant / insured name | Yes | [Text] | [Enter rule] |
| Practitioner type / specialty | Yes | [Dropdown] | [Enter eligible values] |
| Practice location | Yes | [Address] | [Enter jurisdiction rule] |
| Years in practice | [Yes/No] | [Number] | [Enter range] |
| Coverage limit | Yes | [Currency / dropdown] | [Enter allowed limits] |
| Deductible | [Yes/No] | [Currency / dropdown] | [Enter allowed deductibles] |
| Prior claims / incidents | Yes | [Yes/No and details] | [Enter referral rule] |
| Effective date | Yes | [Date] | [Enter date constraints] |
| Additional risk information | [Yes/No] | [Text / attachment] | [Enter conditional rule] |

## Acceptance Criteria

1. Given an eligible applicant and jurisdiction, when the user starts a CDSPI Medical Malpractice transaction, then the product is available.
2. Given the product is available, when the user enters valid required applicant and risk information, then the system accepts the information.
3. Given required information is missing or invalid, when the user attempts to continue, then the system displays field-level validation messages and blocks progression.
4. Given valid risk information, when the user selects an allowed coverage limit and deductible, then the system accepts the selection and applies the configured rules.
5. Given valid rating inputs, when the user requests a quote, then the system calculates and displays the correct premium and applicable charges.
6. Given a risk meets an underwriting referral condition, when the user attempts to quote or bind, then the system creates the configured referral and prevents completion until the required action is resolved.
7. Given a coverage and transaction are eligible for documents, when the policy is quoted or issued, then the required CDSPI forms and documents are attached with the correct version and effective date.
8. Given all validations and approvals are complete, when the user completes the policy transaction, then the policy status and selected coverage details are saved correctly.
9. Given a saved transaction, when an authorized user reviews its history, then the relevant inputs, changes, referrals, approvals, and documents are available for audit.

## Business Rules and Configuration

- Eligibility rules: [TBD]
- Practitioner / specialty rules: [TBD]
- Territory or jurisdiction rules: [TBD]
- Coverage and limit rules: [TBD]
- Deductible rules: [TBD]
- Rating factors and premium calculation: [TBD]
- Underwriting referral rules and messages: [TBD]
- Forms, document versions, and effective dates: [TBD]
- Transaction-specific behavior: [New Business / Renewal / Policy Change / Cancellation]

## Integrations and Dependencies

| Component | Required Change / Dependency | Owner | Status |
|---|---|---|---|
| Product model | [TBD] | [Team] | [TBD] |
| Rating engine | [TBD] | [Team] | [TBD] |
| Underwriting rules | [TBD] | [Team] | [TBD] |
| Forms and document service | [TBD] | [Team] | [TBD] |
| External CDSPI integration | [TBD / Not applicable] | [Team] | [TBD] |

## Open Questions

- Which practitioners, specialties, and jurisdictions are eligible?
- What coverage limits, deductibles, and optional endorsements are available?
- Which fields are mandatory and which are conditional?
- What rating factors and premium calculation rules apply?
- Which conditions trigger referral, decline, or manual underwriting review?
- Which forms and document editions must be attached for each transaction and effective date?
- What are the required validation messages and policy status transitions?
