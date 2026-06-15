# Multi-Agent Delivery Team

這個 repo 定義一套可用於 Codex CLI / Codex App 的精簡 Multi-Agent Software Delivery Workflow。

這版團隊刻意不要切太細，先用最實用的角色：

```text
User Request
   ↓
PM Agent
   ↓
SA Agent
   ↓
RD Pool
   ├─ Frontend RD：React 專家，自行判斷專案 UI 設計風格
   └─ Backend RD：資深 Java / Spring Boot 工程師，重視 OOP 與 Design Pattern
   ↓
QA Agent
   ↓
Final Delivery
```

## 角色定位

### PM Agent

PM 是需求守門員。

特色：

- 會先釐清需求
- 會確認目標、範圍、角色、流程、驗收條件
- 需求不清楚時，不會急著派工
- 等一切明確後，才會安排 SA 分析與 RD 實作

### SA Agent

SA 是系統分析與設計者。

特色：

- 根據 PM 的需求拆解任務
- 規劃 SD，也就是系統設計文件
- 定義 API、資料模型、流程、模組責任、錯誤處理
- 把任務切給 Frontend RD 與 Backend RD

### Frontend RD Agent

Frontend RD 是 React 專家。

特色：

- 專門寫 React 前端
- 會自行判斷專案使用的設計風格，例如 Material UI、Ant Design、Tailwind、Bootstrap、自研 Design System
- 不會硬套風格，會先觀察既有專案結構
- 負責 UI component、頁面、表單、狀態管理、API 串接

### Backend RD Agent

Backend RD 是資深 Java / Spring Boot 工程師。

特色：

- 專門寫 Java 後端
- 主要使用 Spring Boot
- 設計風格偏 OOP
- 喜歡用 Design Pattern 寫出乾淨、可維護、優雅的 code
- 重視分層、封裝、可測試性、交易一致性與錯誤處理

### QA Agent

QA 是交付守門員。

特色：

- 檢查需求是否被滿足
- 檢查 SA 設計是否完整
- 檢查 RD 實作是否符合設計
- 產生測試案例、edge case、regression risk
- 最後給出 PASS / FAIL / CONDITIONAL PASS

## 使用方式

在 repo root 執行：

```bash
codex
```

然後輸入：

```text
請依照 AGENTS.md 的 multi-agent workflow 執行任務。

任務：
新增使用者管理功能，包含前端 React 頁面與後端 Spring Boot API。

請依序讓：
1. PM 先釐清需求
2. SA 根據 PM 結果規劃 SD 與拆分任務
3. Frontend RD 實作 React UI
4. Backend RD 實作 Spring Boot API
5. QA 驗收

最後輸出 Final Delivery Report。
```

## 目錄

```text
.
├─ AGENTS.md
├─ .codex/agents/
│  ├─ pm.toml
│  ├─ sa.toml
│  ├─ rd-frontend-react.toml
│  ├─ rd-backend-java.toml
│  └─ qa.toml
├─ docs/
│  ├─ templates/
│  └─ workflows/
└─ examples/
```
