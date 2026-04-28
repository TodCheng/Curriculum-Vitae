# Tech Stack & Business Projects

> **AI-Powered**: Deep AI integration across the full R&D lifecycle—from specification writing and code generation to troubleshooting. AI is embedded in every stage: requirements → design → development → testing.

## 1. Business Projects

| Tech Stack | Project | Period | Main Features |
|------------|---------|--------|---------------|
| Oracle Stored Procedures | Oracle EBS ERP | 2018–Present | Product, Planning, Procurement, QC, Stocking, Customs, Shipping, Inventory, Cost, Orders, RMA, Warehouse Split, Courier Split, Picking, Courier, Dispatch, Payables, Prepayments, General Ledger, Period Close, Invoicing, Reconciliation, Reporting |
| Liruan Agile Framework (.NET) | Order OMS | 2021–Present | Orders, RMA, Pan-European Sales, Warehouse Split, Courier Split |
| Kingdee Cloud Xinghan APAAS (Java Gradle) | Supply Chain SCM | 2021–2023 | Order Forecast, Shipping Plan, API Integration |
| Kingdee Cloud Xinghan APAAS (Java Gradle) | Sales SOM | 2021–2023 | Sales Forecast, Sales Quotation, API Integration |
| Kingdee Cloud Xinghan APAAS (Java Gradle) | Marketing MMS | 2021–2023 | Promotion, Workflow, API Integration |
| Kingdee Cloud Xinghan APAAS (Java Gradle) | Finance FMS | 2024–2025 | Reconciliation, API Integration |
| Cainiao | Warehouse WMS | 2025–2026 | API Integration |
| Java SpringBoot Maven | Logistics Tracking Platform PTC | 2025–Present | Integration of trackingmore, amazonshipping and other third-party courier APIs |
| Java SpringBoot Maven | Oracle EBS External API Platform | 2025–Present | EBS external interface platform |
| Java SpringBoot Maven | Complete Inventory Calculation Platform CIC | 2025–Present | WMS integration, box-level complete inventory calculation |
| Java SpringBoot Maven | Order Center OC | 2026–Present | Multi-platform store order download, waybill upload and other interfaces |
| Python | Multi-Box Palletizing System PL | 2025–2026 | Web, Mobile, PDA integration, pallet loading simulation |
| Aozhe CloudPivot 8.6 (Java Maven) | Aozhe CloudPivot APAAS POC | 2026–Present | Tenant extension, user extension, launcher/user service extension, frontend modules |
| Shushi Oinone 6.4.5 (Java Maven) | Aozhe CloudPivot APAAS POC | 2026–Present | Tenant extension, user extension, model, AI Agent, frontend modules |
| Defan 5.0 (Java Maven) | Defan APAAS POC | 2026–Present | Tenant extension, user extension, model, AI Agent, frontend modules |

---

## 2. Tech Stack

### 2.1 AI-Assisted Development
- **AI IDE**: Cursor (AI-native editor with code completion, conversational programming, multi-file understanding)
- **Code Assistants**: GitHub Copilot, Tongyi Lingma (code generation, comment completion, unit testing)
- **Spec-Driven**: Spec-DD specification documents → AI-generated code skeletons and implementations
- **Collaboration**: Feishu AI, intelligent document summarization, knowledge base Q&A

### 2.2 Database & Data Tools
- Plsql, MongoDB Compass, DMS NineData, DBeaver, RedisDesktopManager

### 2.3 Development Tools
- Cursor AI, IntelliJ IDEA, Eclipse, Visual Studio, VS Code
- Notepad++

### 2.4 API & Testing
- ApiFox, Postman, Fork

### 2.5 Remote & Ops
- SecureCRT, WinSCP, DAS-USM

### 2.6 Message Queue
- Offset Explorer (Kafka Tool)

### 2.7 Version Control
- GitLab, GitHub, SVN

### 2.8 Task Scheduling
- XXL-JOB

### 2.9 Integration Platform
- Definesys Cloud iPaaS Platform

### 2.10 Collaboration & Knowledge Base
- Feishu Project, Feishu Cloud Document Knowledge Base

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

---

## 3. R&D Capabilities

Based on tech stack and business project experience, R&D capabilities are summarized as follows:

### 3.1 AI Empowerment
- **Spec→Code**: Spec-DD document-driven development; AI generates complete Controller/Service/Dao implementations from specs
- **Conversational Programming**: Cursor multi-file understanding, context-aware code completion and refactoring
- **Troubleshooting**: AI-assisted log analysis, root cause analysis, Feishu notification context interpretation
- **Knowledge Retention**: Feishu Cloud Documents + AI summarization; specs and functional docs are AI-searchable and referenceable

### 3.2 Tech Stack Breadth
- **Multi-Language**: Java (SpringBoot), .NET, Python, Oracle PL/SQL
- **Full-Stack Toolchain**: Database (Oracle, MongoDB, Redis), API testing, CI/CD, monitoring, ETL covering the full R&D lifecycle
- **Cloud-Native**: Kubernetes, Rancher for container orchestration and ops

### 3.3 Business Domain Depth
- **End-to-End Supply Chain**: From ERP (product, procurement, inventory, cost) to Order OMS, Supply Chain SCM, Sales SOM, Marketing MMS, Finance FMS, Warehouse WMS
- **Logistics & Fulfillment**: Logistics tracking platform, courier API integration, warehouse/courier split, picking and dispatch
- **E-Commerce & Orders**: Multi-platform store orders, waybill upload, RMA, Pan-European sales

### 3.4 System Integration
- **API Integration**: EBS external interface platform, business system APIs, third-party courier APIs (trackingmore, amazonshipping)
- **Platformization**: Definesys Cloud iPaaS, Order Center OC, Complete Inventory Calculation Platform CIC
- **Data Sync**: ETL DP, DataX for data integration and migration
- **Cross-Platform Integration**: Amazon SP-API, AWS S3/KMS/SQS, Oracle EBS SOAP

### 3.5 Engineering Capabilities
- **Quality Assurance**: Jenkins, SonarQube for continuous integration and code quality
- **Observability**: Grafana, Prometheus, Guance Cloud for monitoring and alerting
- **Task Scheduling**: XXL-JOB for scheduled and distributed job scheduling
- **Logging & Tracing**: OpenTelemetry + AOP-based tracing; MDC injection of traceId/spanId for log correlation; Slf4j structured logging; automatic Feishu exception notifications (nested call deduplication, connection reset silencing)
- **Multi-Datasource**: dynamic-datasource for MySQL, Oracle, MongoDB dynamic switching
- **Retry & Resilience**: Spring Retry, message idempotency design
- **Modular Architecture**: common module + business module layered reuse
- **Microservice Layering**: Controller (API entry) → Service (business logic) → Dao/Repository (data access); Job scheduled tasks; Mapper external interfaces; common abstract interfaces for business module implementation

### 3.6 Standards & Delivery
- **Spec-Driven**: Spec-DD specification-driven development; documentation first (spec → code → test)
- **Version & Collaboration**: GitLab/GitHub, Feishu Project, Feishu Cloud Document Knowledge Base

### 3.7 Testing & Quality
- **Unit Testing**: JUnit 5, Mockito, AssertJ, JaCoCo coverage
- **Multi-Environment Config**: Spring Profiles switching, externalized config, feature flags

### 3.8 Security & Authentication
- **OAuth 2.0**: Amazon SP-API refresh token flow
- **Cloud Credentials**: AWS IAM roles, environment variables, config files
- **Token Management**: Auto-refresh, caching, RestrictedDataToken
