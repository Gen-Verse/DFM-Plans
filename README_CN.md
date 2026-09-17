# Discovery Foundation Models

### 发现智能 · 研究与开源

[English](README.md) · **中文** · [官方网站](https://phai-labs.com/) · [技术报告](https://arxiv.org/abs/2609.15973) · [研究项目与进展](#研究项目与进展) · [科学家合作计划](https://phai-labs.com/collaborate/)

**从回答问题、执行任务，走向发现有价值的未知。**

Discovery Foundation Models（DFMs）探索 AI 如何发现问题、形成可研究的问题、构造科学表征与假设、获取外部证据，并在不同任务中持续提升发现能力。

本仓库由 **[PhAI Labs](https://phai-labs.com/)** 发起，汇总 DFM 技术报告、研究版图、成果介绍与开放研究入口。**各项研究工作将在独立 GitHub 仓库中开发和发布；DFM-Plans 负责汇总、里程碑更新与项目导航。**

<p align="center">
  <img src="assets/dfm-architecture-zh.webp" width="1000" alt="发现智能：Chat、Agent 与 Discovery 的演进，以及递归发现闭环。">
</p>

*发现智能架构：连接外部实验、五层协同与闭环反馈。*

## 技术报告

**[Discovery Foundation Models: Toward Open-Ended Discovery Intelligence](https://arxiv.org/abs/2609.15973)** — 技术报告。

报告提出七项核心能力：**问题发现、问题形成、表征构造、假设形成、干预与实验、证据驱动的修正，以及跨任务的持续发现能力提升。**

参考架构 **Zetema** 探索如何通过显式研究状态、记忆、科学工具、实验环境、验证机制和人类监督，组织递归发现循环。它是一套研究设计；具体实现与验证进展将通过各项独立研究持续更新。

## 研究项目与进展

从 **Chat** 到 **Code**，再到 **Discovery Intelligence**，AI 的学习经验从已有知识扩展到行动反馈，进一步进入科学研究过程。我们围绕支撑这一转变的科学数据、环境与反馈，推进三个具体项目：

| 方向 | 项目 | 研究重点 | 发布日期 / 计划 | 项目入口 |
| --- | --- | --- | --- | --- |
| **科学家交互** | **[ScienceBuddy](sciencebuddy/README_CN.md)** | 科研交互工作空间，通过递归嵌套的自我改进协同优化 Agent Harness 与模型 | 已发布 · 2026-09-16 | [论文](https://arxiv.org/abs/2609.17523) · [代码](https://github.com/Gen-Verse/ScienceBuddy) · [产品](http://science-buddy.io/) |
| **科学环境** | **[ScienceIDE](scienceide/README_CN.md)** | 将科学代码转化为可执行、可验证的学习环境，支持 SFT、RL 与评测 | 已发布 · 2026-09-17 | [论文](https://arxiv.org/abs/2609.19134) · [代码](https://github.com/aitofound/ScienceIDE) · [模型](https://huggingface.co/collections/AItonomy/scienceide-model-series) |
| **科学世界模型** | **JEPA Anything** | 跨领域科学状态表征与干预后的状态变化预测 | 2026 年 9 月 18 日 | [Overview](https://phai-labs.com/papers/) · Code: Coming Soon |

三个项目围绕**交互反馈、可复用环境与世界状态预测**展开，共同服务于 DFM 的研究目标，各自独立开发、评测和发布。科学数据与发现推理贯穿其中。

**当前状态**：ScienceBuddy 已发布预览产品、论文与研究代码；ScienceIDE 已发布论文、预览代码、部分科学环境与任务，以及 PhAI-IDE-4B、9B、72B 模型系列。训练与评测基础设施的持续建设见 [ScienceInfra](https://github.com/Gen-Verse/ScienceInfra)。JEPA Anything 仍按上表计划推进，具体技术文档与后续版本由各自项目仓库维护。

## 科学家合作计划

<p align="center">
  <a href="https://phai-labs.com/collaborate/">
    <img src="assets/scientist-collaboration-zh.jpg" width="1000" alt="DFM 科学家合作计划中文页面预览。">
  </a>
</p>

欢迎拥有重要开放问题、专业数据、可执行环境或真实实验验证条件的科学家、研究团队与实验平台参与合作。

- **[申请加入 DFM 科学家合作计划](https://ecnxosgyafi8.feishu.cn/wiki/Z1A2wr23ViqAOBkq3xfcgfl7nZg?table=tblboSz1SkRQ0iM2&view=vewoiUIlNk)**
- **[DFM 科学家合作计划介绍](https://phai-labs.com/collaborate/)**

## 开发者导航与索引维护

- 代码、安装说明、技术问题、Issue 与贡献方式，请前往对应项目的独立仓库。
- 如需推荐收录项目、纠正链接或讨论整体研究版图，请使用[本仓库 Issues](https://github.com/Gen-Verse/DFM-Plans/issues)。
- 提交索引或里程碑更新，请参阅 [贡献指南](CONTRIBUTING_CN.md)。

## 引用与联系

如果本研究对你有帮助，请引用 DFM 技术报告；使用具体项目时，也请引用相应项目论文。

```bibtex
@article{yang2026discovery,
  title={Discovery Foundation Models: Toward Open-Ended Discovery Intelligence},
  author={Yang, Ling and Yin, Zhenfei and Wu, Yingcheng},
  journal={arXiv preprint arXiv:2609.15973},
  year={2026}
}
```

<details>
<summary>ScienceBuddy</summary>

```bibtex
@article{xue2026sciencebuddy,
  title={ScienceBuddy: Recursive-in-Recursive Self-Improvement for Interactive Scientific Agents},
  author={Xue, Shuhan and Zhong, Jianyuan and Nan, Ziyuan and Li, Wenbin and Yu, Zhaochen and Ding, Jinchao and Gao, Qiang and Zhan, Pengyu and Zhang, Yuntong and Cheng, Tian and Yin, Zhenfei and Wu, Yingcheng and Yang, Ling},
  journal={arXiv preprint arXiv:2609.17523},
  year={2026}
}
```

</details>

<details>
<summary>ScienceIDE</summary>

```bibtex
@article{geng2026scienceide,
  title={ScienceIDE: Turning World's Scientific Codebase into Agent Learnable Environments},
  author={Geng, Hejia and Huang, Zesen and Li, Haoyang and Li, Wenbin and Wu, Koutian and Zhou, Zihan and Pang, Yuanbo and Liu, Weihao and Xu, Zigong and Li, Zhiping and Zhang, Zongzheng and Dong, Chuanfei and Sun, Jiankai and Zheng, Tianzhe and Xie, Fengyu and Ma, Yue and Shi, Yueheng and Xie, Tong and Di, Zonglin and Liu, Xianrong and Gao, Qucheng and Liu, Yimin and Pan, Jiaming and Huang, Sheng and Ma, Xiao-Han and Yuan, Lanqing and Zhu, Zhenlin and Liu, Ziang and Xu, Ziyang and Wang, Junkai and Liang, Kangkai and Xian, Jiayi and Zhao, Zehong and Xu, Liuwei and Xie, Jingxu and Zhang, Peijin and Gao, Qiang and Xing, Chengyi and Zhao, Zhe and Wang, Xi and Xing, Yaopeng and Meng, Xing and Yin, Zhenfei and Wu, Yingcheng and Yang, Ling},
  journal={arXiv preprint arXiv:2609.19134},
  year={2026}
}
```

</details>

**PhAI Labs** · [官方网站](https://phai-labs.com/) · [yang@phai-labs.com](mailto:yang@phai-labs.com)
