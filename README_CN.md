# Discovery Foundation Models

### 一个长期运行的 AI × Discovery 开放网络

> **连接前沿 AI、领域知识与真实世界发现。**

[English](README.md) · [开放问题](OPEN_PROBLEMS.md) · [合作](COLLABORATE.md) · [路线图](ROADMAP.md) · [贡献指南](CONTRIBUTING.md)

**联系方式：** [yang@phai-labs.com](mailto:yang@phai-labs.com) — 科研合作、领域合作、产业合作以及 Funded Projects。

**Discovery Foundation Models（DFMs）** 希望推动基础模型从解决已经定义好的任务，进一步走向**开放式发现**：主动发现值得研究的问题、构建和修正表征、形成可检验的假设、设计具有区分力的干预，并根据外部证据持续修正研究过程，最终不断提升发现能力本身。

**DFM Community** 是围绕这一愿景长期运行的网络，连接 **AI 研究者、领域科学家、基础设施建设者、科研机构、企业与真实研究环境**。

**DFM Commons** 是 Community 共同建设和共享的开放资源层，包括算法、基础设施、环境、Benchmark、数据、开放问题与可复现科研资产。

> **论文定义方向，Zetema 提供技术实现，DFM Community 持续扩展它。**

---

## 我们提供什么

对于具有实质性贡献的合作伙伴和重要研究方向，我们会积极支持：

- **科研合作与论文机会**：包括 DFM 主线工作、独立研究方向，以及与合适的高水平正刊、合作子刊、会议和跨学科项目进一步合作。
- **科研经费支持**：包括算力、工程支持、数据建设、Simulation、标注、实验费用以及 Wet-Lab 成本。
- **学术与真实场景合作**：从开放研究、联合研发，到 Domain Challenge、Pilot 和面向部署的真实验证。
- 对重要早期贡献者授予 **DFM Community Founding Contributor** 认可。

所有论文署名、成果归属与发表均依据实际科研贡献，并遵循正常、独立的同行评议流程。

---

## 什么是 DFM？

当前绝大多数基础模型开始工作时，人类已经提前定义好了问题、表征、目标、工具和评价标准。**Discovery 应该从更早的位置开始。**

我们将 DFM 概括为七项相互关联的核心能力：

**问题发现 → 问题定义 → 表征构建 → 假设形成 → 干预与实验 → 基于证据的修正 → 持续发现能力提升**

我们的目标，是让 Discovery 真正成为一种可以被**学习、执行、外部验证和系统评测**的模型能力。

---

## 如何参与

### 构建 Discovery Intelligence

探索 Discovery Agent、Scientific RL、Post-Training、Representation Construction、Intervention Design、Failure Attribution、World Model、Process-Level Scaling 和 Continual Discovery Skills。

### 构建 Discovery Infrastructure

建设 Research State、Branching & Rollback、Memory、Provenance、Tools、Environments、Verification、Experimental Gating、Dry/Wet-Lab Interface 与 Evaluation Infrastructure。

### Bring a World

你不需要是 AI 研究者。我们欢迎来自生物、化学、材料、医学、机器人、物理、数学、气候、工程、社会科学以及其他领域的专家。

你可以贡献：**真实科学问题、数据、Simulator、Benchmark、实验环境、Protocol、Validator、Wet-Lab 或 Domain Expertise**。

> **带来一个算法，带来基础设施，带来一个领域，或者带来一个真正困难的问题。**

---

## 仓库全貌

仓库会从一开始展示完整的 DFM Research Stack，即使部分模块尚未正式 release：

```text
DiscoveryModels/
├── zetema/         # DFM 参考系统组织
├── training/       # Capability Formation / Scientific Post-Training
├── environments/   # Digital / Simulation / Physical Grounding
├── evaluation/     # Process / Transfer / Efficiency / Controls
├── benchmarks/     # Discovery Benchmark
├── data/           # Trajectory / Interaction / Domain Data
├── domains/        # AI × 不同科学与工程领域
├── examples/       # 可复现实例与 Discovery Traces
├── docs/           # 扩展文档
├── community/      # DFM Community、合作伙伴与 Funded Challenges
└── discoveries/    # 未来经过外部验证的 Discovery Records
```

这些目录会提前展示，是为了让大家从第一天就看到 **DFM 的完整研究地图**。每个目录中的 README 都会明确说明其研究范围和当前状态。

---

## 开放研究地图

我们将开放问题组织在七项 DFM 能力与四类 Research Horizons 中：

**Digital → Simulation-Grounded → Physical → Recursive**

每一个交叉点都可能需要新的：

**算法 × Infrastructure × Environment × Benchmark × Domain**

初始 Research Agenda 见 [`OPEN_PROBLEMS.md`](OPEN_PROBLEMS.md)。

---

## 我们会逐步开源

包括：

- DFM / Zetema 基础设施
- Discovery 算法与训练方案
- Scientific RL 与 Process Supervision
- Research Environment 与 Benchmark
- Evaluation Protocol
- Discovery Skill Memory
- 不同领域中的真实实践与经验

这是一个持续演化的开放研究计划，而不是一次性的代码发布。

---

## 开放，但不降低标准

DFM Community 面向所有研究者开放，同时保持严格的科研标准。我们重视：

**可复现性 · Provenance · External Grounding · Falsification · Independent Validation · Transfer**

一个贡献是否重要，不取决于它听起来有多新，而取决于**它真正带来了什么，以及什么能够经受验证**。Negative Results、反例、复现失败，以及对当前 DFM Framework 的挑战，同样是有价值的贡献。

> **Open to everyone. Promoted by evidence.**

### Discovery 太广阔，不应该由单个实验室独立完成。

**一起构建 Discovery Network。**
