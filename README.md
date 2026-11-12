# 出租车湖仓一体大数据分析系统

毕业设计课题：基于湖仓一体架构的出租车大数据分析系统的设计与实现。

项目计划使用纽约市 TLC 2025 年 Yellow 与 Green 出租车月度行程数据，在单节点 Ubuntu 虚拟机中验证历史处理、Iceberg 表管理、交互查询、可视化，以及同源片段的流式回放与批流对账。计划组件包括 RustFS、Iceberg、REST Catalog、Spark、Kafka、Flink、Trino、Superset、PostgreSQL 和 Docker Compose。实际组件版本与可运行范围以验证结果为准。

**当前状态：** 用户确认虚拟机目前只有 Ubuntu 基础环境，核心系统尚未实现。本目录先存放项目说明与[进度和 AI 接手记录](PROJECT_PROGRESS.md)，后续随开发加入代码、配置与验证记录。

## 计划实施顺序

1. 核对月度文件、字段、数据质量和使用条件。
2. 验证对象存储、目录、Iceberg、Spark、Trino 的最小读写闭环。
3. 完成历史数据清洗、分层存储、分析 SQL 和展示。
4. 加入受控回放、Kafka 和 Flink，验证批流统计及故障恢复。
5. 整理部署说明、测试记录和演示材料。

进度、难点和下一步以 [`PROJECT_PROGRESS.md`](PROJECT_PROGRESS.md) 为准。公开仓库只收录适合分享的源代码、配置模板和文档，不收录凭据、个人信息或全量原始数据。

