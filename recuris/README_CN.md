# Recuris

[English](README.md) · **中文** · **长程 Agent 的记忆与 Harness 演化**

**Recuris: Recursive Experiential–Working Memory Evolution for Long-Horizon Agent Harnesses** 研究在**冻结模型权重**的情况下，如何通过结构化记忆演化，持续提升 Agent 的长程任务能力。

| | |
| --- | --- |
| **论文** | [arXiv:2608.24876](https://arxiv.org/abs/2608.24876) |
| **代码** | [Gen-Verse/Recuris](https://github.com/Gen-Verse/Recuris) |
| **发布时间** | 2026 年 8 月 |
| **研究重点** | 长程任务、经验记忆、工作记忆、验证门控的局部修复 |

## 在 DFM 体系中的位置

Recuris 将**经验记忆**（已积累的技能与历史经验）和**工作记忆**（当前进度及尚未完成的目标）耦合起来。Meta-Agent 依据执行轨迹识别失败来源，只修复特定记忆组件，并在留出任务上的验证通过后保留更新。

在 DFM 研究体系中，这代表**持续改进 Agent 的另一条技术路线**：[ScienceBuddy](../sciencebuddy/README_CN.md) 关注 Harness 与模型的协同改进，[RSI-Anything](../rsi-anything/README_CN.md) 关注预测、行动、反馈和模型更新；Recuris 则探索在**不更新基座模型权重**时，长程记忆与工作流程能如何演化。

## 代表性证据

已公开研究在完成评估的 **37** 组模型—Benchmark 组合中有 **35** 组实现提升，部分长程场景增益更明显。不同模型与任务间存在差异，也有个别设置没有提升，详见[原项目仓库](https://github.com/Gen-Verse/Recuris)中的评测协议与完整结果。

[← 返回 DFM 研究版图](../README_CN.md#研究项目与进展)

