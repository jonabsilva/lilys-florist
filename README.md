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

## Traceability

Everything in this repository hangs off one chain. Each link is verifiable, so no
requirement exists without a customer need behind it and no screen exists without a
requirement behind it.

```
Lily (interview)
   └─► User story        US-01 … US-30
          └─► Requirement   FR-01 … FR-27  ·  NFR-01 … NFR-08
                 └─► Screen   01-home … 07-confirmation
```

- **Interview → stories.** Every story traces to something Lily raised. No requirement
  was invented beyond what the interview supported.
- **Story → requirement.** The mapping is held in
  [`traceability-matrix.xlsx`](docs/requirements/traceability-matrix.xlsx), which also
  records requirement type and the screen each one is realised in.
- **Requirement → screen.** Each annotated screen cites the requirements it addresses,
  so the design is auditable against the specification.

**Coverage.** All 30 user stories map to at least one requirement and to a screen — no
story is orphaned. All 27 functional requirements appear in the matrix.

Two non-functional requirements are also mapped to specific stories: **NFR-05**
(authentication and role-based access) and **NFR-06** (privacy and data protection).
The remaining six — NFR-01 to NFR-04 (performance and consistency) and NFR-07 to NFR-08
(accessibility, hosting and backups) — are system-level constraints rather than outcomes
of any single user story, so they are specified without a story parent.

Eight open questions from the interview were carried forward and deliberately left
unresolved rather than assigned invented values. Where they affect a requirement, that
requirement states the gap explicitly — see NFR-08, where backup frequency, retention and
recovery targets remain open.

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

## Requirements coverage

A self-assessment against the project rubric, pointing to where each criterion is
evidenced.

| Criterion | Evidence |
| --- | --- |
| 15+ user stories | 30 stories, US-01 – US-30 — [`user-stories.md`](docs/requirements/user-stories.md) |
| Multiple user types | 7 roles: Guest, Returning Customer, Customer, AI Support, Staff, Manager, Owner/Admin |
| AI-related user stories | US-11 – US-15 — AI Q&A, recommendations, cart assistance, bilingual EN/IE, escalation to staff |
| User journey | Persona, scenario, goal, 11-step happy path — [`user-journey.md`](docs/ux/user-journey.md) |
| Alternative and error paths | 3 alternative paths + 3 failure scenarios (payment failure, unconfirmed status, failed delivery) |
| 20+ requirements | 35 total: FR-01 – FR-27 and NFR-01 – NFR-08 |
| Functional requirements | [`functional-requirements.md`](docs/requirements/functional-requirements.md) |
| Non-functional requirements | [`non-functional-requirements.md`](docs/requirements/non-functional-requirements.md) |
| Numbered and categorised | Every requirement carries an ID and a functional/non-functional classification |
| Quantifiable / testable | NFR-01 ≈2s page load, NFR-02 ≈3s checkout, NFR-03 100+ orders/day, NFR-05 lockout after failed attempts |
| Traceability | [`traceability-matrix.xlsx`](docs/requirements/traceability-matrix.xlsx) — US → FR/NFR → screen |
| Mockups / wireframes | 7 annotated screens — [`annotated-screens/`](docs/design/annotated-screens/) |
| Annotations with design rationale | Each screen annotates its elements and cites the requirements they satisfy |
| AI-enabled customer support in requirements | FR-11 – FR-16 |
| Final document ≥ 4 pages | [`Lily_Florist_AI_Project_FINAL.pdf`](deliverables/Lily_Florist_AI_Project_FINAL.pdf) |
| Interview link | [Interview with Lily — 24 September 2026](https://chatgpt.com/share/6ab583cf-a810-83eb-987c-9f6593724535) |

**On story count.** The brief asks for 15+. This project documents 30. The extra
stories exist to keep traceability for functional findings from the interview that
would otherwise have been merged or lost — splitting them keeps each independently
actionable and individually traceable. Coverage and rationale are recorded in
[`user-stories.md`](docs/requirements/user-stories.md).

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

