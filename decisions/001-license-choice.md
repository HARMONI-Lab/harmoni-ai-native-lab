# Decision Record: 001 - Open Core License Choice

## Context
The Harmoni AI-Native Lab requires a software license for its core infrastructure that aligns with our philosophy of Open Core, Open Science, and Open Source. The license needs to apply specifically to the lab infrastructure codebase, while recognizing that research outputs, trained models, and datasets may adopt separate, more specific open-science licenses (such as Creative Commons or specific OpenRAIL licenses) in the future.

## Decision
We have selected the **Apache License 2.0** for the core lab infrastructure.

## Rationale
- **Permissive Nature:** Apache 2.0 allows users to freely use, modify, distribute, and sell the software. This fits our goal to "foster innovation and collaboration" by allowing broad adoption without restrictive copyleft conditions that might deter commercial or widespread academic use.
- **Open Core Alignment:** As a permissive license, it naturally enables an open-core model. Commercial products or proprietary plugins can be built on top of the open-source infrastructure without legally requiring the downstream additions to also be open-source.
- **Patent Protection:** Unlike the MIT or BSD licenses, Apache 2.0 explicitly grants patent rights from contributors to users and includes a patent retaliation clause. This is vital for an AI-focused research lab where patentable methodologies, algorithms, and infrastructure components might be developed or utilized.
- **Clear Scope Separation:** By applying a permissive software license specifically to the infrastructure, we clearly delineate the "code/infrastructure" from "data and research outputs", empowering the lab to license datasets and papers under appropriate separate terms (e.g., CC-BY-4.0).

## Status
Accepted

## Consequences
- All infrastructure source code added to the repository must be compatible with Apache 2.0.
- Contributors agree to provide the explicit patent and copyright grants defined in the license.
- Non-software assets (datasets, weights, models, research papers) will need independent license evaluations and explicit declarations in their respective sub-directories.
