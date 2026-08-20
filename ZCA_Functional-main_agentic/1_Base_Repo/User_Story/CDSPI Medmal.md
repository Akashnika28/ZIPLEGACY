# CDSPI Medical Malpractice User Story

## User Story

As an insurance product user,  
I want to quote and manage CDSPI Medical Malpractice coverage using the configured product rules,  
so that eligible risks receive accurate coverage, pricing, documentation, and policy processing.

## Requirements

1. The CDSPI Medical Malpractice product is available for eligible users, jurisdictions, and transactions.
2. The user can enter the required applicant, practitioner, practice, and risk information.
3. The system validates eligibility and underwriting rules before the policy can proceed.
4. The user can select permitted coverage limits, deductibles, endorsements, and optional protections.
5. The system calculates and displays the premium and applicable charges using configured rating rules.
6. The system displays clear validation errors and creates an underwriting referral when configured conditions are met.
7. The system attaches the required CDSPI forms and documents with the correct version and effective date.
8. The user can save, quote, bind, and issue the policy after all validations and approvals are complete.
9. The system retains coverage selections, rating inputs, referrals, approvals, documents, and relevant changes for audit purposes.

## Acceptance Criteria

### AC1: Product Availability

Given an eligible applicant and jurisdiction,  
when the user starts a CDSPI Medical Malpractice transaction,  
then the product is available for selection.

### AC2: Applicant and Risk Information

Given the product is available,  
when the user enters valid required applicant and risk information,  
then the system accepts and saves the information.

### AC3: Validation of Required Information

Given required information is missing or invalid,  
when the user attempts to continue,  
then the system displays field-level validation messages and blocks progression.

### AC4: Coverage Selection

Given valid risk information,  
when the user selects an allowed coverage limit and deductible,  
then the system accepts the selection and applies the configured product rules.

### AC5: Rating and Quote

Given valid rating inputs,  
when the user requests a quote,  
then the system calculates and displays the correct premium and applicable charges.

### AC6: Underwriting Referral

Given the risk meets an underwriting referral condition,  
when the user attempts to quote or bind,  
then the system creates the configured referral and prevents completion until it is resolved.

### AC7: Forms and Documents

Given the selected coverage and transaction are eligible for documents,  
when the policy is quoted or issued,  
then the required CDSPI forms and documents are attached with the correct version and effective date.

### AC8: Policy Completion

Given all validations and approvals are complete,  
when the user completes the policy transaction,  
then the policy status and selected coverage details are saved correctly.

### AC9: Audit History

Given a saved transaction,  
when an authorized user reviews its history,  
then the relevant inputs, changes, referrals, approvals, and documents are available for audit.

## Open Items

- Eligible practitioners, specialties, and jurisdictions: [TBD]
- Available coverage limits, deductibles, and endorsements: [TBD]
- Required and conditional fields: [TBD]
- Rating factors and premium rules: [TBD]
- Referral, decline, and manual underwriting conditions: [TBD]
- Required forms, document editions, and effective dates: [TBD]
