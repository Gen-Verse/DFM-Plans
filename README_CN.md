# DFM Plans

### Discovery Foundation Models 技术路线图与开发者入口

[English](README.md) · [实现里程碑](ROADMAP.md) · [贡献指南](CONTRIBUTING.md)

这个仓库是 **Discovery Foundation Models（DFMs）** 的技术对接入口。后续会持续更新 DFM 系统不同模块与能力的实现进展，汇总开源发布与 Demo，并为开发者提供明确的参与和协作路径。

DFM 的整体愿景、科学背景、科学家合作计划和申请入口将由官方网站负责承接，相关链接上线后会放在这里。这个仓库只聚焦技术实现与开发者协作。

DFM 由一组发现能力定义，而不是某一个模型 checkpoint 或固定架构。因此，这里主要承担的是**技术路线图与发布索引**，不要求所有实现都集中在同一个代码仓库中。不同模块的独立仓库会在发布后统一链接到这里。

## 这里会更新什么

- **实现里程碑**：DFM 各系统模块当前处于规划、开发还是发布阶段。
- **技术开源**：代码、模型、环境、评测工具与可复现资产。
- **Demo**：单项能力的最小示例，以及端到端系统演示。
- **开发者协作**：技术问题、模块接口、外部集成与贡献机会。

## 技术范围

| 模块 | 主要内容 |
| --- | --- |
| 核心系统 | Research State、任务编排、Provenance、Memory、Branching 与 Rollback |
| Discovery 模块 | 问题发现与定义、表征构建、假设形成、干预与实验、基于证据的修正 |
| 训练与持续改进 | Scientific Post-training、Process Supervision、Discovery Skill Learning 与 Continual Improvement |
| 环境与评测 | Digital、Simulation 与 Physical Grounding；Process、Transfer、Efficiency 与 Control Evaluation |
| Demo 与集成 | 可复现能力 Demo、Domain Adapter、工具、API 与外部系统集成 |

我们会按照模块逐步推进。只有当公开资产、使用说明、评测证据和当前局限都已明确链接时，对应能力才会在里程碑中标记为已发布。

## 从这里开始

- 在 [ROADMAP.md](ROADMAP.md) 查看当前实现状态。
- 通过 [GitHub Issues](../../issues) 提出技术问题、模块建议与集成需求。
- 提交代码、Demo、文档或评测资产前，请阅读 [CONTRIBUTING.md](CONTRIBUTING.md)。

只有当实际实现、接口规范或可运行 Demo 出现时，仓库才会新增相应目录。

## 联系方式

如需围绕 DFM 模块实现、技术开源、Demo 或开发者集成展开合作，请联系：

**[yang@phai-labs.com](mailto:yang@phai-labs.com)**
