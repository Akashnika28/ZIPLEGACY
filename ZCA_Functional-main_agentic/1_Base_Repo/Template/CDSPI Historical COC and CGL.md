# CDSPI Historical COC and CGL Requirements Template

## Feature Information

**Feature name:** CDSPI Historical Certificate of Completion and Commercial General Liability  
**Product:** CDSPI [Enter product name]  
**Lines of business:** COC / Commercial General Liability (CGL)  
**Jurisdiction:** [Enter province / territory]  
**Transaction type:** [New Business / Renewal / Policy Change]  
**Target release or effective date:** [Enter date]  
**Business owner:** [Enter owner]

## Business Objective

[Describe the business need for capturing historical Certificate of Completion (COC) information and configuring Commercial General Liability coverage for CDSPI risks.]

## User Story

As an insurance product user,  
I want to capture and validate historical COC information while configuring CDSPI Commercial General Liability coverage,  
so that the system can accurately assess the risk, apply underwriting rules, calculate the premium, and generate the correct policy documentation.

## Scope

### In Scope

- Historical COC information capture and validation
- CDSPI CGL risk and coverage configuration
- Eligibility, underwriting referral, rating, and document behavior
- Save, quote, bind, and issue workflow

### Out of Scope

- [Excluded line of business or product]
- [Excluded historical period or transaction type]
- [Known limitation]

## Requirements

**R1. Product Availability**  
The CDSPI COC and CGL options must be available for eligible applicants, jurisdictions, and transaction types.

**R2. Historical COC Information**  
The system must allow the user to capture historical COC details, including the completion date, project or risk description, applicable limits, and supporting documentation where required.

**R3. COC Validation**  
The system must validate required historical COC fields, date rules, limits, and document requirements before the policy can proceed.

**R4. CGL Risk Information**  
The system must allow the user to capture the required applicant, business, operations, location, exposure, and claims information for CGL underwriting.

**R5. Coverage Configuration**  
The user must be able to select permitted CGL coverages, limits, deductibles, extensions, exclusions, and endorsements according to the configured product rules.

**R6. Eligibility and Underwriting**  
The system must apply CDSPI eligibility and underwriting rules to the historical COC and CGL information and create a referral or decline outcome when configured conditions are met.

**R7. Rating and Premium**  
The system must calculate and display the CGL premium, applicable charges, and total premium using the configured rating factors and exposure information.

**R8. Forms and Documents**  
The system must attach and generate the required COC and CGL forms, endorsements, disclosures, and supporting documents based on coverage, jurisdiction, transaction, and effective date.

**R9. Policy Workflow**  
The user must be able to save, quote, bind, and issue the policy after all required validations, referrals, and approvals are complete.

**R10. Auditability**  
The system must retain historical COC values, CGL selections, rating inputs, referrals, approvals, document versions, and relevant changes for audit purposes.

## Data Requirements

| Data Element | Required | Type / Format | Validation / Notes |
|---|---|---|---|
| Applicant / insured name | Yes | [Text] | [Enter rule] |
| Business name and operations | Yes | [Text / dropdown] | [Enter eligible values] |
| COC status | Yes | [Dropdown] | [Enter allowed statuses] |
| COC completion date | Yes | [Date] | [Enter date constraints] |
| Project or risk description | Yes | [Text] | [Enter length and content rules] |
| Historical COC limits | [Yes/No] | [Currency] | [Enter minimum / maximum] |
| Supporting COC document | [Yes/No] | [Attachment] | [Enter file and document rule] |
| CGL operations and exposures | Yes | [Text / number] | [Enter exposure rules] |
| CGL coverage limit | Yes | [Currency / dropdown] | [Enter allowed limits] |
| CGL deductible | [Yes/No] | [Currency / dropdown] | [Enter allowed deductibles] |
| Claims or incidents history | Yes | [Yes/No and details] | [Enter referral rules] |
| Effective date | Yes | [Date] | [Enter date constraints] |

## Acceptance Criteria

1. Given an eligible applicant, jurisdiction, and transaction type, when the user starts the CDSPI COC and CGL transaction, then the applicable product options are available.
2. Given the COC section is available, when the user enters valid historical COC information, then the system accepts and saves the information.
3. Given required COC information or supporting documentation is missing or invalid, when the user attempts to continue, then the system displays field-level validation messages and blocks progression.
4. Given valid CGL risk information, when the user selects permitted coverages, limits, deductibles, extensions, or endorsements, then the system accepts the selections and applies the configured rules.
5. Given valid COC, CGL, and exposure information, when the user requests a quote, then the system calculates and displays the correct premium and applicable charges.
6. Given the historical COC or CGL risk meets an underwriting referral condition, when the user attempts to quote or bind, then the system creates the configured referral and prevents completion until it is resolved.
7. Given the selected coverage and transaction are eligible for documents, when the policy is quoted or issued, then the required COC and CGL documents are attached with the correct version and effective date.
8. Given all validations and approvals are complete, when the user binds and issues the policy, then the policy status, historical COC information, and CGL selections are saved correctly.
9. Given a saved transaction, when an authorized user reviews the history, then the COC values, CGL changes, referrals, approvals, rating inputs, and documents are available for audit.

## Business Rules and Configuration

- Eligible CDSPI applicants, operations, and jurisdictions: [TBD]
- Historical period covered by COC information: [TBD]
- COC completion-date and expiry rules: [TBD]
- COC document and attachment requirements: [TBD]
- CGL coverage, limit, deductible, and endorsement rules: [TBD]
- CGL exposure and rating factors: [TBD]
- Claims, incident, and underwriting referral rules: [TBD]
- Decline conditions and referral messages: [TBD]
- Forms, document versions, and effective dates: [TBD]
- Transaction-specific behavior: [New Business / Renewal / Policy Change]

## Integrations and Dependencies

| Component | Required Change / Dependency | Owner | Status |
|---|---|---|---|
| Product model | [COC and CGL configuration] | [Team] | [TBD] |
| Rating engine | [Exposure and coverage rating] | [Team] | [TBD] |
| Underwriting rules | [Eligibility and referral rules] | [Team] | [TBD] |
| Document service | [COC and CGL forms / attachments] | [Team] | [TBD] |
| Claims or history data | [Historical data source, if applicable] | [Team] | [TBD] |
| Audit service | [Change and approval history] | [Team] | [TBD] |

## Open Questions

- What does COC represent in the CDSPI workflow, and which historical periods are required?
- Which applicants, operations, jurisdictions, and transaction types are eligible?
- Which COC fields and supporting documents are mandatory or conditional?
- What CGL coverages, limits, deductibles, extensions, and endorsements are available?
- Which historical COC or CGL conditions trigger referral, decline, or manual underwriting review?
- What rating factors and exposure calculations apply?
- Which forms and document editions must be attached for each transaction and effective date?
- What are the required validation messages and policy status transitions?
