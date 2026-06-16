# Tech Stack & Business Projects

> **AI-Powered**: Deep AI integration across the full R&D lifecycle—from specification writing and code generation to troubleshooting. AI is embedded in every stage: requirements → design → development → testing.

## 1. Business Projects

| Tech Stack | Project | Period | Main Features |
|------------|---------|--------|---------------|
| Oracle Stored Procedures | Oracle EBS ERP | 2018–Present | Product, Planning, Procurement, QC, Stocking, Customs, Shipping, Inventory, Cost, Orders, RMA, Warehouse Split, Courier Split, Picking, Courier, Dispatch, Payables, Prepayments, General Ledger, Period Close, Invoicing, Reconciliation, Reporting |
| Liruan Agile Framework (.NET) | Order OMS | 2021–Present | Orders, RMA, Pan-European Sales, Warehouse Split, Courier Split, Consignment & Distribution |
| Kingdee Cloud Xinghan APAAS (Java Gradle) | Supply Chain SCM | 2021–2023 | Order Forecast, Shipping Plan, API Integration |
| Kingdee Cloud Xinghan APAAS (Java Gradle) | Sales SOM | 2021–2023 | Sales Forecast, Sales Quotation, API Integration |
| Kingdee Cloud Xinghan APAAS (Java Gradle) | Marketing MMS | 2021–2023 | Amazon SP/ST auto-bidding & budget, report upload, workflow, API integration |
| Kingdee Cloud Xinghan APAAS (Java Gradle) | Finance FMS | 2024–2025 | Reconciliation, API Integration |
| Cainiao | Warehouse WMS | 2025–2026 | API Integration |
| Java SpringBoot Maven | Logistics Tracking Platform PTC | 2025–Present | Integration of trackingmore, amazonshipping and other third-party courier APIs |
| Java SpringBoot Maven | Oracle EBS External API Platform | 2025–Present | EBS external interface platform |
| Java SpringBoot Maven | Complete Inventory Calculation Platform CIC | 2025–Present | WMS integration, box-level complete inventory calculation |
| Java SpringBoot Maven | Order Center OC | 2026–Present | Multi-platform store order download, waybill upload, product update APIs, SQS notifications, observability (@AosException, MDC, Feishu exception alerts) |
| Python | Multi-Box Palletizing System PL | 2025–2026 | Web, Mobile, PDA integration, pallet loading simulation |
| Aozhe CloudPivot 8.6 (Java Maven) | Aozhe CloudPivot APAAS POC | 2026–2026 | Tenant extension, user extension, launcher/user service extension, frontend modules |
| Shushi Oinone 6.4.5 (Java Maven) | Aozhe CloudPivot APAAS POC | 2026–2026 | Tenant extension, user extension, model, AI Agent, frontend modules |
| Defan 5.0 (Java Maven) | Defan APAAS POC | 2026–2026 | Tenant extension, user extension, model, AI Agent, frontend modules |
| Java SpringBoot Maven | Order Center Frontend oc-web | 2026–2026 | Multi-theme, multi-store order query, API services, account management |
| Java SpringBoot Maven | Inventory Center IC | 2026–2026 | Mongo inventory snapshot/transaction/reservation/combined SKU, XXL-Job Feishu heartbeat |
| Cursor Agent / PowerShell | Shared Skills Submodule Repo | 2026–2026 | `.cursor` triple Submodule, skill Hook Feishu ledger, InnoSetup installer |
| Cursor Agent / Feishu MCP · Apifox CLI | Feishu Project Apifox API Spec Workflow | 2026–2026 | Requirements lock → OpenAPI → Apifox import → CLI smoke test four-step skill pack (WMS loading order practice) |
| Cursor Agent / Feishu CLI | AI Collaboration Infrastructure | 2026–2026 | Daily report skill pack, Spec-DD doc standards, Feishu Project six-step delivery workflow, Git branch/commit conventions |

---

## 2. Tech Stack

### 2.1 AI-Assisted Development
- **AI IDE**: Cursor (AI-native editor with code completion, conversational programming, multi-file understanding)
- **Agent Skills**: Standalone skill packs (`SKILL.md` + `assets/` + `scripts/`), copyable as a whole folder; `.cursor` triple leaf **Git Submodule** for distributing shared skills
- **Cursor Hooks**: `beforeSubmitPrompt` skill usage telemetry → PowerShell → **lark-cli** writes to Feishu "Skill Usage Count" ledger
- **Feishu Project MCP**: Work item locking, `search_by_mql`, `add_comment` write-back (API spec / Apifox / smoke report chain)
- **lark-cli**: Bitable read/write, calendar `+agenda`, IM `+messages-search`, Wiki doc ingestion (user-scoped `identity=user`)
- **Code Assistants**: GitHub Copilot, Tongyi Lingma (code generation, comment completion, unit testing)
- **Spec-Driven**: Spec-DD specification documents → AI-generated code skeletons and implementations; OpenAPI pre-import checklist gate
- **Apifox CLI**: Private deployment `--api-base-url`, `test-suite run`, `--upload-report` smoke tests and report write-back
- **Collaboration**: Feishu AI, intelligent document summarization, knowledge base Q&A; daily report multi-source collection (Feishu closed items + Git + calendar + IM)

### 2.2 Database & Data Tools
- Plsql, MongoDB Compass, DMS NineData, DBeaver, RedisDesktopManager

### 2.3 Development Tools
- Cursor AI, IntelliJ IDEA, Eclipse, Visual Studio, VS Code
- **PowerShell**: Hook scripts, skill pack `Import.ps1` / ledger writes, InnoSetup compile helper
- **InnoSetup**: Cursor skill pack / Submodule one-click installer (`Aosom-Skills`)
- Notepad++

### 2.4 API & Testing
- **Apifox** (Web + **CLI**): OpenAPI `import-data` HTTP import, test suite smoke runs, private deployment base URL
- Postman, Fork
- **OpenAPI 3**: Spec-driven API contracts; `x-apifox-folder` folder alignment; Feishu `work_item_id` end-to-end traceability extension fields

### 2.5 Remote & Ops
- SecureCRT, WinSCP, DAS-USM

### 2.6 Message Queue
- Offset Explorer (Kafka Tool)

### 2.7 Version Control
- GitLab, GitHub, SVN
- **Git Submodule**: `kit-skills` triple leaf (rules / commands / shared skills); English **kebab-case** branch names (stable for internal push)

### 2.8 Task Scheduling
- XXL-JOB

### 2.9 Integration Platform
- Definesys Cloud iPaaS Platform

### 2.10 Collaboration & Knowledge Base
- **Feishu Project** (Meego / IT-Project MCP), Feishu Cloud Documents / Wiki knowledge base
- **Feishu Bitable (Base)**: IT daily reports, shared Skills management ledger, skill usage counts, Apifox API release records

### 2.11 CI/CD & Quality
- Jenkins, SonarQube

### 2.12 Monitoring & Observability
- Grafana, Prometheus, Guance Cloud, Kubernetes Rancher

### 2.13 Logging & Tracing
- OpenTelemetry (distributed tracing), ExceptionHandlerAspect (@AosException aspect), AosLog, MDC log correlation, Feishu exception notifications

### 2.14 ETL & Data Sync
- ETL DP, DataX

### 2.15 Messaging & Integration
- Kafka, AWS SQS, Spring Cloud Stream

### 2.16 Rules & Retry
- QLExpress (rule engine), Spring Retry (retry mechanism)

### 2.17 Testing & Quality
- JUnit 5, Mockito, AssertJ, JaCoCo (coverage)

### 2.18 Frontend & Web (2026 · oc-web)
- **Spring Boot + FreeMarker**: Server-side rendering, macro-based list page components
- **Spring Security**: Login/logout transitions, role-based menus (Admin / Sales / Support)
- **Multi-Theme UI**: Multiple frontend style switching; preference-based i18n and timezone (`localStorage` + `oc-web-ui.json`)
- **Pluggable Table Pattern**: Multi-store order query adapters, API services `/ledger` HTTP probing, four Mongo read-only inventory list types

---

## 3. R&D Capabilities

Based on tech stack and business project experience, R&D capabilities are summarized as follows:

### 3.1 AI Empowerment
- **Spec→Code**: Spec-DD document-driven development; AI generates complete Controller/Service/Dao implementations from specs
- **Conversational Programming**: Cursor multi-file understanding, context-aware code completion and refactoring
- **Troubleshooting**: AI-assisted log analysis, root cause analysis, Feishu notification context interpretation
- **Knowledge Retention**: Feishu Cloud Documents + AI summarization; specs and functional docs are AI-searchable and referenceable
- **Feishu MCP**: Feishu Project requirements/task context integrated into Cursor Agent; supports requirements locking and collaboration ledger sync
- **Apifox CLI**: Requirements lock → OpenAPI generation → Apifox import → CLI smoke test four-step skill pack (API spec closed loop)
- **Feishu CLI**: Daily report, Spec-DD doc standards, Feishu Project six-step delivery workflow, Git branch/commit conventions, and other AI collaboration skill packs
- **Agent Skills Infrastructure**: `.cursor` Submodule skill repo, Hook Feishu ledger, PowerShell/InnoSetup installer distribution

### 3.2 Tech Stack Breadth
- **Multi-Language**: Java (SpringBoot), .NET, Python, Oracle PL/SQL
- **Full-Stack Toolchain**: Database (Oracle, MongoDB, Redis), API testing, CI/CD, monitoring, ETL covering the full R&D lifecycle
- **Cloud-Native**: Kubernetes, Rancher for container orchestration and ops

### 3.3 Business Domain Depth
- **End-to-End Supply Chain**: From ERP (product, procurement, inventory, cost) to Order OMS, Supply Chain SCM, Sales SOM, Marketing MMS, Finance FMS, Warehouse WMS
- **Logistics & Fulfillment**: Logistics tracking platform, courier API integration, warehouse/courier split, picking and dispatch
- **E-Commerce & Orders**: Multi-platform store orders (Amazon IE, Trendyol RO, Syncee FR, etc.), waybill upload, SQS order notifications, RMA, Pan-European sales
- **Order Center Operations**: oc-web order query / API service probing / account & inventory management; microservice ledger aligned with K8s Ingress
- **Inventory Domain (oc-inv)**: Mongo snapshot ledger (parallel by country, Feishu Job heartbeat), transaction/reservation/combined SKU sync and CIC/EBS contracts

### 3.4 System Integration
- **API Integration**: EBS external interface platform, business system APIs, third-party courier APIs (trackingmore, amazonshipping)
- **OpenAPI Contract Closed Loop**: Feishu requirements lock → 【Spec】+ OpenAPI → Apifox import → CLI smoke → MCP comment write-back (WMS loading order and other practices)
- **EBS Packages/Stored Procedures**: `insert_order_iface`, platform product sync, loading order/WMS performance and field iterations
- **Platformization**: Definesys Cloud iPaaS, Order Center OC, Complete Inventory Calculation Platform CIC
- **Data Sync**: ETL DP, DataX for data integration and migration
- **Cross-Platform Integration**: Amazon SP-API (refresh token, confirmShipment), AWS S3/KMS/SQS, Oracle EBS SOAP

### 3.5 Engineering Capabilities
- **Quality Assurance**: Jenkins, SonarQube for continuous integration and code quality
- **Observability**: Grafana, Prometheus, Guance Cloud for monitoring and alerting
- **Task Scheduling**: XXL-JOB for scheduled and distributed job scheduling; long-running Job **Feishu heartbeat** (snapshot ledger country k/N progress)
- **Logging & Tracing**: OpenTelemetry + AOP-based tracing; MDC injection of traceId/spanId for log correlation; Slf4j structured logging; automatic Feishu exception notifications (nested call deduplication, connection reset silencing)
- **Agent Skill Governance**: Hook four-step onboarding (install → local config → lark-cli auth → trial write); scan registration + usage count formula aggregation
- **Multi-Datasource**: dynamic-datasource for MySQL, Oracle, MongoDB dynamic switching
- **Retry & Resilience**: Spring Retry, message idempotency design
- **Modular Architecture**: common module + business module layered reuse; `application-shared-*.yml` slim skeleton + per-service overrides
- **Microservice Layering**: Controller (API entry) → Service (business logic) → Dao/Repository (data access); Job scheduled tasks; Mapper external interfaces; common abstract interfaces for business module implementation

### 3.6 Standards & Delivery
- **Spec-Driven**: Spec-DD specification-driven development; documentation first (spec → code → test); 【Type】Chinese doc naming and `.docs/` single source
- **Feishu Six-Step Delivery**: Lock task → 【Feature】design + `add_comment` → development → verification → doc retention → Git branch & commit (step-by-step manual confirmation)
- **Daily Reports & Timesheets**: Feishu CLI multi-source read-only collection + preview before final write to Base; empty "major item" row reuse, 0.5h increments and daily cap
- **Version & Collaboration**: GitLab/GitHub, Submodule collaboration (business repo commit Hook, source repo local install); Feishu Project, Feishu Cloud Document knowledge base

### 3.7 Testing & Quality
- **Unit Testing**: JUnit 5, Mockito, AssertJ, JaCoCo coverage
- **API Smoke Tests**: Apifox CLI test suites + report upload; OpenAPI pre-import checklist mandatory gate
- **Multi-Environment Config**: Spring Profiles switching, `application-ledger-{dev,test,prod}.yml` probe matrix, externalized config, feature flags

### 3.8 Security & Authentication
- **OAuth 2.0**: Amazon SP-API refresh token flow
- **Cloud Credentials**: AWS IAM roles, environment variables, config files
- **Token Management**: Auto-refresh, caching, RestrictedDataToken
