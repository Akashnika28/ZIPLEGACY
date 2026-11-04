# Everest COC User Story

## Feature Context

**Product / line of business:** [TBD]  
**Meaning of COC:** [TBD]  
**Jurisdiction:** [TBD]  
**Transaction type:** [New Business / Renewal / Policy Change / Other - confirm]  
**Primary user roles:** [TBD]

## User Story

As an authorized insurance user,  
I want to capture, validate, and process the required Everest COC and risk information,  
so that eligible risks can be assessed and processed with the correct decisions, coverage, and documentation.

## Requirements

1. The Everest COC workflow is available to authorized users for configured eligible risks, jurisdictions, and transaction types.
2. The user can start a new transaction or retrieve and resume a saved transaction.
3. The user can enter the applicant, insured, contact, risk, location, and COC information required for the selected product and transaction.
4. The system validates required fields, formats, date constraints, and configured cross-field rules, and prevents progression when blocking errors remain.
5. The system applies configured Everest eligibility and underwriting rules and returns the appropriate acceptance, referral, or decline outcome.
6. Where coverage or rating applies, the user can select permitted options and the system calculates and displays the configured premium and charges.
7. The system attaches or generates required COC-related forms and supporting documents based on the configured product, jurisdiction, transaction, and effective date.
8. The user can complete applicable transaction actions after required validations, referrals, and approvals are resolved.
9. The system displays the current COC information and transaction status and retains relevant inputs, decisions, approvals, and document versions for audit purposes.

## Workflow

1. The user authenticates and accesses the Everest COC workflow.
2. The user starts a new transaction or retrieves a saved transaction.
3. The user enters applicant, insured, risk, location, and COC information.
4. The user completes applicable product or coverage information.
5. The system validates the transaction and identifies errors, referrals, or approval requirements.
6. The user resolves blocking errors and completes required underwriting actions.
7. The system displays the applicable decision, premium, and transaction summary.
8. The user saves or completes the applicable transaction actions, and the system generates required documents.

## Acceptance Criteria

### AC1: Workflow Availability

Given an authorized user and a configured eligible risk, jurisdiction, and transaction type,  
when the user opens the Everest COC workflow,  
then the applicable workflow and product options are available.

### AC2: Start or Resume a Transaction

Given the user has permission to access the workflow,  
when the user starts a new transaction or retrieves a saved transaction,  
then the system displays the appropriate workflow and restores previously saved information, where applicable.

### AC3: Capture Risk and COC Information

Given a new or saved transaction,  
when the user enters valid required applicant, insured, risk, location, and COC information,  
then the system accepts and saves the information.

### AC4: Field and Cross-Field Validation

Given required information is missing, invalid, or inconsistent with a configured rule,  
when the user attempts to continue,  
then the system displays a clear validation message for the affected information and blocks progression when the error is blocking.

### AC5: Eligibility and Underwriting Outcome

Given the transaction information meets a configured eligibility, referral, or decline condition,  
when the system evaluates the transaction,  
then it displays the appropriate outcome and enforces the configured next steps.

### AC6: Coverage and Rating (If Applicable)

Given the transaction includes coverage selection and rating,  
when the user selects permitted options and requests a quote,  
then the system calculates and displays the configured premium and applicable charges.

### AC7: Documents

Given the transaction is eligible for COC-related documents,  
when the applicable processing step is completed,  
then the system generates or attaches the required documents with the correct version and effective date.

### AC8: Complete Transaction

Given all required validations, referrals, and approvals are complete,  
when the user completes the applicable transaction action,  
then the system saves the final status and COC information accurately.

### AC9: Audit History

Given a saved transaction,  
when an authorized user reviews its history,  
then relevant changes, decisions, approvals, rating inputs where applicable, and generated documents are available for audit.

## Open Items

- Confirm the full meaning and business purpose of COC in the Everest workflow.
- Identify the products, risks, operations, jurisdictions, and transaction types in scope.
- Define required and conditional applicant, risk, location, and COC fields.
- Define COC status, effective-date, completion-date, limit, and expiry rules.
- Define supporting document requirements and permitted file types.
- Confirm whether coverage selection, rating, quoting, binding, and issuance apply.
- Define eligibility, referral, decline, and approval conditions.
- Identify required forms, document versions, and effective dates.
- Define user roles, permissions, validation messages, and transaction status transitions.
