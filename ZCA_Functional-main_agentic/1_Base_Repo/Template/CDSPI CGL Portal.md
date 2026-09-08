# CDSPI Commercial General Liability Portal Requirements Template

## Feature Information

**Feature name:** CDSPI Commercial General Liability Portal  
**Product:** Commercial General Liability (CGL)  
**Line of business:** Commercial General Liability  
**Jurisdiction:** [Enter province / territory]  
**Transaction type:** [New Business / Renewal / Policy Change]  
**Target release or effective date:** [Enter date]  
**Business owner:** [Enter owner]  
**Primary user roles:** [Broker / Underwriter / Service user / Other]

## Business Objective

[Describe the business need for the CDSPI CGL Portal, including the users, applicants, risks, and policy transactions supported.] 

## User Story

As an insurance product user,  
I want to enter, validate, quote, and manage CDSPI Commercial General Liability information through the portal,  
so that eligible risks receive accurate coverage, pricing, documentation, and policy processing.

## Scope

### In Scope

- CDSPI applicant, insured, business, and contact information
- CGL operations, locations, exposures, and claims information
- CGL coverage, limits, deductibles, exclusions, and endorsements
- Eligibility, underwriting referral, rating, and document behavior
- Save, validate, quote, bind, issue, and policy-summary workflow
- Portal navigation, user access, and audit history

### Out of Scope

- [Excluded product, line of business, or jurisdiction]
- [Excluded transaction type or portal function]
- [Known limitation]

## Requirements

**R1. Portal and Product Availability**  
The CDSPI CGL Portal and applicable CGL product options must be available to authorized users for eligible applicants, jurisdictions, and transaction types.

**R2. Applicant and Insured Information**  
The portal must allow the user to capture and maintain the required applicant, insured, contact, business, and mailing information.

**R3. Operations and Exposure Information**  
The portal must allow the user to capture CGL operations, locations, classifications, payroll or sales exposures, subcontractor information, and other underwriting data required for the risk.

**R4. Coverage Configuration**  
The user must be able to select permitted CGL coverages, limits, deductibles, extensions, exclusions, and endorsements according to the configured product rules.

**R5. Eligibility and Underwriting**  
The system must apply CDSPI eligibility and underwriting rules and create a referral or decline outcome when configured conditions are met.

**R6. Validation and Navigation**  
The portal must validate required and cross-field information at the appropriate workflow step, display clear field-level messages, and prevent progression when blocking errors remain.

**R7. Rating and Premium**  
The system must calculate and display the CGL premium, applicable charges, taxes, and total premium using the configured rating factors and exposure information.

**R8. Forms and Documents**  
The system must attach and generate the required CDSPI CGL forms, endorsements, schedules, disclosures, and supporting documents based on coverage, jurisdiction, transaction, and effective date.

**R9. Policy Workflow**  
The user must be able to save a draft, resume the transaction, quote, bind, and issue the policy after all required validations, referrals, and approvals are complete.

**R10. Policy Summary and Auditability**  
The portal must display the saved CGL selections and transaction status in the policy summary and retain relevant inputs, changes, referrals, approvals, rating results, and document versions for audit purposes.

## Portal Workflow

1. Authenticate the user and verify access to the CDSPI CGL Portal.
2. Start or retrieve a CGL transaction.
3. Enter applicant, insured, business, location, operation, and exposure information.
4. Select applicable CGL coverages, limits, deductibles, exclusions, and endorsements.
5. Validate the transaction and resolve errors or underwriting referrals.
6. Calculate and review the premium, charges, and policy summary.
7. Save, quote, bind, issue, and generate the required documents.

## Data Requirements

| Data Element | Required | Type / Format | Validation / Notes |
|---|---|---|---|
| Applicant / insured name | Yes | [Text] | [Enter rule] |
| Business name and contact details | Yes | [Text / contact] | [Enter rule] |
| Business operations | Yes | [Text / dropdown] | [Enter eligible operations] |
| Primary and additional locations | Yes | [Address] | [Enter jurisdiction rule] |
| CGL classification | Yes | [Dropdown] | [Enter allowed classifications] |
| Exposure basis and amount | Yes | [Currency / number] | [Enter exposure rules] |
| Subcontractor information | [Yes/No] | [Yes/No and details] | [Enter conditional rule] |
| Claims or incidents history | Yes | [Yes/No and details] | [Enter referral rule] |
| CGL coverage limit | Yes | [Currency / dropdown] | [Enter allowed limits] |
| Deductible | [Yes/No] | [Currency / dropdown] | [Enter allowed deductibles] |
| Optional coverages and endorsements | [Yes/No] | [Multi-select] | [Enter availability rules] |
| Effective date | Yes | [Date] | [Enter date constraints] |

## Acceptance Criteria

1. Given an authorized user and an eligible applicant, jurisdiction, and transaction type, when the user opens the CDSPI CGL Portal, then the applicable CGL product options are available.
2. Given a new or saved transaction, when the user enters valid applicant, insured, business, location, operations, and exposure information, then the portal accepts and saves the information.
3. Given required information is missing, invalid, or inconsistent, when the user attempts to continue, then the portal displays field-level validation messages and blocks progression.
4. Given valid risk information, when the user selects permitted CGL coverages, limits, deductibles, exclusions, or endorsements, then the portal accepts the selections and applies the configured rules.
5. Given valid rating inputs, when the user requests a quote, then the system calculates and displays the correct premium, charges, taxes, and total premium.
6. Given the risk meets an underwriting referral or decline condition, when the user attempts to quote or bind, then the system creates the configured outcome and prevents completion until the required action is resolved.
7. Given the selected coverage and transaction are eligible for documents, when the policy is quoted or issued, then the required CDSPI CGL documents are attached with the correct version and effective date.
8. Given all validations and approvals are complete, when the user binds and issues the policy, then the policy status, CGL selections, rating results, and transaction data are saved correctly.
9. Given a saved transaction, when the user returns to the portal, then the transaction can be resumed and the previously saved information is displayed accurately.
10. Given an authorized user reviews the policy history, when the transaction history is opened, then relevant changes, referrals, approvals, rating inputs, and generated documents are available for audit.

## Business Rules and Configuration

- Authorized portal roles and access permissions: [TBD]
- Eligible CDSPI applicants, operations, classifications, and jurisdictions: [TBD]
- Required and conditional applicant, location, operations, and exposure fields: [TBD]
- Coverage, limit, deductible, exclusion, and endorsement rules: [TBD]
- Claims, incident, subcontractor, and underwriting referral rules: [TBD]
- Decline conditions and referral messages: [TBD]
- Rating factors, exposure calculations, taxes, and fees: [TBD]
- Save-draft, resume, quote, bind, and issue status transitions: [TBD]
- Forms, document versions, and effective dates: [TBD]
- Portal timeout, session, error, and recovery behavior: [TBD]

## Integrations and Dependencies

| Component | Required Change / Dependency | Owner | Status |
|---|---|---|---|
| Portal UI | [Screens, navigation, controls, and validation] | [Team] | [TBD] |
| Identity and access | [Authentication and role permissions] | [Team] | [TBD] |
| Product model | [CDSPI CGL product and coverage configuration] | [Team] | [TBD] |
| Rating engine | [Exposure and coverage rating] | [Team] | [TBD] |
| Underwriting rules | [Eligibility, referral, and decline rules] | [Team] | [TBD] |
| Policy transaction service | [Save, quote, bind, and issue workflow] | [Team] | [TBD] |
| Forms and document service | [CGL forms, endorsements, and schedules] | [Team] | [TBD] |
| Audit service | [Change and approval history] | [Team] | [TBD] |

## Open Questions

- Which CDSPI users and roles can access the portal and each transaction action?
- Which applicants, operations, classifications, jurisdictions, and transaction types are eligible?
- Which portal sections, fields, and controls are mandatory or conditional?
- What CGL coverages, limits, deductibles, exclusions, and endorsements are available?
- Which conditions trigger referral, decline, or manual underwriting review?
- What exposure factors, rating rules, taxes, and fees apply?
- Which forms and document editions must be attached for each transaction and effective date?
- What save-draft, resume, timeout, error, and recovery behavior is required?
- What are the required validation messages and policy status transitions?
