# Everest COC Requirements Template

## Feature Information

**Feature name:** Everest COC [Enter full feature name]  
**Product / line of business:** [Enter product and line of business]  
**Meaning of COC in this workflow:** [Confirm full term]  
**Jurisdiction:** [Enter province / territory / state]  
**Transaction type:** [New Business / Renewal / Policy Change / Other]  
**Target release or effective date:** [Enter date]  
**Business owner:** [Enter owner]  
**Primary user roles:** [Broker / Underwriter / Service user / Other]

## Business Objective

[Describe the business need for the Everest COC workflow, including who uses it, which risks or policies it supports, and the expected business outcome.]

## User Story

As an authorized insurance user,  
I want to capture, validate, and process the required Everest COC information,  
so that eligible risks can be assessed and processed with the correct coverage, decisions, and documentation.

## Scope

### In Scope

- [COC information and related risk details]
- [Eligibility and underwriting behavior]
- [Coverage, limits, and rating behavior, if applicable]
- [Validation, workflow, and document behavior]
- [Save, quote, bind, issue, or other applicable transaction actions]

### Out of Scope

- [Excluded product, line of business, jurisdiction, or transaction]
- [Excluded workflow or portal capability]
- [Known limitation]

## Requirements

**R1. Product and Workflow Availability**  
The Everest COC workflow must be available to authorized users for configured eligible risks, jurisdictions, and transaction types.

**R2. Risk and Applicant Information**  
The system must allow the user to capture and maintain the applicant, insured, contact, risk, and location information required for the workflow.

**R3. COC Information**  
The system must allow the user to capture the COC details required for the selected product and transaction, including applicable status, dates, description, limits, and supporting information.

**R4. Validation**  
The system must validate required fields, formats, date constraints, and configured cross-field rules before the user can proceed.

**R5. Eligibility and Underwriting**  
The system must apply configured Everest eligibility and underwriting rules and return the appropriate acceptance, referral, or decline outcome.

**R6. Coverage and Rating**  
Where applicable, the system must allow permitted coverage selections and calculate the premium, charges, and total using configured rating inputs.

**R7. Documents**  
The system must attach or generate the required COC-related forms and supporting documents based on the configured product, jurisdiction, transaction, and effective date.

**R8. Transaction Workflow**  
The user must be able to save and complete the applicable transaction actions after required validations, referrals, and approvals are resolved.

**R9. Summary and Auditability**  
The system must display the current COC information and transaction status and retain relevant inputs, decisions, approvals, and document versions for audit purposes.

## Workflow

1. Authenticate the user and verify access to the Everest COC workflow.
2. Start a new transaction or retrieve a saved transaction.
3. Enter applicant, insured, risk, location, and COC information.
4. Select applicable coverage or complete related product information, if required.
5. Validate the transaction and resolve errors, referrals, or approval requirements.
6. Review the outcome, premium, and transaction summary, where applicable.
7. Save and complete the applicable transaction actions; generate required documents.

## Data Requirements

| Data Element | Required | Type / Format | Validation / Notes |
|---|---|---|---|
| Applicant / insured name | [Yes/No] | [Text] | [Enter rule] |
| Contact information | [Yes/No] | [Email / phone / other] | [Enter format rules] |
| Risk or project description | [Yes/No] | [Text] | [Enter length and content rules] |
| Risk / insured location | [Yes/No] | [Address] | [Enter jurisdiction rules] |
| COC type or status | [Yes/No] | [Dropdown] | [Confirm meaning and allowed values] |
| COC effective / completion date | [Yes/No] | [Date] | [Enter date constraints] |
| COC expiry date | [Yes/No] | [Date] | [Enter date and relationship rules] |
| Applicable limits or values | [Yes/No] | [Currency / number] | [Enter permitted values and ranges] |
| Supporting documentation | [Yes/No] | [Attachment] | [Enter file and conditional requirements] |
| Coverage selection | [Yes/No] | [Dropdown / multi-select] | [Enter allowed options, if applicable] |
| Effective date | [Yes/No] | [Date] | [Enter transaction-specific rules] |

## Acceptance Criteria

1. Given an authorized user and an eligible risk, when the user opens the Everest COC workflow, then the configured options for the applicable jurisdiction and transaction are available.
2. Given a new or saved transaction, when the user enters valid required risk and COC information, then the system accepts and saves the information.
3. Given required information is missing or invalid, when the user attempts to continue, then the system displays clear field-level validation messages and blocks progression where the error is blocking.
4. Given the entered information meets a configured referral or decline condition, when the system evaluates the transaction, then the appropriate outcome is displayed and further processing follows the configured rules.
5. Given coverage or rating applies to the transaction, when the user selects permitted options and requests a quote, then the system calculates and displays the configured premium and charges.
6. Given the transaction is eligible for documents, when the applicable processing step is completed, then the required documents are generated or attached with the correct version and effective date.
7. Given all required validations, referrals, and approvals are complete, when the user completes the transaction, then the final status and COC information are saved accurately.
8. Given a saved transaction, when an authorized user reviews its history, then relevant changes, decisions, approvals, and documents are available for audit.

## Business Rules and Configuration

- Full meaning and business purpose of COC: [TBD]
- Eligible applicants, risks, operations, jurisdictions, and transaction types: [TBD]
- Required and conditional COC fields: [TBD]
- COC status, effective-date, completion-date, and expiry rules: [TBD]
- Supporting document requirements and permitted file types: [TBD]
- Coverage options, limits, exclusions, or endorsements, if applicable: [TBD]
- Eligibility, referral, decline, and approval conditions: [TBD]
- Rating inputs, calculations, charges, and taxes, if applicable: [TBD]
- Required forms, document versions, and effective dates: [TBD]
- Save, resume, quote, bind, issue, and status-transition behavior: [TBD]
- Validation messages and error-recovery behavior: [TBD]

## Integrations and Dependencies

| Component | Required Change / Dependency | Owner | Status |
|---|---|---|---|
| User interface / portal | [Screens, navigation, controls, and validation] | [Team] | [TBD] |
| Identity and access | [Authentication and role permissions] | [Team] | [TBD] |
| Product model | [Everest product and COC configuration] | [Team] | [TBD] |
| Underwriting rules | [Eligibility, referral, and decline rules] | [Team] | [TBD] |
| Rating engine | [Rating inputs and calculations, if applicable] | [Team] | [TBD] |
| Policy transaction service | [Save and transaction workflow] | [Team] | [TBD] |
| Forms and document service | [COC forms and supporting documents] | [Team] | [TBD] |
| Audit service | [Change and decision history] | [Team] | [TBD] |

## Open Questions

- What does COC stand for in the Everest workflow, and what business process does it support?
- Which products, risks, jurisdictions, and transaction types are in scope?
- Which fields and supporting documents are required or conditional?
- What are the COC date, status, limit, and expiry rules?
- Which conditions result in referral, decline, or approval?
- Does the workflow include coverage selection, rating, quoting, binding, or issuance?
- Which forms and document versions must be produced?
- What user roles, access permissions, and audit details are required?
