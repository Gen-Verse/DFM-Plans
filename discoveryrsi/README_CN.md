# DiscoveryRSI

[English](README.md) · **中文** · **递归学习发现有价值的假设**

**DiscoveryRSI: Recursively Learning to Discover Valuable Hypotheses** 研究让研究智能体从自己的研究经历中持续改进 —— 不只是更好地执行任务，而是更好地判断哪些假设值得推进、以及如何修订它们。

| | |
| --- | --- |
| **论文** | [arXiv:2610.23839](https://arxiv.org/abs/2610.23839) · [技术报告 PDF](https://phai-labs.com/papers/discoveryrsi/discoveryrsi-technical-report-v1-2026-10.pdf) |
| **代码** | [Gen-Verse/DiscoveryRSI](https://github.com/Gen-Verse/DiscoveryRSI) |
| **模型** | [DiscoveryRSI-27B](https://huggingface.co/Gen-Verse/DiscoveryRSI-27B) · [模型合集](https://huggingface.co/collections/Gen-Verse/discoveryrsi) |
| **数据** | [DiscoveryRSI-Hypothesis-Task-Examples](https://huggingface.co/datasets/Gen-Verse/DiscoveryRSI-Hypothesis-Task-Examples) |
| **评测** | [DFM-Bench](https://github.com/Gen-Verse/DFM-Bench) |
| **在线 Arena** | [DiscoveryRSI Arena](https://foundry-arena.rsi-arena.workers.dev/arena) |
| **发布** | 2026-10-19 · [发布介绍](https://phai-labs.com/news/discoveryrsi/) |
| **领域** | 临床与人群健康、治疗靶点优先级排序、疾病机制、人群多组学；以电池科学检验跨领域迁移 |

## 什么是“假设”

针对一个关键不确定性、有证据支撑的论断，并配有可行的研究方案、明确的判定标准以及备择解释。

## 在 DFM 研究版图中的位置

**假设树 → 编译 → 记录 → 改进 → 重新发现。**

1. **假设树。** 由 Lead Agent 协调多智能体演化搜索（演化、修复、交叉、重启、选择），每个版本都经过评议。
2. **编译。** 选中的计算研究被编译为可执行的 [Harbor](https://github.com/laude-institute/harbor) 任务，包含输入、环境、输出与检查。
3. **研究记录。** 每个提案与修订都保留证据、决策、评估和贡献记录。
4. **三种衔接的改进机制：**
   - *假设贡献度优化* —— 把研究质量评估归到具体贡献上，用于训练 **DiscoveryRSI-27B**；
   - *Harness 回放* —— 从研究记录中找出有效策略和反复出现的失败，改进工作流，并经开发集检验；
   - *重新发现* —— 把通过检验的更新应用到新的研究问题上，产生下一轮学习的经验。

[ScienceBuddy](../sciencebuddy/README_CN.md) 在交互式研究中协同改进 Harness 与模型，[RSI-Anything](../rsi-anything/README_CN.md) 用世界模型选择行动；DiscoveryRSI 则把递归改进作用于**研究问题本身**。其 Harbor 任务与 [ScienceIDE](../scienceide/README_CN.md)、[ScienceInfra](https://github.com/Gen-Verse/ScienceInfra) 的可执行环境路线相衔接。这是研究层面的关联，并非同一套已集成部署的系统。

## DFM-Bench

[DFM-Bench](https://github.com/Gen-Verse/DFM-Bench) 从五个层级评估累积的研究进展 —— **假设、修订（每一次父子修订）、发展路径、整轮研究（完整研究图）以及发现（去重后的贡献族）** —— 另设交付维度，评估完成度、编译情况与就绪程度。整轮研究得分不是假设得分的平均，贡献族也不等于已确认的发现。

## 代表性结果

- **假设质量：** 两轮自我改进后平均分 **4.86 → 5.39**，提升主要在可检验性 —— 可证伪性 **4.00 → 6.20**，备择解释 **4.44 → 5.98**，数据能否回答问题 **3.73 → 4.99**。
- **研究行为：** 推进或修复已有假设的回合占比从 **77.5% 升至 91.7%**，另起新问题的占比从 **21.7% 降至 5.0%**。
- **专家评审：** **27** 名生物医学或临床背景评审者盲评 **292** 份提案，每次修订的平均分变化：DiscoveryRSI-27B 为 **+0.07**，两个对照前沿模型分别为 +0.03 与 −0.01。
- **与后续文献对照：** DiscoveryRSI-27B 有 **6.3%** 的假设与模型截止日期之后发表的研究存在具体可延续的联系，在参与对照的模型中最高。
- **相对基座模型：** 在匹配运行中，DiscoveryRSI-27B 选出的不同假设多 **16.7%**，编译的 Harbor 任务多 **50%**。

## 局限

两轮后重要性与新颖性的自动评分有所下降，提升主要体现在研究方案设计上。人工评审为初步结果，修订比较限于研究树内部，与已发表研究的对照仅为描述性比较（各组规模与截止时间不同），假设的实际采纳效果有待前瞻性追踪。发布内容不包含任何患者数据、UK Biobank 材料或私有研究轨迹。

## 引用

```bibtex
@article{zhong2026discoveryrsi,
  title={DiscoveryRSI: Recursively Learning to Discover Valuable Hypotheses},
  author={Zhong, Jianyuan and Wu, Chenwei and Yu, Zhaochen and Jiang, Xixian and Li, Xuewei and Xiao, Hao and Dai, Xilin and Wang, Junyang and Zou, Jiaru and Cui, Zhiqing and Zheng, Boyuan and Xiong, Jing and Zhang, Zhen and Gao, Qiang and Morley, Michael and Nakayama, Luis and Xu, Qiang and Shen, Liyue and Gui, Tao and Celi, Leo Anthony and Zou, James and Yin, Zhenfei and Wu, Yingcheng and Yang, Ling},
  journal={arXiv preprint arXiv:2610.23839},
  year={2026}
}
```

[← DFM 研究版图](../README_CN.md#研究项目与进展)
