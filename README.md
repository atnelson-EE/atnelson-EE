# Alex Nelson, PE

**Licensed Electrical Engineer | Building Automation & AI-Driven Design**

I design electrical systems for commercial buildings -- power distribution, lighting, branch circuits, panel schedules, service sizing. The kind of work that keeps the lights on (literally).

I'm also building the tools to automate it.

---

## What I'm Working On

I'm developing an open research platform that applies AI and deterministic rule engines to commercial electrical engineering design. The goal: take a building's occupancy type, square footage, and room schedule, and produce code-compliant electrical calculations -- automatically.

### The Problem

Electrical load calculations for commercial buildings are manual, repetitive, and error-prone. Every engineer does them slightly differently. The NEC (National Electrical Code) is 1,000+ pages of rules, tables, and exceptions that interact in complex ways. A single hotel project requires cross-referencing dozens of articles, applying demand factors from multiple tables, and sizing everything from branch circuits to the main service entrance.

This work hasn't changed in decades. I think it should.

### What I've Built

**NEC Compliance Engine** -- A deterministic calculation engine that reads structured NEC rule data and produces compliant electrical designs. Currently targeting Article 220 (load calculations) for hotel/motel occupancy types.

Sample output from a 30,000 sqft hotel test case:

```
ELECTRICAL DESIGN SUMMARY
Building: Test Hotel - Scottsdale
Occupancy: hotel_motel | Area: 30,201 sqft

SERVICE LOAD CALCULATION (NEC Article 220)
  General Lighting                     27,671 VA
  Receptacles (non-guest)               8,280 VA
  Kitchen Equipment                    22,100 VA
  HVAC - Heating (per 220.60)        162,000 VA
  Elevator                             25,000 VA
  Water Heating                        67,500 VA
  Equipment                           130,818 VA
  ----------------------------------------
  Total Demand                        443,869 VA
  Service Size: 1200A, 480/277V, 3-phase
```

**NEC Reference Data Pipeline** -- Structured, machine-readable versions of NEC 2020, 2023, and 2026. Three-stage pipeline: raw text extraction, cleaning, and transformation into deterministic rule records. Covers 600+ articles across three editions.

**Revit Integration Prototype** -- A C# add-in for Autodesk Revit (2025/2026) that reads electrical family data and interfaces with the compliance engine. Working demo for automated circuit assignment.

**Spatial Classification Engine** -- Maps building spaces to NEC occupancy types and electrical requirements. Given a room schedule, determines which NEC articles, demand factors, and circuit rules apply to each space.

### Architecture

```
Building Input (rooms, equipment, sqft)
         |
         v
  Spatial Engine -----> Occupancy classification
         |
         v
  Load Estimator -----> NEC Article 220 calculations
         |                  + demand factors
         v                  + circuit sizing
  Compliance Engine --> Code-compliant design output
         |
         v
  Revit Add-In ------> BIM model integration
```

All backed by a structured NEC reference library covering three editions (2020, 2023, 2026) plus IBC, IECC, and IgCC building codes.

---

## Background

- PE (Electrical) -- licensed professional engineer
- Commercial building design -- hotels, restaurants, offices, mixed-use
- Proficient in Revit MEP, NEC code analysis, electrical system design
- Building with: Python, C#/.NET, Claude Code, multi-agent AI workflows

---

## Why This Matters

The AEC (Architecture, Engineering, Construction) industry is one of the least digitized sectors in the economy. Most electrical engineers still do load calculations by hand or in spreadsheets with no traceability back to the code sections that govern them.

Deterministic, code-referenced electrical design isn't just faster -- it's auditable. Every number in the output traces back to a specific NEC article, table, and edition. That matters for plan review, for liability, and for the profession.

I'm one engineer building this in the open. If you're interested in the intersection of AI, building codes, and electrical engineering -- I'd like to talk.

---

*Repositories are private during active development. Reach out for access or demos.*

[LinkedIn](https://www.linkedin.com/in/alex-nelson-ee/) | atnelson1103@gmail.com

*Profile last updated: April 2026*
