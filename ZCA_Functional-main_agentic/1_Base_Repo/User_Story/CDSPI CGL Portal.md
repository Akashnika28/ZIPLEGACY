# CDSPI Commercial General Liability Portal User Story

## User Story

As an authorized insurance product user,  
I want to enter, validate, quote, and manage CDSPI Commercial General Liability information through the portal,  
so that eligible risks receive accurate coverage, pricing, documentation, and policy processing.

## Requirements

1. The CDSPI CGL Portal and applicable CGL product options are available to authorized users for eligible applicants, jurisdictions, and transaction types.
2. The user can capture and maintain the required applicant, insured, contact, business, and mailing information.
3. The user can capture CGL operations, locations, classifications, payroll or sales exposures, subcontractor information, and other required underwriting data.
4. The user can select permitted CGL coverages, limits, deductibles, extensions, exclusions, and endorsements according to configured product rules.
5. The system applies CDSPI eligibility and underwriting rules and creates a referral or decline outcome when configured conditions are met.
6. The portal validates required and cross-field information, displays clear field-level messages, and prevents progression when blocking errors remain.
7. The system calculates and displays the CGL premium, applicable charges, taxes, and total premium using configured rating factors and exposure information.
8. The system attaches and generates the required CDSPI CGL forms, endorsements, schedules, disclosures, and supporting documents.
9. The user can save a draft, resume the transaction, quote, bind, and issue the policy after all required validations, referrals, and approvals are complete.
10. The portal displays saved CGL selections and transaction status in the policy summary and retains relevant inputs, changes, referrals, approvals, rating results, and document versions for audit purposes.

## Portal Workflow

1. The user authenticates and accesses the CDSPI CGL Portal.
2. The user starts a new CGL transaction or retrieves a saved transaction.
3. The user enters applicant, insured, business, location, operations, and exposure information.
4. The user selects applicable CGL coverages, limits, deductibles, exclusions, and endorsements.
5. The system validates the transaction and identifies errors, referrals, or decline conditions.
6. The user resolves blocking errors or required underwriting actions.
7. The system calculates the premium and displays the charges and policy summary.
8. The user saves, quotes, binds, and issues the policy, and the system generates the required documents.

## Acceptance Criteria

### AC1: Portal and Product Availability

Given an authorized user and an eligible applicant, jurisdiction, and transaction type,  
when the user opens the CDSPI CGL Portal,  
then the applicable CGL product options are available.

### AC2: Start or Resume a Transaction

Given the user has access to the portal,  
when the user starts a new transaction or retrieves a saved transaction,  
then the portal displays the correct CGL workflow and previously saved information, where applicable.

### AC3: Applicant and Risk Information

Given a new or saved CGL transaction,  
when the user enters valid applicant, insured, business, location, operations, classification, and exposure information,  
then the portal accepts and saves the information.

### AC4: Required-Field and Cross-Field Validation

Given required information is missing, invalid, or inconsistent,  
when the user attempts to continue,  
then the portal displays clear field-level validation messages and blocks progression until the blocking errors are resolved.

### AC5: Coverage Selection

Given valid CGL risk information,  
when the user selects permitted coverages, limits, deductibles, extensions, exclusions, or endorsements,  
then the portal accepts the selections and applies the configured product rules.

### AC6: Eligibility and Underwriting Referral

Given the risk meets a configured eligibility, referral, or decline condition,  
when the user attempts to quote or bind,  
then the system creates the appropriate outcome, displays the required message, and prevents completion until the required action is resolved.

### AC7: Rating and Quote

Given valid applicant, exposure, and coverage information,  
when the user requests a quote,  
then the system calculates and displays the correct premium, charges, taxes, and total premium.

### AC8: Policy Summary

Given valid saved transaction data,  
when the user opens the policy summary,  
then the portal displays the current CGL selections, exposure information, premium, transaction status, and effective date accurately.

### AC9: Forms and Documents

Given the selected coverage and transaction are eligible for documents,  
when the policy is quoted or issued,  
then the required CDSPI CGL forms, endorsements, schedules, disclosures, and supporting documents are attached with the correct version and effective date.

### AC10: Quote, Bind, and Issue

Given all validations, referrals, and approvals are complete,  
when the user quotes, binds, and issues the policy,  
then the policy status, CGL selections, rating results, and transaction data are saved correctly.

### AC11: Audit History

Given a saved transaction,  
when an authorized user reviews the transaction history,  
then relevant changes, referrals, approvals, rating inputs, generated documents, and document versions are available for audit.

## Open Items

- Authorized CDSPI portal roles and permitted transaction actions: [TBD]
- Eligible applicants, operations, classifications, jurisdictions, and transaction types: [TBD]
- Required and conditional applicant, location, operations, and exposure fields: [TBD]
- Available CGL coverages, limits, deductibles, extensions, exclusions, and endorsements: [TBD]
- Eligibility, referral, decline, and manual underwriting conditions: [TBD]
- Exposure factors, rating rules, taxes, and fees: [TBD]
- Required validation messages and policy status transitions: [TBD]
- Required forms, document editions, and effective dates: [TBD]
- Save-draft, resume, timeout, error, and recovery behavior: [TBD]
