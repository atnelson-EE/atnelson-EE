# Alex Nelson, PE

I'm a licensed electrical engineer building rule-driven automation for
commercial design workflows. My background is in commercial building
electrical design -- hotels, restaurants, offices, and mixed-use projects.

I am also building software to automate the repetitive, rule-following parts
of that work -- grounded in code requirements, not just professional habit.

## Lead Project: Ani-Revit2

**Ani-Revit2** is a C#/.NET 10 Revit add-in that automates circuit assignment
and panel-driven load grouping inside Revit 2025/2026. It applies structured
engineering rules during the design process -- not as a post-design check, but
inside the live model where the work happens.

The core logic is Revit-free and testable. Circuit assignment strategies are
explicit, configurable objects that can be inspected and traced back to the
engineering requirements they implement.

### Demo

<!-- Demo video will be added here -->
_A demo video is in progress showing rule-driven auto-circuiting and panel
assignment running inside a live Revit model. The system is functional today --
a live walkthrough or deeper demo is available on request._

## Deeper Foundation: ani-digital-twin-engine

Building the Revit prototype clarified something important: encoding rule logic
from professional experience alone was useful for prototyping, but not sufficient
for a system that needs to be repeatable, auditable, and traceable back to code
requirements.

**ani-digital-twin-engine** is that foundation -- a deterministic NEC/IBC
calculation and knowledge engine, structured code library, and data ingest pipeline.
Every calculation traces to a specific code section. No ML inference in the
engineering path. The system includes a self-assessing validation layer that
classifies its own data surfaces by trust status and explicitly labels what it
has not verified.

## How the Pieces Fit Together

```
Project / Building Inputs
        |
        v
Spatial + Program Understanding
        |
        v
Deterministic Rule + Calculation Layer
        |
        v
Revit-Side Workflow Automation
        |
        v
Governance / Standards / Reviewability
```

- **Ani-Revit2** -- visible Revit-side workflow automation (the application layer)
- **ani-digital-twin-engine** -- deterministic, code-referenced logic and calculations (the foundation layer)
- **ANI-Standards** -- governance, conventions, and shared skills (the coordination layer)
- Supporting repos handle spatial reasoning, project-grounded test cases, and earlier calculation prototypes

Components exist at each layer. Some are mature and demonstrable; others are
architecturally defined and partially built. The full pipeline is directional,
not fully connected end-to-end.

That broader direction matters because the same approach can support practical,
bounded automation inside engineering firms.

## Business Applications

This work is oriented toward practical problems in engineering firms:

- **Revit/API workflow assistants** -- automating repetitive modeling, circuiting, and labeling tasks inside the design tool
- **Electrical rule/calculation assistants** -- bounded, code-referenced support for load calculations, branch circuit sizing, and panel scheduling
- **Documentation/process assistants** -- structured support for proposals, submittal prep, and repetitive engineering documentation
- **Review/QA assistants** -- helping organize and prioritize the review process without replacing professional judgment

The goal is not autonomous engineering. It is specialized, bounded workflow
support for repetitive and reviewable tasks -- where the engineer stays in
control and the system stays traceable.

## How It Gets Built

AI agents assist in developing and maintaining this software, but they operate
under explicit constraints -- and a human PE retains authority over all
engineering decisions. The AI builds the tooling. Engineering judgment stays
human.

What is different here is the combination: engineering domain expertise,
deterministic rule logic traceable to building codes, and a governed
AI-assisted development workflow -- applied to a real licensed-professional
domain, not just a software demo.

## Background

- Licensed Professional Engineer (Electrical)
- Revit MEP, NEC analysis, electrical system design
- Building with C#, .NET, Python, and AI-assisted development workflows
- R&D informed by real project documentation and engineering complexity

Selected demos, walkthroughs, and architecture discussions are available on request.
Repositories are private during active development.

[LinkedIn](https://www.linkedin.com/in/alex-nelson-ee/) | alex@ani-labs.org

_Profile last updated: April 2026_
