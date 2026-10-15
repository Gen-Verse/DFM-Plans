# Recuris

**English** · [中文](README_CN.md) · **Long-Horizon Memory and Harness Evolution**

**Recuris: Recursive Experiential–Working Memory Evolution for Long-Horizon Agent Harnesses** studies how a frozen agent can improve through structured memory evolution rather than model weight updates.

| | |
| --- | --- |
| **Paper** | [arXiv:2608.24876](https://arxiv.org/abs/2608.24876) |
| **Code** | [Gen-Verse/Recuris](https://github.com/Gen-Verse/Recuris) |
| **Released** | August 2026 |
| **Focus** | Long-horizon agent tasks, experiential memory, working memory, validation-gated edits |

## Place in the DFM research map

Recuris couples **experiential memory** (reusable skills and past outcomes) with **working memory** (current progress and unresolved goals). A meta-agent traces failures to specific memory components, proposes localized repairs, and retains them only after validation on held-out evidence.

Within the DFM agenda, it demonstrates a complementary route to **persistent agent improvement**. Where [ScienceBuddy](../sciencebuddy/README.md) studies joint harness and model learning and [RSI-Anything](../rsi-anything/README.md) connects predictions with policy/world-model updates, Recuris studies what can improve **without changing the base model**.

## Selected evidence

The released study reports gains in **35 of 37** completed model–benchmark pairs, with larger gains in selected long-horizon settings. Results vary by model and benchmark, and some individual comparisons do not improve. See [the original repository](https://github.com/Gen-Verse/Recuris) for evaluation protocols and complete tables.

[← DFM research map](../README.md#research-progress)

