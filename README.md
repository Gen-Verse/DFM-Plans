# DFM Plans

### Technical roadmap and developer entry point for Discovery Foundation Models

[中文](README_CN.md) · [Implementation Milestones](ROADMAP.md) · [Contributing](CONTRIBUTING.md)

This repository is the technical coordination point for **Discovery Foundation Models (DFMs)**. It tracks the implementation of DFM system modules and capabilities, links open-source releases and demos, and provides a clear entry point for developers who want to build with us.

The official DFM website will explain the broader vision, scientific context, scientist collaboration program, and application process. Those links will be added here when available. This repository stays focused on implementation and developer coordination.

DFM is defined by discovery capabilities rather than a single model checkpoint or architecture. Accordingly, this repository is a **roadmap and release index**, not necessarily one monolithic codebase. Individual implementations may live in separate repositories and will be linked here as they become available.

## What This Repository Tracks

- **Implementation milestones** — what is planned, in development, or released across the DFM system.
- **Open-source releases** — code, models, environments, evaluation tools, and reproducible artifacts.
- **Demos** — minimal examples and end-to-end demonstrations of DFM capabilities.
- **Developer collaboration** — technical issues, module interfaces, integrations, and contribution opportunities.

## Technical Scope

| Area | Examples |
| --- | --- |
| Core system | Research state, orchestration, provenance, memory, branching, and rollback |
| Discovery modules | Problem discovery and formulation, representation construction, hypothesis formation, intervention and experimentation, evidence-grounded revision |
| Training and improvement | Scientific post-training, process supervision, discovery skill learning, and continual improvement |
| Environments and evaluation | Digital, simulation, and physical grounding; process, transfer, efficiency, and control evaluation |
| Demos and integrations | Reproducible capability demos, domain adapters, tools, APIs, and external integrations |

The roadmap will evolve module by module. A capability is considered released only when its public artifact, usage instructions, evaluation evidence, and current limitations are linked from the milestone tracker.

## Start Here

- Check [ROADMAP.md](ROADMAP.md) for the current implementation status.
- Use [GitHub Issues](../../issues) for technical questions, proposals, and integration requests.
- Read [CONTRIBUTING.md](CONTRIBUTING.md) before submitting code, demos, documentation, or evaluation artifacts.

New directories will be added only when they contain an actual implementation, specification, or runnable demo.

## Contact

For technical collaboration related to DFM implementations, open-source releases, demos, or developer integration:

**[yang@phai-labs.com](mailto:yang@phai-labs.com)**
