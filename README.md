# Alex Nelson, PE
Licensed Electrical Engineer | Revit Automation | Code-Referenced Electrical Design

I design electrical systems for commercial buildings: power distribution, lighting, branch circuits, panel schedules, feeder sizing, and service sizing.

I am also building software to automate parts of that work.

My current demo focus is **Ani.Revit2** — a C#/.NET 8 Revit add-in built around the Revit 2025/2026 API generation. It currently demonstrates panel-driven grouping, automatic circuit assignment, and circuit label naming inside Revit.

Building that prototype clarified something important: I was starting to build a rule engine from engineering experience alone. That was useful for prototyping, but not good enough for a system that needs to be repeatable, auditable, and traceable back to code requirements.

So I stepped back and rebuilt the foundation from the source material itself — starting with the **NEC** and **IBC**, then structuring requirements into deterministic data and rule records. The goal is to design the logic from the ground up, then connect it back into Revit and production workflows.

## Current Focus

- **Ani.Revit2** — Revit integration prototype for grouping, circuiting, labeling, and structured electrical data exchange
- **ani-digital-twin-engine** — code library, ingest pipeline, and deterministic electrical calculation framework
- **ani-spatial-engine** — spatial and occupancy classification layer for mapping room and building data to electrical requirements
- **ANI-Standards** — cross-repo contracts, validation rules, manifests, and governance
- **ani-load-estimator** — earlier NEC load-calculation prototype and validation engine

## Why This Matters

Commercial electrical design still depends heavily on manual interpretation, spreadsheet logic, and office-specific conventions. I am working toward systems where outputs are faster to produce, easier to review, and traceable back to the governing code section, edition, and assumption.

## Background

- Licensed Professional Engineer
- Commercial building design: hotels, restaurants, offices, mixed-use
- Revit MEP, NEC analysis, electrical system design
- Building with C#, .NET, Python, and AI-assisted development workflows

Selected demos and architecture discussions are available on request.
Some repositories remain private during active development.



[LinkedIn](https://www.linkedin.com/in/alex-nelson-ee/) | atnelson1103@gmail.com

_Profile last updated: April 2026_
