# Example: User Management Feature

## Request

新增使用者管理功能。

功能包含：

- 使用者清單
- 新增使用者
- 編輯使用者
- 停用使用者
- 角色設定

## Workflow

```text
PM -> SA -> Frontend RD + Backend RD -> QA
```

## PM Clarifies

- 使用者角色
- 新增、編輯、停用權限
- 是否需要審核
- 是否需要 audit log
- 停用後是否可恢復
- Email 是否唯一

## SA Designs

- API contract
- User data model
- Role model
- Main flow
- Error handling
- Frontend pages
- Backend boundaries

## Frontend RD Handles

- Detect current UI style
- User list page
- User form
- Role selector
- UI states
- API integration

## Backend RD Handles

- Spring Boot API
- User domain model
- Role model
- Validation
- Transaction boundary
- Error handling
- Audit log
- Tests

## QA Validates

- CRUD flow
- Permission control
- Duplicate email
- Disabled user behavior
- Error messages
- Audit log
- Regression risk
