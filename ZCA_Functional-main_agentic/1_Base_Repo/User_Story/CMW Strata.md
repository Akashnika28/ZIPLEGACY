# CMW Strata User Story

## User Story

As an insurance product user,  
I want to quote and manage CMW Strata coverage using the configured product and underwriting rules,  
so that the strata risk receives accurate protection, pricing, documentation, and policy processing.

## Requirements

1. The CMW Strata product is available for eligible strata risks, jurisdictions, building types, and transaction types.
2. The user can capture strata corporation, building, unit, and common-property information required for underwriting.
3. The user can capture property values, replacement cost, unit and common-area exposures, amenities, parking, utilities, and loss-prevention details.
4. The user can select permitted property, liability, equipment breakdown, directors and officers, and other optional coverages, limits, deductibles, exclusions, and endorsements.
5. The system applies configured eligibility and underwriting rules and creates a referral or decline outcome when required.
6. The system calculates and displays the premium, applicable charges, and total premium using configured risk and exposure factors.
7. The system displays clear validation errors for missing, invalid, or inconsistent strata and building information.
8. The system attaches and generates the required CMW Strata forms, schedules, endorsements, disclosures, and supporting documents.
9. The user can save, quote, bind, and issue the policy after all validations, referrals, and approvals are complete.
10. The system retains strata details, building exposures, coverage selections, rating inputs, referrals, approvals, document versions, and relevant changes for audit purposes.

## Acceptance Criteria

### AC1: Product Availability

Given an eligible strata risk, jurisdiction, building type, and transaction type,  
when the user starts a CMW Strata transaction,  
then the product is available.

### AC2: Strata and Building Information

Given the product is available,  
when the user enters valid strata corporation, building, unit, and common-property information,  
then the system accepts and saves the information.

### AC3: Validation

Given required or inconsistent strata information is missing or invalid,  
when the user attempts to continue,  
then the system displays field-level validation messages and blocks progression.

### AC4: Coverage Configuration

Given valid exposure information,  
when the user selects permitted strata coverages, limits, deductibles, exclusions, or endorsements,  
then the system accepts the selections and applies the configured rules.

### AC5: Rating and Quote

Given valid building, exposure, and coverage information,  
when the user requests a quote,  
then the system calculates and displays the correct premium and applicable charges.

### AC6: Underwriting Referral or Decline

Given the strata risk meets a configured referral or decline condition,  
when the user attempts to quote or bind,  
then the system creates the appropriate outcome and prevents completion until the required action is resolved.

### AC7: Forms and Documents

Given the selected coverage and transaction are eligible for documents,  
when the policy is quoted or issued,  
then the required CMW Strata forms and documents are attached with the correct version and effective date.

### AC8: Policy Completion

Given all validations and approvals are complete,  
when the user binds and issues the policy,  
then the policy status, strata details, building exposures, and coverage selections are saved correctly.

### AC9: Audit History

Given a saved transaction,  
when an authorized user reviews the history,  
then the relevant changes, rating inputs, referrals, approvals, and documents are available for audit.

## Open Items

- Eligible strata risks, building types, operations, jurisdictions, and transaction types: [TBD]
- Required and conditional building, unit, common-property, amenities, and exposure fields: [TBD]
- Replacement-cost and valuation rules: [TBD]
- Available property, liability, equipment, and optional coverages: [TBD]
- Coverage limits, deductibles, exclusions, and endorsements: [TBD]
- Referral, decline, and manual underwriting conditions: [TBD]
- Rating factors and premium calculations: [TBD]
- Required forms, document editions, and effective dates: [TBD]
- Validation messages and policy status transitions: [TBD]
