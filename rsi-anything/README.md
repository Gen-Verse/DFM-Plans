# RSI-Anything

**English** · [中文](README_CN.md) · **World-Model-Guided Recursive Self-Improvement**

**RSI-Anything: Unlocking Recursive Self-Improvement with World Models** connects the predictive foundation of [JEPA-Anything](../jepa-anything/README.md) to action selection, external feedback, and persistent system updates.

| | |
| --- | --- |
| **Paper** | [arXiv:2610.13912](https://arxiv.org/abs/2610.13912) |
| **Code & reproduction guides** | [Gen-Verse/RSI-Anything](https://github.com/Gen-Verse/RSI-Anything) |
| **Released** | October 2026 |
| **Applications** | Code repair, GUI interaction, laboratory planning, reaction optimization, immune-science workflows |

## Place in the DFM research map

**Propose → Predict → Select → Evaluate → Learn → Retain.**

A policy or scientific workflow proposes candidate actions. The world model predicts likely outcomes and helps select which actions to test. Actual environment or experimental feedback then supports improvement of the policy, predictive model, or workflow. Compatibility and validation checks determine which changes are retained for subsequent rounds.

Unlike predictive modeling on its own, the goal is **to turn predictions and externally observed outcomes into sustained improvement**. This complements [ScienceIDE](../scienceide/README.md)'s executable scientific environments and [ScienceInfra](https://github.com/Gen-Verse/ScienceInfra)'s training and evaluation workflows; it does not imply a single integrated deployment.

## Selected results

- **Code repair:** 26.3% hidden-test success for a static-verifier baseline, 29.2% with a fixed world model, and **31.2%** with a feedback-adapted world model under the reported protocol.
- **GUI:** **18.4% relative** improvement on OSWorld compared with the initial agent; the MiniWoB++ checkbox setting reaches 99% success in the reported evolved controller.
- **Laboratory planning and reaction optimization:** demonstrated successive policy improvement and feedback-guided selection of experimental conditions. See the [paper](https://arxiv.org/abs/2610.13912) and [benchmark documentation](https://github.com/Gen-Verse/RSI-Anything/blob/main/docs/benchmarks.md) for evaluation details.
- **Immune science:** reports a prospective intervention hypothesis for experimental testing, **not** a validated biological discovery.

These are study-specific results; domain adapters, data and evaluators differ across applications.

[← DFM research map](../README.md#research-progress)

