# Tech Stack & Business Projects

> **AI-Powered**: Deep AI integration across the full R&D lifecycle—from specification writing and code generation to troubleshooting. AI is embedded in every stage: requirements → design → development → testing.

## 1. Tech Stack

### 1.1 AI-Assisted Development
- **AI IDE**: Cursor (AI-native editor with code completion, conversational programming, multi-file understanding)
- **Code Assistants**: GitHub Copilot, Tongyi Lingma (code generation, comment completion, unit testing)
- **Spec-Driven**: Spec-DD specification documents → AI-generated code skeletons and implementations
- **Collaboration**: Feishu AI, intelligent document summarization, knowledge base Q&A

### 1.2 Database & Data Tools
- Plsql, MongoDB Compass, DMS NineData, DBeaver, RedisDesktopManager

### 1.3 Development Tools
- Cursor AI, IntelliJ IDEA, Eclipse, Visual Studio, VS Code
- Notepad++

### 1.4 API & Testing
- ApiFox, Postman, Fork

### 1.5 Remote & Ops
- SecureCRT, WinSCP, DAS-USM

### 1.6 Message Queue
- Offset Explorer (Kafka Tool)

### 1.7 Version Control
- GitLab, GitHub, SVN

### 1.8 Task Scheduling
- XXL-JOB

### 1.9 Integration Platform
- Definesys Cloud iPaaS Platform

### 1.10 Collaboration & Knowledge Base
- Feishu Project, Feishu Cloud Document Knowledge Base

### 1.11 CI/CD & Quality
- Jenkins, SonarQube

### 1.12 Monitoring & Observability
- Grafana, Prometheus, Guance Cloud, Kubernetes Rancher

### 1.13 Logging & Tracing
- OpenTelemetry (distributed tracing), ExceptionHandlerAspect (@AosException aspect), AosLog, MDC log correlation, Feishu exception notifications

### 1.14 ETL & Data Sync
- ETL DP, DataX

### 1.15 Messaging & Integration
- Kafka, AWS SQS, Spring Cloud Stream

### 1.16 Rules & Retry
- QLExpress (rule engine), Spring Retry (retry mechanism)

### 1.17 Testing & Quality
- JUnit 5, Mockito, AssertJ, JaCoCo (coverage)

---

## 2. Business Projects

| Project | Tech Stack | Period | Main Features |
|---------|------------|--------|---------------|
| Oracle EBS ERP | Oracle Stored Procedures | 2018–Present | Product, Planning, Procurement, QC, Stocking, Customs, Shipping, Inventory, Cost, Orders, RMA, Warehouse Split, Courier Split, Picking, Courier, Dispatch, Payables, Prepayments, General Ledger, Period Close, Invoicing, Reconciliation, Reporting |
| Order OMS | Liruan Agile Framework (.NET) | 2021–Present | Orders, RMA, Pan-European Sales, Warehouse Split, Courier Split |
| Supply Chain SCM | Kingdee Cloud Xinghan APAAS (Java Gradle) | 2021–2023 | Order Forecast, Shipping Plan, API Integration |
| Sales SOM | Kingdee Cloud Xinghan APAAS (Java Gradle) | 2021–2023 | Sales Forecast, Sales Quotation, API Integration |
| Marketing MMS | Kingdee Cloud Xinghan APAAS (Java Gradle) | 2021–2023 | Promotion, Workflow, API Integration |
| Finance FMS | Kingdee Cloud Xinghan APAAS (Java Gradle) | 2024–2025 | Reconciliation, API Integration |
| Warehouse WMS | Cainiao | 2025–2026 | API Integration |
| Logistics Tracking Platform PTC | Java SpringBoot Maven | 2025–Present | Integration of trackingmore, amazonshipping and other third-party courier APIs |
| Oracle EBS External API Platform | Java SpringBoot Maven | 2025–Present | EBS external interface platform |
| Complete Inventory Calculation Platform CIC | Java SpringBoot Maven | 2025–Present | WMS integration, box-level complete inventory calculation |
| Order Center OC | Java SpringBoot Maven | 2026–Present | Multi-platform store order download, waybill upload and other interfaces |
| Multi-Box Palletizing System PL | Python | 2025–2026 | Web, Mobile, PDA integration, pallet loading simulation |

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
