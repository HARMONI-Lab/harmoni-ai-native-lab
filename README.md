# Harmoni AI-Native Lab

The operational infrastructure for an AI-native independent research lab focused on AI in women's health. Our mission is to accelerate discoveries and improve health outcomes for women by leveraging artificial intelligence, rigorous research methodologies, and collaborative open science.

## Table of Contents

- [Status](#status)
- [Philosophy](#philosophy)
- [License](#license)
- [Part 1: Lab Description](#part-1-lab-description)
  - [What This Lab Is](#what-this-lab-is)
  - [Mission](#mission)
  - [Operating Principles](#operating-principles)
  - [Domain Focus](#domain-focus)
  - [Operational Stack](#operational-stack)
  - [Roles](#roles)
  - [What This Lab Produces](#what-this-lab-produces)
- [Part 2: Step-by-Step Execution Plan](#part-2-step-by-step-execution-plan)
  - [Phase 1: Foundation](#phase-1-foundation)
  - [Phase 2: LLM Runtime](#phase-2-llm-runtime)
  - [Phase 3: Knowledge Base (`lab-brain`)](#phase-3-knowledge-base-lab-brain)
  - [Phase 4: Developer Experience](#phase-4-developer-experience)
  - [Phase 5: Contributor Infrastructure](#phase-5-contributor-infrastructure)
  - [Phase 6: Automation](#phase-6-automation)
  - [Phase 7: Public Presence](#phase-7-public-presence)
  - [Phase 8: Governance](#phase-8-governance)
- [Part 3: Suggested Build Schedule](#part-3-suggested-build-schedule)
- [Part 4: Minimum Viable Lab](#part-4-minimum-viable-lab)
- [Part 5: What Success Looks Like](#part-5-what-success-looks-like)
- [Part 6: One Guiding Principle](#part-6-one-guiding-principle)

## Status
**under construction**

## Philosophy
Our lab is built upon three foundational principles:
- **Open Core:** We build on and contribute to robust, extensible open technologies.
- **Open Science:** We are committed to transparency, reproducibility, and sharing our methodologies and findings with the global community.
- **Open Source:** We release our tools, models, and infrastructure under permissive licenses to foster innovation and collaboration.

## License
The lab infrastructure itself is licensed under the [Apache License 2.0](LICENSE). 

*Note: Research outputs, models, and datasets may have separate licenses defined independently as they are released.*

---

# AI-Native Independent Lab: Description & Execution Plan

---

# Part 1: Lab Description

## What This Lab Is

An **AI-native, independent research lab** at the intersection of **artificial intelligence and women's health**, operated by a **single Principal Investigator** with a community of **distributed open source contributors**, built on a foundation of **open core, open science, and open source** principles.

The lab is structured as a **lean operational system** rather than a traditional research institution. It uses **local-first AI** as a persistent collaborator across research, writing, coding, knowledge management, and community coordination. The lab produces **open datasets, open methods, open tools, and open publications** designed to address the systemic underrepresentation of women's health in both medical research and AI applications.

---

## Mission

To advance AI research in women's health by:

- closing data and methodological gaps left by decades of underrepresentation
- producing open, reproducible, and equitable AI tools and datasets
- demonstrating that a single researcher, supported by AI and community, can run a credible, productive, and impactful research program
- building public infrastructure that other women's health researchers can build on

---

## Operating Principles

### 1. AI-Native, Not AI-Enhanced
AI is not an add-on. It is the operational layer underneath research, coding, writing, documentation, and coordination. The lab is designed assuming AI participation from day zero.

### 2. Local-First AI
The lab prefers locally-run open weight models (Gemma 4 via Ollama) for privacy, cost control, sovereignty, and alignment with open science values. Cloud AI is used only when local capacity is insufficient.

### 3. Open by Default
Code, data, decisions, methods, governance, and even research process artifacts are public by default. Privacy and ethics determine what is held back, not convenience or competitive advantage.

### 4. Lean Operations
The lab uses the smallest viable toolchain: GitHub, Zenodo, Google Workspace, Mercury, Ollama, and a Python-based development stack. New tools must justify their existence by solving a specific, painful problem.

### 5. Community as the Lab
Open source contributors are not peripheral helpers. They are the extended research team. The infrastructure is designed to make contribution self-serve and asynchronous.

### 6. Knowledge Compounding
Institutional memory accumulates in a structured `lab-brain` knowledge base — readable by both humans and the local LLM. Nothing important is reconstructed twice.

### 7. Reproducibility as Architecture
Every experiment, dataset, decision, and analysis is reproducible by design. Reproducibility is structural, not policy.

### 8. Equity Lens on Every Decision
The lab exists partly because mainstream research has systematically underrepresented women's health. Every methodological, data, and design decision is examined through that corrective lens.

---

## Domain Focus

**AI in women's health research**, with explicit attention to:

- understudied conditions (endometriosis, menopause, PCOS, maternal health)
- data gaps across demographics, race, socioeconomic status, and geography
- bias in existing models and datasets
- diagnostic disparities
- patient-centered AI applications
- ethical use of sensitive health data

---

## Operational Stack

| Layer | Tool |
|---|---|
| Code, issues, project tracking, contributor coordination | **GitHub** |
| Datasets and papers | **Zenodo** |
| Email and document storage | **Google Workspace** |
| Banking and entity | **Mercury** |
| Local LLM runtime | **Ollama** |
| Primary model | **Gemma 4** |
| Editor | **VS Code + Continue** |
| Python tooling | **uv, ruff, pre-commit** |
| Knowledge base | **`lab-brain`** (markdown in Git) |
| Public site | **GitHub Pages** |
| Async community | **GitHub Discussions** |

---

## Roles

### The PI
- Sets research direction
- Final authority on scientific, ethical, and editorial decisions
- Curates contributor community
- Maintains the `lab-brain`
- Publishes outputs

### The Local LLM (Gemma 4)
- Daily research collaborator
- Coding assistant
- Literature processor
- Briefing generator
- Code reviewer
- Writing partner
- Context-aware lab assistant via the `lab-brain`

### Open Source Contributors
- Code contributions
- Data contributions
- Documentation
- Domain expertise
- Research input
- Community support

---

## What This Lab Produces

- Open datasets (published on Zenodo)
- Open source AI tools and methods (published on GitHub)
- Open access papers and preprints
- Public research agenda
- Reusable lab infrastructure (this repository)
- Documented methods, decisions, and negative results

---

# Part 2: Step-by-Step Execution Plan

The plan is organized into **eight phases** mapped to the eight milestones from the GitHub issue plan. Each phase has objectives, detailed actions, deliverables, dependencies, and success criteria.

---

## Phase 1: Foundation

**Goal:** Establish a stable, reproducible repository with technical baseline.

### Step 1.1 — Create the repository
- Create new GitHub repository (suggested name: `ai-native-lab` or similar)
- Set visibility to public
- Initialize with no default files (you will add them deliberately)

### Step 1.2 — Write the initial README
- One-paragraph mission statement
- "Philosophy" section describing open core, open science, open source
- "Status" section with `🚧 under construction` indicator
- Placeholder table of contents

### Step 1.3 — Choose and apply a license
- Decide on open source license aligned with open core philosophy (e.g., MIT, Apache 2.0, or AGPL depending on intent)
- Add `LICENSE` file
- Reference license in README
- Document rationale in `/decisions/001-license-choice.md`

### Step 1.4 — Establish decisions log
- Create `/decisions` directory
- Add `000-template.md` with fields: date, status, context, decision, consequences
- File the license decision as the first ADR

### Step 1.5 — Configure `.gitignore`
- Cover Python, Jupyter, virtual environments, OS files, common data file patterns, model weights
- Add commented section headers

### Step 1.6 — Initialize Python project with `uv`
- Install `uv`
- Create `pyproject.toml` with project metadata
- Specify minimum Python version
- Test virtual environment creation
- Document development setup in README

### Step 1.7 — Configure `ruff`
- Add as dev dependency
- Add `[tool.ruff]` section to `pyproject.toml`
- Choose a strict but reasonable rule set
- Verify clean run of `ruff check .` and `ruff format .`

### Step 1.8 — Set up `pre-commit`
- Create `.pre-commit-config.yaml`
- Hooks: ruff lint, ruff format, trailing whitespace, end-of-file fixer, YAML check, large file check
- Test with sample commit
- Document `pre-commit install` in README

### Step 1.9 — Create directory structure
```
/src
/notebooks
/docs
/decisions
/lab-brain
/scripts
/tests
```
- Add a brief `README.md` to each
- Use `.gitkeep` to preserve empty directories

### Deliverables
- Working public repository
- Reproducible Python environment
- Code quality enforcement on commit
- ADR system in place

### Success Criteria
- A new contributor can clone, install, and run quality checks in under 10 minutes
- Every architectural decision from this point forward is documented

---

## Phase 2: LLM Runtime

**Goal:** Make the local AI layer (Gemma 4 via Ollama) usable across the lab's workflows.

### Step 2.1 — Document Ollama and Gemma 4 setup
- Create `/docs/llm-setup.md`
- Document installation steps for Ollama
- Document Gemma 4 pull command and variant choice
- Record hardware requirements and observed performance
- Document the API endpoint at `localhost:11434`
- Include a verification test prompt

### Step 2.2 — Build the base CLI wrapper
- Python script in `/src` that calls Ollama HTTP API
- Accepts prompt from CLI argument or stdin
- Prints response to stdout
- Handles connection errors gracefully
- Verified working with Gemma 4

### Step 2.3 — Build the context-injection script
- Accepts a query and one or more file paths or globs
- Reads markdown files from `/lab-brain`
- Constructs a prompt with context + query
- Sends to Ollama
- Returns response
- Includes context size limit with warning
- Documented in `/docs/llm-setup.md`

### Step 2.4 — Build the code review utility
- Accepts stdin (e.g., `cat file.py | python src/review.py`)
- Uses a code review system prompt
- Supports git diffs (`git diff | python src/review.py`)
- Output formatted for terminal readability

### Deliverables
- Documented local LLM setup
- Three working AI utilities (general query, context-aware query, code review)

### Success Criteria
- The PI can invoke Gemma 4 from the terminal in under 1 second of typing
- The model can answer questions using lab-specific context

---

## Phase 3: Knowledge Base (`lab-brain`)

**Goal:** Build durable institutional memory accessible to both the PI and the local LLM.

### Step 3.1 — Initialize `lab-brain` structure
```
/lab-brain
  /hypotheses
  /literature-notes
  /project-states
  /decisions-log         (reference to /decisions)
  /datasets-registry
  /contributor-guide
  /weekly-briefings
  /contacts
  /grants
  /_templates
```
- Each subdirectory has a brief `README.md`
- `_templates/` holds markdown templates

### Step 3.2 — Create the hypothesis template
- Fields: title, date, status (proposed/active/tested/archived), research question, background, proposed approach, expected outcome, datasets needed, related literature, open questions
- Machine-parseable structure with consistent headings
- One filled-in example
- Saved at `/lab-brain/_templates/hypothesis.md`

### Step 3.3 — Create the literature note template
- Fields: citation, DOI/URL, date read, summary, key findings, methods, relevance to lab, limitations, bias flags, related hypotheses, tags
- YAML frontmatter for machine parsing
- One filled-in example
- Saved at `/lab-brain/_templates/literature-note.md`

### Step 3.4 — Create the project state template
- Fields: project name, status, objective, current blockers, next actions, key decisions made, contributors involved, related datasets, related hypotheses, timeline
- Saved at `/lab-brain/_templates/project-state.md`

### Step 3.5 — Create the dataset registry template
- Fields: name, description, source, Zenodo DOI, access tier, demographics covered, known limitations, license, date added, related projects
- Saved at `/lab-brain/_templates/dataset-entry.md`

### Step 3.6 — Write the first weekly briefing manually
- Active projects, open questions, recent decisions, contributor activity, literature of interest, weekly priorities
- Date-stamped filename in `/lab-brain/weekly-briefings/`

### Step 3.7 — Build the briefing generator script
- Reads from project states, decisions, recent git activity
- Sends structured prompt to Ollama
- Outputs markdown draft to `/lab-brain/weekly-briefings/`
- PI reviews and edits before committing

### Deliverables
- Structured knowledge base with templates
- One working example of each artifact type
- Automated weekly briefing generation

### Success Criteria
- The PI can re-orient on any active project in under 60 seconds by reading its state document
- Gemma 4 can answer questions using lab-brain content meaningfully

---

## Phase 4: Developer Experience

**Goal:** Make the daily coding environment fast, AI-assisted, and consistent.

### Step 4.1 — Configure VS Code with Continue
- Install Continue extension
- Point Continue to `localhost:11434` and Gemma 4
- Verify tab completion, inline chat, codebase context
- Save settings in `.vscode/settings.json`
- Document in `/docs/editor-setup.md`

### Step 4.2 — Create workspace configuration
- `.vscode/settings.json`: Python path, ruff as formatter and linter
- `.vscode/extensions.json`: recommended extensions
- Documented in README

### Step 4.3 — Install and configure GitHub CLI
- Install `gh` and authenticate
- Verify ability to manage issues, PRs, discussions from terminal
- Document common commands in `/docs/workflows.md`

### Step 4.4 — Set up `direnv`
- Install `direnv`
- Create `.envrc` with `OLLAMA_HOST` and project paths
- Add `.envrc` to `.gitignore`
- Commit `.envrc.example` with placeholder values
- Document in README

### Deliverables
- AI-assisted editor connected to local model
- Terminal-native GitHub workflow
- Project-specific environment auto-loading

### Success Criteria
- The PI's daily coding loop happens entirely in VS Code with Gemma 4 always available
- All GitHub operations can happen from the terminal

---

## Phase 5: Contributor Infrastructure

**Goal:** Enable distributed contributors to participate without requiring synchronous PI time.

### Step 5.1 — Write `CONTRIBUTING.md`
- How to set up the dev environment
- How to find work
- How to submit contributions
- Coding standards
- Welcome contribution types: code, data, docs, research, domain expertise
- Issue label meanings
- Review process and honest timelines
- Attribution policy reference

### Step 5.2 — Write `LAB_MANUAL.md`
- Mission
- Research philosophy
- Domain focus
- Decision-making process
- Attribution norms
- Ethical commitments
- Data principles
- Linked from README

### Step 5.3 — Write `CODE_OF_CONDUCT.md`
- Respectful communication
- Inclusion
- Handling sensitive health topics
- Enforcement process
- Reporting contact
- Linked from README and CONTRIBUTING

### Step 5.4 — Create GitHub issue templates
- `.github/ISSUE_TEMPLATE/`
- Templates: bug report, feature request, hypothesis proposal, dataset suggestion, documentation improvement, general question
- `config.yml` for the chooser

### Step 5.5 — Create pull request template
- `.github/PULL_REQUEST_TEMPLATE.md`
- Fields: description, related issue, contribution type, testing, checklist

### Step 5.6 — Set up labels
- Type labels: `bug`, `feature`, `research`, `data`, `documentation`, `infrastructure`
- Priority: `priority: critical/high/normal/low`
- Experience: `good-first-issue`, `needs-domain-context`, `advanced`
- Status: `needs-triage`, `in-progress`, `blocked`, `help-wanted`
- Domain: `womens-health`, `methods`, `tooling`
- Documented in CONTRIBUTING

### Step 5.7 — Configure GitHub Projects board
- Columns: Backlog, Up Next, In Progress, In Review, Done
- Add existing issues
- Documented in README

### Step 5.8 — Enable GitHub Discussions
- Turn on Discussions
- Categories: Announcements, Research Ideas, Q&A, Show & Tell, General
- Welcome announcement post
- Linked from README and CONTRIBUTING

### Deliverables
- Complete contributor onboarding pathway
- Async-first community infrastructure
- Self-service contribution workflow

### Success Criteria
- A capable stranger can submit a quality contribution within their first week without PI assistance
- Issues, PRs, and discussions are organized and discoverable

---

## Phase 6: Automation

**Goal:** Eliminate repetitive overhead through scripts and CI.

### Step 6.1 — Create a task runner
- `Makefile` or `justfile` in repo root
- Targets: `setup`, `lint`, `format`, `test`, `briefing`, `review`, `clean`
- Documented in README

### Step 6.2 — Build the PDF-to-literature-note pipeline
- Accept PDF file path
- Extract text (basic extraction acceptable initially)
- Send to Ollama with literature note template prompt
- Output draft markdown to `/lab-brain/literature-notes/`
- PI reviews and edits before committing

### Step 6.3 — Build the commit message generator
- Run `git diff --staged`
- Send to Ollama
- Return conventional-commit-style message
- Used as `git commit -m "$(python scripts/commit-msg.py)"`

### Step 6.4 — Set up basic CI
- `.github/workflows/ci.yml`
- Runs ruff lint, format check, tests on push to main and PRs
- Target completion under 2 minutes

### Step 6.5 — Build the lab-brain backup script
- Sync `/lab-brain` to Google Drive or other cloud storage
- Manual or cron-driven
- Logs backup timestamps
- Documented in `/docs/backup.md`

### Deliverables
- Repetitive tasks automated
- CI enforcing code quality
- Knowledge base backed up regularly

### Success Criteria
- The PI rarely repeats the same manual task more than three times before automating it
- Code quality is enforced on every commit and PR

---

## Phase 7: Public Presence

**Goal:** Make the lab discoverable and legible to external collaborators.

### Step 7.1 — Launch GitHub Pages site
- Enable from `/docs` folder or dedicated branch
- Landing page: lab name, mission, research focus, contribution pathway, links to GitHub and Zenodo
- Minimal theme, no custom CSS
- Linked from README

### Step 7.2 — Publish open science manifesto
- Pre-registration commitment
- Open access publishing
- Data sharing principles
- Negative result publication
- Transparent methods
- Community attribution
- Reproducibility standards
- Specific to the women's health domain

### Step 7.3 — Publish research agenda
- Active research questions with brief context
- Questions actively pursued vs. open for contributors
- Linked to hypothesis documents
- Updated as priorities shift

### Deliverables
- Public-facing lab identity
- Stated commitments to open science
- Visible research agenda

### Success Criteria
- A potential collaborator can understand the lab's mission and find a way to engage within five minutes of landing on the site

---

## Phase 8: Governance

**Goal:** Establish minimum legal, ethical, and attribution clarity for sustainable operation.

### Step 8.1 — Establish contributor legal basis
- Choose between DCO (lighter) or full CLA
- Document signing process in CONTRIBUTING
- Record rationale in `/decisions`

### Step 8.2 — Publish attribution policy
- Code contributions
- Data contributions
- Research input
- Documentation
- Community support
- Authorship vs. acknowledgment criteria
- AI-generated contribution handling
- Published in LAB_MANUAL

### Step 8.3 — Publish data governance document
- Access tiers (open / controlled / restricted)
- De-identification standards
- Consent requirements
- Synthetic data policies
- Bias documentation requirements
- Saved at `/docs/data-governance.md`
- Linked from LAB_MANUAL

### Deliverables
- Legal clarity for contributors
- Documented attribution norms
- Documented data ethics standards

### Success Criteria
- Contributors know exactly what they are agreeing to
- Data handling is defensible to ethics reviewers, journal editors, and the community

---

# Part 3: Suggested Build Schedule

A practical 8-week schedule (each week roughly maps to one milestone, but with realistic flex):

| Week | Focus | Outcome |
|---|---|---|
| 1 | Foundation | Repo, license, tooling, structure |
| 2 | LLM Runtime | Local AI working end-to-end |
| 3 | Knowledge Base | `lab-brain` initialized with templates and first briefing |
| 4 | Dev Experience | Editor and terminal optimized for the workflow |
| 5 | Contributor Infrastructure | Community can self-serve |
| 6 | Automation | Repetitive work eliminated |
| 7 | Public Presence | Lab visible to the world |
| 8 | Governance | Legal and ethical clarity in place |

After Week 8, the lab transitions from **building infrastructure** to **doing research with the infrastructure**.

---

# Part 4: Minimum Viable Lab

The lab achieves its first complete operating loop when these are simultaneously true:

1. ✅ Ollama + Gemma 4 running reliably
2. ✅ `lab-brain` initialized with at least one real hypothesis, project state, and literature note
3. ✅ AI-assisted coding working in VS Code
4. ✅ Context-injection script working
5. ✅ Weekly briefing generation working
6. ✅ At least one issue template, PR template, and contributing guide live
7. ✅ Public README clearly stating mission, philosophy, and how to engage
8. ✅ License chosen and applied

That is the version that proves the lab is a real operating system, not a plan.

---

# Part 5: What Success Looks Like

When this lab is operating well:

- **Ideas are captured, not lost.** Every research thought lands in the `lab-brain`.
- **Context compounds.** Each new project benefits from prior projects automatically.
- **The local model is a daily collaborator** — for code, writing, synthesis, and review.
- **Contributors join without friction.** Self-service onboarding works.
- **Outputs flow naturally** to GitHub and Zenodo as part of the workflow, not as a separate effort.
- **The PI's attention is protected.** The system absorbs coordination overhead.
- **Trust is earned through transparency.** The lab's public infrastructure is its credibility.
- **The lab can grow** without becoming administratively heavy — scale comes from community and AI, not headcount.

---

# Part 6: One Guiding Principle

> *Build the smallest possible system that can do real research today, then let it grow only in response to actual pain — never in anticipation of imagined complexity.*
