# RSI-Anything

[English](README.md) · **中文** · **世界模型驱动的递归自我改进**

**RSI-Anything: Unlocking Recursive Self-Improvement with World Models** 将 [JEPA-Anything](../jepa-anything/README_CN.md) 的预测世界模型与行动选择、外部反馈和可保留的系统改进连接起来。

| | |
| --- | --- |
| **论文** | [arXiv:2610.13912](https://arxiv.org/abs/2610.13912) |
| **代码与复现** | [Gen-Verse/RSI-Anything](https://github.com/Gen-Verse/RSI-Anything) |
| **发布时间** | 2026 年 10 月 |
| **研究场景** | 代码修复、GUI 交互、实验室规划、反应条件优化、免疫科学工作流 |

## 在 DFM 体系中的位置

**提出候选 → 预测结果 → 选择行动 → 外部验证 → 学习更新 → 保留改进。**

Policy 或研究流程提出候选行动，世界模型预测可能结果并辅助选择值得测试的行动；随后依据真实环境或实验反馈，更新 Policy、世界模型或 Harness，并通过验证和兼容性检查决定是否保留改进，用于下一轮任务。

这项工作的核心不仅是预测，而是**将预测和外部证据连接为持续改进机制**。它与 [ScienceIDE](../scienceide/README_CN.md) 提供的可执行科学环境、[ScienceInfra](https://github.com/Gen-Verse/ScienceInfra) 提供的训练评测基础设施互补，但并不意味着这些系统已实现完整集成部署。

## 代表性结果

- **代码修复：**静态 Verifier 基线 **26.3%**，固定世界模型 **29.2%**，根据反馈适配世界模型后达到 **31.2%**。
- **GUI：**OSWorld 相比初始 Agent 的任务成功率**相对提升 18.4%**；MiniWoB++ checkbox 设置下迭代后的控制器达到 99% 成功率。
- **实验室规划与反应优化：**报告了多轮策略改进和基于反馈的实验条件选择，详细设置见[论文](https://arxiv.org/abs/2610.13912)及[实验说明](https://github.com/Gen-Verse/RSI-Anything/blob/main/docs/benchmarks.md)。
- **免疫科学：**提出供后续实验检验的候选干预假设，**不代表已经验证的生物学发现**。

不同场景使用独立的数据、任务接口与评估标准，结果不可直接横向比较。

[← 返回 DFM 研究版图](../README_CN.md#研究项目与进展)

