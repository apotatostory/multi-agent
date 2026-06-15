# Prompt Examples

## Full-stack Feature

```text
請依照 AGENTS.md 的 multi-agent workflow 執行。

任務：
新增使用者管理功能。

請讓：
1. PM 先釐清需求
2. SA 規劃 SD，並拆分前後端任務
3. rd-frontend-react 實作 React UI
4. rd-backend-java 實作 Spring Boot API
5. qa 驗收

注意：
- 前端 RD 要自行判斷既有設計風格
- 後端 RD 要用 OOP 與適合的 design pattern 寫出乾淨 code
- PM 不清楚需求時要先停下來釐清
```

## Backend-only Feature

```text
請依照 AGENTS.md 執行。

任務：
新增訂單狀態流轉 API。

請讓：
1. PM 釐清狀態規則與驗收條件
2. SA 設計狀態機、API、DB、錯誤處理
3. rd-backend-java 實作 Spring Boot API
4. qa 驗收
```

## Frontend-only Feature

```text
請依照 AGENTS.md 執行。

任務：
新增設備清單查詢頁面。

請讓：
1. PM 釐清查詢條件、欄位、操作流程
2. SA 規劃前端頁面行為與 API dependency
3. rd-frontend-react 判斷現有 UI 風格後實作
4. qa 驗收
```
