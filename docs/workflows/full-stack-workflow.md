# Full-Stack Multi-Agent Workflow

## Flow

```text
User Request
   ↓
PM Clarification
   ↓
SA System Design
   ↓
Frontend RD + Backend RD
   ↓
QA Validation
   ↓
Final Delivery
```

## Step 1: PM Clarification

PM must clarify:

- Goal
- Users
- Flow
- MVP scope
- Out of scope
- Acceptance criteria
- Priority
- Risks

If requirement is unclear, PM should stop and mark:

```text
Ready for SA = No
```

## Step 2: SA System Design

SA converts PM brief into SD.

SA must produce:

- Frontend design
- Backend design
- API contract
- Data model
- Main flow
- Error handling
- Permission model
- RD task breakdown

If design is not ready, SA should mark:

```text
Ready for RD = No
```

## Step 3: RD Implementation

Frontend RD handles React only.

Backend RD handles Java / Spring Boot only.

Both must follow SA design.

## Step 4: QA Validation

QA checks:

- Requirement coverage
- Design coverage
- Frontend behavior
- Backend behavior
- API consistency
- Edge cases
- Regression risk
- Security / permission risk

## Step 5: Final Delivery

Final report must include:

- PM result
- SA result
- Frontend RD result
- Backend RD result
- QA result
- Risks
- Next actions
