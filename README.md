# 技术栈与业务项目

> **AI 赋能**：研发全流程深度集成 AI，从规范编写、代码生成到问题排查，AI 贯穿需求→设计→开发→测试各环节。

## 1. 业务项目

| 技术栈 | 项目 | 周期 | 主要功能 |
|--------|------|------|----------|
| Oracle 存储过程 | Oracle EBS ERP | 2018-至今 | 产品、计划、采购、质检、备货、报关、出运、库存、成本、订单、RMA、分仓、分快递、拣货、快递、派遣、应付、预付、总账、期间、开票、对账、报表 |
| 力软敏捷开发框架（.NET） | 订单 OMS | 2021-至今 | 订单、RMA、泛欧销售、分仓、分快递、代卖经销 |
| 金蝶云星瀚 APAAS（Java Gradle） | 供应链 SCM | 2021-2023 | 排单预测、出运计划、API 对接 |
| 金蝶云星瀚 APAAS（Java Gradle） | 销售 SOM | 2021-2023 | 销售预测、销售报价、API 对接 |
| 金蝶云星瀚 APAAS（Java Gradle） | 营销 MMS | 2021-2023 | 推广亚马逊SP/ST自动出价预算、报告上传、工作流、API 对接 |
| 金蝶云星瀚 APAAS（Java Gradle） | 财务 FMS | 2024-2025 | 对账、API 对接 |
| 菜鸟 | 仓储 WMS | 2025-2026 | API 对接 |
| Java SpringBoot Maven | 物流轨迹平台 PTC | 2025-至今 | 集成 trackingmore、amazonshipping 等第三方快递接口 |
| Java SpringBoot Maven | Oracle EBS 外挂 API 接口平台 | 2025-至今 | EBS 对外接口平台 |
| Java SpringBoot Maven | 齐套库存计算平台 CIC | 2025-至今 | 对接 WMS，分箱齐套库存计算 |
| Java SpringBoot Maven | 订单中心 OC | 2026-至今 | 各平台店铺订单下载、运单上传、产品更新等接口、SQS 通知、可观测性（@AosException、MDC、飞书异常通知） |
| Python | 多箱码垛系统 PL | 2025-2026 | Web、Mobile、PDA 三端集成，托盘装箱模拟 |
| 奥哲云枢 CloudPivot 8.6（Java Maven） | 奥哲云枢 APAAS POC | 2026-2026 | 租户扩展、用户扩展、launcher/user 服务扩展、前端模块 |
| 数式 Oinone 6.4.5（Java Maven） | 奥哲云枢 APAAS POC | 2026-2026 | 租户扩展、用户扩展、模型、AI Agent、前端模块 |
| 得帆 5.0（Java Maven） | 得帆 APAAS POC | 2026-2026 | 租户扩展、用户扩展、模型、AI Agent、前端模块 |
| Java SpringBoot Maven | 订单中心前端 oc-web | 2026-2026 | 多主题、订单查询多店铺、接口服务、账号管理 |
| Java SpringBoot Maven | 库存中心 IC | 2026-2026 | Mongo 库存快照/事务/保留/组合货号、XXL-Job 飞书心跳 |
| Cursor Agent / PowerShell | 通用技能子仓库 | 2026-2026 | `.cursor` 三 Submodule、技能 Hook 飞书台账、InnoSetup 安装包 |
| Cursor Agent / 飞书 MCP · Apifox CLI | 飞书项目 Apifox 接口规范流程 | 2026-2026 | 需求锁定 → OpenAPI → Apifox 导入 → CLI 冒烟四步技能包（WMS 装车单实践） |
| Cursor Agent / 飞书 CLI | AI 协作基础设施 | 2026-2026 | 日报填写技能包、Spec-DD 文档规范、飞书项目六步交付流程、Git 分支/提交规范 |

---

## 2. 技术栈

### 2.1 AI 辅助开发
- **AI IDE**：Cursor（AI 原生编辑器，代码补全、对话编程、多文件理解）
- **Agent Skills**：独立技能包（`SKILL.md` + `assets/` + `scripts/`），可整夹复制外传；`.cursor` 三 leaf **Git Submodule** 分发通用技能
- **Cursor Hooks**：`beforeSubmitPrompt` 技能使用埋点 → PowerShell → **lark-cli** 写飞书「技能使用次数」台账
- **飞书项目 MCP**：工作项锁定、`search_by_mql`、`add_comment` 回写（接口规范 / Apifox / 冒烟报告链）
- **lark-cli**：多维表读写、日历 `+agenda`、IM `+messages-search`、Wiki 文档入库（用户态 `identity=user`）
- **代码助手**：GitHub Copilot、通义灵码（代码生成、注释补全、单元测试）
- **规范驱动**：Spec-DD 规范文档 → AI 生成代码骨架与实现；OpenAPI 导入前检查清单门禁
- **Apifox CLI**：私有化 `--api-base-url`、`test-suite run`、`--upload-report` 冒烟与报告回写
- **协作提效**：飞书 AI、文档智能总结、知识库问答；日报多源采集（飞书结案 + Git + 日历 + IM）

### 2.2 数据库与数据工具
- Plsql、MongoDB Compass、DMS NineData、DBeaver、RedisDesktopManager

### 2.3 开发工具
- Cursor AI、IntelliJ IDEA、Eclipse、Visual Studio、VS Code
- **PowerShell**：Hook 脚本、技能包 `Import.ps1` / 台账写入、InnoSetup 编译辅助
- **InnoSetup**：Cursor 技能包 / Submodule 一键安装程序（`Aosom-Skills`）
- Notepad++

### 2.4 API 与测试
- **Apifox**（Web + **CLI**）：OpenAPI `import-data` HTTP 导入、测试套件冒烟、私有化部署基址
- Postman、Fork
- **OpenAPI 3**：规范驱动接口契约；`x-apifox-folder` 目录对齐；飞书 `work_item_id` 全链路追溯扩展字段

### 2.5 远程与运维
- SecureCRT、WinSCP、DAS-USM

### 2.6 消息队列
- Offset Explorer（Kafka Tool）

### 2.7 版本控制
- GitLab、GitHub、SVN
- **Git Submodule**：`kit-skills` 三 leaf（rules / commands / 通用技能）；英文 **kebab-case** 分支名（内网 push 稳定）

### 2.8 任务调度
- XXL-JOB

### 2.9 集成平台
- 得帆云 iPaaS 平台

### 2.10 协作与知识库
- **飞书项目**（Meego / IT-项目 MCP）、飞书云文档 / Wiki 知识库
- **飞书多维表（Base）**：IT 日报、通用 Skills 管理台账、技能使用次数、Apifox 接口发布记录

### 2.11 CI/CD 与质量
- Jenkins、SonarQube

### 2.12 监控与可观测
- Grafana、Prometheus、观测云、Kubernetes Rancher

### 2.13 日志链路
- OpenTelemetry（链路追踪）、ExceptionHandlerAspect（@AosException 切面）、AosLog、MDC 日志关联、飞书异常通知

### 2.14 ETL 与数据同步
- ETL DP、DataX

### 2.15 消息与集成
- Kafka、AWS SQS、Spring Cloud Stream

### 2.16 规则与重试
- QLExpress（规则引擎）、Spring Retry（重试机制）

### 2.17 测试与质量
- JUnit 5、Mockito、AssertJ、JaCoCo（覆盖率）

### 2.18 前端与 Web（2026 · oc-web）
- **Spring Boot + FreeMarker**：服务端渲染、宏组件化列表页
- **Spring Security**：登录/退出转场、角色菜单（管理员 / 销售 / 客服）
- **多主题 UI**：多前端风格切换；首选项多语言与时区（`localStorage` + `oc-web-ui.json`）
- **可插拔表格范式**：订单查询多店铺适配器、接口服务 `/ledger` HTTP 探测、库存四类 Mongo 只读列表

---

## 3. 产研能力

基于技术栈与业务项目实践，产研能力可归纳为以下维度：

### 3.1 AI 赋能
- **规范→代码**：Spec-DD 文档驱动，AI 根据规范生成 Controller/Service/Dao 完整实现
- **对话编程**：Cursor 多文件理解、上下文感知的代码补全与重构
- **问题排查**：AI 辅助日志分析、异常根因定位、飞书通知上下文解读
- **知识沉淀**：飞书云文档 + AI 总结，规范、功能文档可被 AI 检索与引用
- **飞书 MCP**：飞书项目需求/任务上下文接入 Cursor Agent，支撑需求锁定与协作台账联动
- **Apifox CLI**：需求锁定 → OpenAPI 生成 → Apifox 导入 → CLI 冒烟测试四步流程技能包（接口规范闭环）
- **飞书 CLI**：日报填写、Spec-DD 文档规范、飞书项目六步交付流程、Git 分支/提交规范等 AI 协作技能包
- **Agent 技能基建**：`.cursor` Submodule 技能子仓库、Hook 飞书台账、PowerShell/InnoSetup 安装包分发

### 3.2 技术栈广度
- **多语言**：Java（SpringBoot）、.NET、Python、Oracle PL/SQL
- **全栈工具链**：数据库（Oracle、MongoDB、Redis）、API 测试、CI/CD、监控、ETL 等覆盖研发全流程
- **云原生**：Kubernetes、Rancher 等容器编排与运维

### 3.3 业务领域深度
- **供应链全链路**：从 ERP（产品、采购、库存、成本）到订单 OMS、供应链 SCM、销售 SOM、营销 MMS、财务 FMS、仓储 WMS
- **物流与履约**：物流轨迹平台、快递接口集成、分仓分快递、拣货派遣
- **电商与订单**：多平台店铺订单（Amazon IE、Trendyol RO、Syncee FR 等）、运单上传、SQS 订单通知、RMA、泛欧销售
- **订单中心运营面**：oc-web 订单查询 / 接口服务探测 / 账号与库存管理；微服务台账与 K8s Ingress 对齐
- **库存域（oc-inv）**：Mongo 快照账本（按国别并行、飞书 Job 心跳）、事务/保留/组合货号同步与 CIC/EBS 契约

### 3.4 系统集成能力
- **API 对接**：EBS 外挂接口平台、各业务系统 API 对接、第三方快递接口（trackingmore、amazonshipping）
- **OpenAPI 契约闭环**：飞书锁定需求 → 【规范】+ OpenAPI → Apifox 导入 → CLI 冒烟 → MCP 评论回写（WMS 装车单等实践）
- **EBS 包体/存储过程**：`insert_order_iface`、平台商品同步、装车单/WMS 等性能与字段迭代
- **平台化**：得帆云 iPaaS、订单中心 OC、齐套库存计算平台 CIC
- **数据同步**：ETL DP、DataX 等数据集成与迁移
- **跨平台对接**：Amazon SP-API（refresh token、confirmShipment）、AWS S3/KMS/SQS、Oracle EBS SOAP

### 3.5 工程化能力
- **质量保障**：Jenkins、SonarQube 持续集成与代码质量
- **可观测性**：Grafana、Prometheus、观测云 监控与告警
- **任务调度**：XXL-JOB 定时任务与分布式调度；长 Job **飞书心跳**（快照账本等国别 k/N 进度）
- **日志链路**：基于 OpenTelemetry + AOP 的链路追踪，MDC 注入 traceId/spanId 实现日志关联，Slf4j 结构化日志，异常自动飞书通知（嵌套调用去重、连接重置静默）
- **Agent 技能治理**：Hook 四步接入（安装 → 本机 config → lark-cli 授权 → 试写）；扫描登记 + 使用次数公式汇总
- **多数据源**：dynamic-datasource 支持 MySQL、Oracle、MongoDB 动态切换
- **重试与容错**：Spring Retry 重试机制、消息幂等性设计
- **模块化架构**：common 公共模块 + 业务模块分层复用；`application-shared-*.yml` 瘦骨架 + 单服务覆盖
- **微服务分层**：Controller（API 入口）→ Service（业务逻辑）→ Dao/Repository（数据访问），Job 定时任务、Mapper 外部接口，common 抽象接口供业务模块实现

### 3.6 规范与交付
- **规范驱动**：Spec-DD 规范驱动开发，文档先行（规范 → 代码 → 测试）；【类型】中文文档命名与 `.docs/` 单源
- **飞书六步交付**：锁定任务 → 【功能】设计 + `add_comment` → 开发 → 验证 → 文档沉淀 → Git 分支与提交（分步人工确认）
- **日报与工时**：飞书 CLI 多源只读采集 + 预览定稿后写入 Base；空「大项」行复用、0.5h 步进与单日上限
- **版本与协作**：GitLab/GitHub、Submodule 协作（业务仓 commit Hook，源仓库本地安装）；飞书项目、飞书云文档知识库

### 3.7 测试与质量
- **单元测试**：JUnit 5、Mockito、AssertJ、JaCoCo 覆盖率
- **接口冒烟**：Apifox CLI 测试套件 + 报告上传；OpenAPI 导入前检查清单强制门禁
- **多环境配置**：Spring Profiles 切换、`application-ledger-{dev,test,prod}.yml` 探测矩阵、配置外部化、功能开关

### 3.8 安全与认证
- **OAuth 2.0**：Amazon SP-API refresh token 流程
- **云凭证**：AWS IAM 角色、环境变量、配置文件
- **Token 管理**：自动刷新、缓存、RestrictedDataToken
