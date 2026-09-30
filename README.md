# Lily Florist AI Project

Requirements engineering and UX documentation for **Lily Florist**, an AI-assisted
e-commerce florist application.

| | |
| --- | --- |
| **Author** | Jonathan Bruno Silva ([jonabsilva](https://github.com/jonabsilva)) |
| **Institution** | [Quantic School of Business and Technology](https://quantic.edu/) |
| **Degree** | Master of Science in AI Engineering (MSAIE) |
| **Course** | Managing AI Engineering (MSAIE75+) |
| **Project** | *Meeting Customer Requirements* |

---

## About this repository

This repository is the public documentation record of the project. It holds the
requirements, UX and design artefacts, plus the final deliverable report.

Anyone is welcome to read and view everything here. The repository is open for
viewing; contributions are welcome via issues and pull requests.

---

## The project

The brief: conduct a one-on-one requirements-gathering interview with a potential
client, then work the elicited needs through the full requirements engineering
chain. For this project the client is **Lily**, the proprietor of *Lily's Florist
Shop*.

**Client context.** Lily's Florist Shop is handling growing order volume and needs a
website that supports both customer ordering and inventory management. She also wants
generative AI woven into the site to provide customer support around the clock, rather
than only during opening hours. The discovery interview focused on customer pain points,
her goals for the AI-enabled site, and ambiguity to be eliminated — covering both the
happy path and divergent paths, dead ends and failure cases.

**Scope of work.**

| Stage | Output |
| --- | --- |
| Requirements gathering | 1:1 discovery interview with the client |
| User stories | 15+ stories, spanning multiple user types, including AI-enabled support |
| User journey | Persona, scenario, and step-by-step interactions for a selected goal |
| Requirements | 20+ numbered requirements — functional and non-functional — traceable to the source stories |
| Design | Figma wireframes of the user journey, annotated with design rationale and requirement traceability |

The emphasis is on turning ambiguous customer intent into requirements that are
unambiguous, quantifiable, categorised, and verifiable — since poorly specified
requirements are a leading cause of project failure.

**Requirements gathering record:**
[Interview with Lily — 24 September 2026](https://chatgpt.com/share/6ab583cf-a810-83eb-987c-9f6593724535)

---

## Repository structure

```
lilys-florist/
│
├── README.md
│
├── deliverables/
│   └── Lily_Florist_AI_Project_FINAL.pdf     # Final project report
│
├── docs/
│   ├── requirements/
│   │   ├── user-stories.md                   # User stories and personas
│   │   ├── functional-requirements.md        # Functional requirements
│   │   ├── non-functional-requirements.md    # Non-functional requirements
│   │   └── traceability-matrix.xlsx          # Traceability matrix
│   │
│   ├── ux/
│   │   └── user-journey.md                   # User journey map
│   │
│   └── design/
│       └── annotated-screens/                # Annotated UI screens
│           ├── 01-home-annotated.png
│           ├── 02-product-search-annotated.png
│           ├── 03-ai-assistant-annotated.png
│           ├── 04-product-details-annotated.png
│           ├── 05-cart-annotated.png
│           ├── 06-checkout-annotated.png
│           └── 07-confirmation-annotated.png
│
└── assets/                                   # Supporting visual assets
```

---

## Documentation map

### Requirements

| Document | Contents |
| --- | --- |
| [`user-stories.md`](docs/requirements/user-stories.md) | 30 user stories (US-01 – US-30) across 7 user roles |
| [`functional-requirements.md`](docs/requirements/functional-requirements.md) | 27 functional requirements (FR-01 – FR-27) |
| [`non-functional-requirements.md`](docs/requirements/non-functional-requirements.md) | 8 non-functional requirements (NFR-01 – NFR-08) |
| [`traceability-matrix.xlsx`](docs/requirements/traceability-matrix.xlsx) | Traceability from requirements back to user stories |

### UX

| Document | Contents |
| --- | --- |
| [`user-journey.md`](docs/ux/user-journey.md) | Persona, scenario, happy path, 3 alternative paths, 3 failure scenarios, AI interaction points |

### Design

| Screen | File |
| --- | --- |
| Home | [`01-home-annotated.png`](docs/design/annotated-screens/01-home-annotated.png) |
| Product search | [`02-product-search-annotated.png`](docs/design/annotated-screens/02-product-search-annotated.png) |
| AI assistant | [`03-ai-assistant-annotated.png`](docs/design/annotated-screens/03-ai-assistant-annotated.png) |
| Product details | [`04-product-details-annotated.png`](docs/design/annotated-screens/04-product-details-annotated.png) |
| Cart | [`05-cart-annotated.png`](docs/design/annotated-screens/05-cart-annotated.png) |
| Checkout | [`06-checkout-annotated.png`](docs/design/annotated-screens/06-checkout-annotated.png) |
| Confirmation | [`07-confirmation-annotated.png`](docs/design/annotated-screens/07-confirmation-annotated.png) |

---

## Deliverable

| Document | Location |
| --- | --- |
| Final project report (PDF) | [`deliverables/Lily_Florist_AI_Project_FINAL.pdf`](deliverables/Lily_Florist_AI_Project_FINAL.pdf) |

---

## Status

Complete. Requirements, user journey, traceability matrix, annotated wireframes and
the final report are all included.

---

## Notes

The `.docx` originals are preserved in the local working copy; the documents here are
Markdown conversions. Previous document versions are kept outside this repository in a
local archive folder.

---

## Course reference

Managing AI Engineering, Quantic School of Business and Technology — project brief
*"Meeting Customer Requirements"* (MSAIE75+). The brief is summarised above in the
author's own words.

