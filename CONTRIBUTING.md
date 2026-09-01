# Contributing to DFM Plans

This repository is the technical coordination point for DFM implementations, releases, demos, and integrations.

## Ways to Contribute

Useful contributions include:

- implementation of a defined DFM module or interface;
- minimal and end-to-end demos;
- environments, tools, adapters, and APIs;
- evaluation tasks, metrics, and reproducibility tooling;
- documentation, examples, and integration guides;
- bug reports, failed cases, and technically grounded design feedback.

## Contribution Flow

1. Check [ROADMAP.md](ROADMAP.md) and existing Issues.
2. Open an Issue before starting a large change. Describe the target module, proposed interface, expected artifact, and how it will be tested.
3. Keep pull requests focused on one module, demo, or integration.
4. Link the relevant milestone or Issue.
5. Include reproduction instructions and clearly state known limitations.

Code may live in this repository or in a linked implementation repository, depending on the module.

## Pull Request Checklist

A technical contribution should make clear:

- what capability or interface it implements;
- how to run the code or demo;
- what dependencies and data are required;
- what evidence shows that it works;
- what remains incomplete or unstable;
- whether any data, model, or third-party license restricts reuse.

Do not submit confidential, proprietary, personally identifiable, or otherwise restricted data.

## Technical Standard

We prioritize inspectable interfaces, reproducibility, provenance, external evidence, and evaluation beyond a single successful example. Negative results and well-documented failure cases are welcome when they improve the system design.

For technical questions, use GitHub Issues. For larger or non-public integration discussions, contact **[yang@phai-labs.com](mailto:yang@phai-labs.com)**.
