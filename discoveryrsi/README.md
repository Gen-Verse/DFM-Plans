# DiscoveryRSI

**English** · [中文](README_CN.md) · **Recursively Learning to Discover Valuable Hypotheses**

**DiscoveryRSI: Recursively Learning to Discover Valuable Hypotheses** studies research agents that improve from their own research experience — not only at executing tasks, but at deciding which hypotheses are worth pursuing and how to revise them.

| | |
| --- | --- |
| **Paper** | [arXiv:2610.23839](https://arxiv.org/abs/2610.23839) · [Technical report PDF](https://phai-labs.com/papers/discoveryrsi/discoveryrsi-technical-report-v1-2026-10.pdf) |
| **Code** | [Gen-Verse/DiscoveryRSI](https://github.com/Gen-Verse/DiscoveryRSI) |
| **Model** | [DiscoveryRSI-27B](https://huggingface.co/Gen-Verse/DiscoveryRSI-27B) · [Collection](https://huggingface.co/collections/Gen-Verse/discoveryrsi) |
| **Data** | [DiscoveryRSI-Hypothesis-Task-Examples](https://huggingface.co/datasets/Gen-Verse/DiscoveryRSI-Hypothesis-Task-Examples) |
| **Benchmark** | [DFM-Bench](https://github.com/Gen-Verse/DFM-Bench) |
| **Live arena** | [DiscoveryRSI Arena](https://foundry-arena.rsi-arena.workers.dev/arena) |
| **Released** | 2026-10-19 |
| **Domains** | Clinical & population health, therapeutic target prioritization, disease mechanisms, population multi-omics; battery science as a transfer test |

## What counts as a hypothesis

An evidence-grounded claim about a consequential uncertainty, paired with a feasible investigation, explicit decision criteria, and alternative explanations.

## Place in the DFM research map

**Hypothesis tree → Compile → Record → Improve → Rediscover.**

1. **Hypothesis tree.** A lead agent coordinates multi-agent evolutionary search (evolve, repair, crossover, restart, select); every version is critiqued.
2. **Compilation.** Selected computational investigations are compiled into executable [Harbor](https://github.com/laude-institute/harbor) tasks with inputs, environments, outputs and checks.
3. **Research record.** Evidence, decisions, assessments and contributions are kept for every proposal and revision.
4. **Three coupled improvement mechanisms:**
   - *Hypothesis credit optimization* — attributes assessments to the documented contributions behind them and trains **DiscoveryRSI-27B**;
   - *Harness replay* — mines productive strategies and recurring failures from the record to refine the workflow, gated by a dev-set check;
   - *Rediscovery* — applies accepted updates to fresh questions, producing experience for the next round.

Where [ScienceBuddy](../sciencebuddy/README.md) couples harness and model learning in interactive research, and [RSI-Anything](../rsi-anything/README.md) uses world models to select actions, DiscoveryRSI applies recursive improvement to the **research question itself**. Its Harbor tasks connect to the executable-environment line of [ScienceIDE](../scienceide/README.md) and [ScienceInfra](https://github.com/Gen-Verse/ScienceInfra). This is a research relationship, not a single integrated deployment.

## DFM-Bench

[DFM-Bench](https://github.com/Gen-Verse/DFM-Bench) evaluates cumulative research progress at five levels — **hypothesis, transition (each revision), trajectory (development path), campaign (whole research graph), and discovery (deduplicated contribution families)** — plus a separate delivery axis for completion, compilation and readiness. Campaign scores are not averages of hypothesis scores, and contribution families are not confirmed discoveries.

## Selected results

- **Hypothesis quality:** mean score **4.86 → 5.39** after two rounds of self-improvement, driven by testability — falsifiability **4.00 → 6.20**, alternative explanations **4.44 → 5.98**, data resolvability **3.73 → 4.99**.
- **Research behavior:** episodes that develop or repair an existing hypothesis rise from **77.5% to 91.7%**; restarts with a new question fall from **21.7% to 5.0%**.
- **Expert review:** **27** reviewers with biomedical or clinical backgrounds blind-assessed **292** proposals; mean score change per revision was **+0.07** for DiscoveryRSI-27B vs. +0.03 and −0.01 for the two compared frontier models.
- **Later literature:** **6.3%** of DiscoveryRSI-27B's hypotheses have a concrete connection to research published after the model cutoff that a researcher could build on — the highest among compared models.
- **Versus base model:** in matched runs, DiscoveryRSI-27B selected **16.7% more** unique hypotheses and compiled **50% more** Harbor tasks.

## Limitations

After two rounds, automated importance and novelty scores fall; the gains are in investigation design. Human assessments are preliminary, revision comparisons are made within research trees, and the published-research comparison is descriptive, with differing group sizes and cutoffs. Whether researchers adopt these hypotheses requires prospective tracking. No patient data, UK Biobank material, or private campaign traces are bundled in the release.

## Citation

```bibtex
@article{zhong2026discoveryrsi,
  title={DiscoveryRSI: Recursively Learning to Discover Valuable Hypotheses},
  author={Zhong, Jianyuan and Wu, Chenwei and Yu, Zhaochen and Jiang, Xixian and Li, Xuewei and Xiao, Hao and Dai, Xilin and Wang, Junyang and Zou, Jiaru and Cui, Zhiqing and Zheng, Boyuan and Xiong, Jing and Zhang, Zhen and Gao, Qiang and Morley, Michael and Nakayama, Luis and Xu, Qiang and Shen, Liyue and Gui, Tao and Celi, Leo Anthony and Zou, James and Yin, Zhenfei and Wu, Yingcheng and Yang, Ling},
  journal={arXiv preprint arXiv:2610.23839},
  year={2026}
}
```

[← DFM research map](../README.md#research-progress)
