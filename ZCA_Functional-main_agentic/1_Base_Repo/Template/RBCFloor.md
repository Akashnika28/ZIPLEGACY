# RBC Floorplan Requirements Template

## Feature

**Feature name:** RBC Floorplan  
**Product / policy line:** [Enter applicable policy line]  
**User role:** Insurance product user

## User Story

As an insurance product user,  
I want to select and configure the RBC Floorplan option during policy setup,  
so that the policy reflects the required floorplan coverage and can be processed correctly.

## Requirements

**R1. Availability**  
The RBC Floorplan option must be available when the applicable policy line is selected.

**R2. Configuration**  
The user must be able to select RBC Floorplan and enter all required information.

**R3. Validation**  
The system must validate the RBC Floorplan selection and required information before the policy can proceed.

**R4. Policy Summary**  
The system must save the selected RBC Floorplan details and display them in the policy summary.

## Required Information

| Field | Required | Validation / Notes |
|---|---|---|
| Applicable policy line | Yes | [Enter allowed policy line] |
| RBC Floorplan selection | Yes | Must be a valid available option |
| Floorplan details | Yes | [Enter required fields and formats] |

## Acceptance Criteria

1. Given the applicable policy line is selected, when the user opens the coverage options, then RBC Floorplan is available.
2. Given RBC Floorplan is selected, when the user enters the required information, then the system accepts and saves the details.
3. Given required information is missing or invalid, when the user tries to proceed, then the system displays validation errors and blocks progression.
4. Given valid RBC Floorplan details are saved, when the user views the policy summary, then the selected details are displayed accurately.

## Open Items

- Applicable policy line: [TBD]
- Required floorplan fields: [TBD]
- Validation messages and rules: [TBD]
- Policy summary display location: [TBD]
