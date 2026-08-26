# CDSPI Historical COC and CGL User Story

## User Story

As an insurance product user,  
I want to capture and validate historical Certificate of Completion (COC) information while configuring CDSPI Commercial General Liability (CGL) coverage,  
so that the system can accurately assess the risk, apply underwriting rules, calculate the premium, and generate the correct policy documentation.

## Requirements

1. The CDSPI COC and CGL options are available for eligible applicants, jurisdictions, and transaction types.
2. The user can capture historical COC details, including completion date, project or risk description, applicable limits, and required supporting documentation.
3. The system validates required COC fields, dates, limits, and document requirements before the policy can proceed.
4. The user can capture the required applicant, business, operations, location, exposure, and claims information for CGL underwriting.
5. The user can select permitted CGL coverages, limits, deductibles, extensions, exclusions, and endorsements.
6. The system applies eligibility and underwriting rules and creates a referral or decline outcome when configured conditions are met.
7. The system calculates and displays the CGL premium, applicable charges, and total premium using configured rating factors.
8. The system attaches and generates the required COC and CGL forms, endorsements, disclosures, and supporting documents.
9. The user can save, quote, bind, and issue the policy after validations, referrals, and approvals are complete.
10. The system retains COC values, CGL selections, rating inputs, referrals, approvals, document versions, and relevant changes for audit purposes.

## Acceptance Criteria

### AC1: Product Availability

Given an eligible applicant, jurisdiction, and transaction type,  
when the user starts the CDSPI COC and CGL transaction,  
then the applicable product options are available.

### AC2: Historical COC Information

Given the COC section is available,  
when the user enters valid historical COC information,  
then the system accepts and saves the information.

### AC3: COC Validation

Given required COC information or supporting documentation is missing or invalid,  
when the user attempts to continue,  
then the system displays field-level validation messages and blocks progression.

### AC4: CGL Coverage Selection

Given valid CGL risk information,  
when the user selects permitted coverages, limits, deductibles, extensions, or endorsements,  
then the system accepts the selections and applies the configured rules.

### AC5: Rating and Quote

Given valid COC, CGL, and exposure information,  
when the user requests a quote,  
then the system calculates and displays the correct premium and applicable charges.

### AC6: Underwriting Referral or Decline

Given the historical COC or CGL risk meets a configured referral or decline condition,  
when the user attempts to quote or bind,  
then the system creates the appropriate outcome and prevents completion until the required action is resolved.

### AC7: Forms and Documents

Given the selected coverage and transaction are eligible for documents,  
when the policy is quoted or issued,  
then the required COC and CGL documents are attached with the correct version and effective date.

### AC8: Policy Completion

Given all validations and approvals are complete,  
when the user binds and issues the policy,  
then the policy status, historical COC information, and CGL selections are saved correctly.

### AC9: Audit History

Given a saved transaction,  
when an authorized user reviews the history,  
then the COC values, CGL changes, referrals, approvals, rating inputs, and documents are available for audit.

## Open Items

- Eligible CDSPI applicants, operations, jurisdictions, and transaction types: [TBD]
- COC historical period, completion-date, and expiry rules: [TBD]
- Required COC fields and supporting documents: [TBD]
- Available CGL coverages, limits, deductibles, extensions, and endorsements: [TBD]
- Exposure and premium rating factors: [TBD]
- Referral, decline, and approval conditions: [TBD]
- Required forms, document editions, and effective dates: [TBD]
- Validation messages and policy status transitions: [TBD]
