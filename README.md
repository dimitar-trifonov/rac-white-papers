# Requirements-as-Code (RaC) White Papers

This repository contains a growing collection of **practically grounded white papers** and supporting files for the **Requirements-as-Code (RaC)** approach — a structured, declarative, and tech-agnostic method for improving software development in the age of Large Language Models (LLMs).

---

## 💡 What Is RaC?

**RaC** introduces an intermediate design layer between intent and implementation. Instead of scattering specifications across documents, UI mockups, code comments, and test cases, RaC consolidates them into a **single structured source of truth** — powered by `.rac.yaml` files.

> _Think of RaC as a recipe that helps the LLM cook your app._

This approach improves:
- Traceability across stakeholders
- Modularity and simulation before coding
- Safe, auditable, tech-agnostic logic reuse

---

## 📄 White Papers

| White Paper # | Title                        | Description |
|---------------|------------------------------|-------------|
| 1             | `01-rac-foundation.md`       | Defines the RaC folder structure, schema logic, lifecycle integration, and its power as an LLM bridge. |
| -             | `rac/get-started.md`         | A system prompt and starter guide to kick off RaC-based development inside Bolt.new, Cursor, or any AI IDE. |
| *(Upcoming)*  | `02-business-systems.md`     | Using RaC to structure enterprise workflows, roles, and processes. |
| *(Upcoming)*  | `03-self-evolving-systems.md`| Vision paper for reflexive RaC logic, hosted agents, and RaC-as-a-Service. |

---

## 📂 Repository Structure

```bash
.
├── 01-rac-foundation.md
├── rac/
│   ├── get-started.md
│   ├── schemas/
│   │   ├── state.schema.rac.yaml
│   │   ├── event.schema.rac.yaml
│   │   ├── logic.schema.rac.yaml
│   │   ├── test.schema.rac.yaml
│   │   ├── ui.schema.rac.yaml
│   │   └── schema-manifest.rac.yaml
├── 02-business-systems.md         # (planned)
├── 03-self-evolving-systems.md    # (planned)
├── LICENSE
└── README.md
```

Each `.md` file is a standalone white paper.  
The `rac/` folder contains schema definitions, templates, and documentation for building RaC systems.

---

## 🚀 Who Is This For?

- Developers using LLMs to scaffold and test apps
- Product teams building AI-native tools
- Designers and PMs seeking executable logic specs
- Teams tired of syncing docs, diagrams, and code

---

## ⚡ Quick Start

To begin using RaC:

1. Clone this repo and explore the `rac/` folder
2. Open `rac/get-started.md` inside **Bolt.new**, **Cursor**, or your AI IDE
3. Paste your goal as a prompt, e.g.:

```
Could you help me build a peer feedback platform using the RaC folder as my design blueprint?
```

The AI will assist in generating:
- `state/` – core data structures
- `events/` (or `services/`) – user/system actions
- `logic/` – validation and business rules
- `ui/` or `api/` – interface definitions
- `tests/` – simulation of user/system behavior
- `bindings/` – optional tech-specific generators

✅ Once your `.rac.yaml` files are valid and connected, ask the LLM to scaffold the actual app.

---

## 🧠 Blueprinting Your Business Logic

RaC supports domain-specific extensions. Each business has its own logic — RaC helps you define it by answering:

| Question                            | Goes in...     |
|-------------------------------------|----------------|
| What do we manage?                  | `state/`       |
| What can users or systems do?       | `events/` or `services/` |
| What must be true or forbidden?     | `logic/`       |
| What should be visible or exposed?  | `ui/` or `api/`|
| What should be simulated or tested? | `tests/`       |

See [`rac/get-started.md`](./rac/get-started.md) for more guidance.

---

## 🔗 Related Repositories

1. [Motion Handled Music Player](https://github.com/dimitar-trifonov/motion-music-player-rac)
   - A RaC implementation of a music player controlled by device motion sensors

---

## 📜 License

MIT License — open to all, attribution appreciated.

---

> _"RaC is not about replacing developers — it's about making software feel more like dialogue and less like translation."_

