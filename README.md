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

## ⚙️ RaC, LangChain & GenKit – Ops in the LLM Ecosystem

RaC isn't a competitor—it's the **declarative logic layer** that complements both prompt‑orchestration and production feature execution frameworks:

| Ops Type     | Focus                                  | Key Tools                 | RaC's Role                                          |
|--------------|----------------------------------------|---------------------------|-----------------------------------------------------|
| **PromptOps** | Prompt chaining, agents, memory       | LangChain                 | Implements RaC‑defined logic flow in agents         |
| **FeatureOps** | AI feature development and deployment | GenKit (Firebase GenKit) | Executes RaC‑defined flows in production, with observability & deployment support |
| **LogicOps**  | Structured spec: events, logic, state | **RaC (Requirements-as-Code)** | Formalizes "what" the app must do, validated by schema and tests |

### 🔄 Combined Flow Example

1. **Define** in RaC:
   - `events/order.create`
   - `logic/order.validate`
   - `tests/order-flow.test.rac.yaml`

2. **Execute**:
   - **LangChain** for conversational prompts (e.g. customer queries)
   - **GenKit** to deploy order‑processing flows with monitoring and UI

3. **Validate**:
   - RaC ensures logic correctness across flows before deployment

### 💼 Why This Matters

In the LLM era, teams need **deterministic business logic** that survives prompt changes and model updates. RaC provides the missing "source of truth" that keeps your core business rules consistent across:
- Different AI models and prompts
- Multiple deployment environments
- Team handoffs and documentation
- Regulatory compliance requirements

By positioning:
- **LangChain** as **PromptOps** (dynamic prompt-based logic),
- **GenKit** as **FeatureOps** (end-to-end AI feature deployment),
- **RaC** as **LogicOps** (formal spec + deterministic logic),

you show that RaC fills a critical gap: the **structured, testable logic layer** essential for robust LLM-driven systems.

---

## ⚡ Quick Start

To begin using RaC:

1. **Add the `rac/` folder** from this repository into a new project in your preferred AI IDE
2. **Open dialog with the LLM** and introduce your idea
3. **Define scope collaboratively** with the AI to establish project boundaries
4. **Ask LLM to generate a `reqs.md` file** for functional and non-functional requirements
5. **Request a project plan** using `rac/get-started.md`, store it as `plan.md`
6. **Build `.rac.yaml` structure** guided by the plan, creating:
   - `state/` – core data structures
   - `events/` (or `services/`) – user/system actions
   - `logic/` – validation and business rules
   - `ui/` or `api/` – interface definitions
   - `tests/` – simulation of user/system behavior
   - `bindings/` – optional tech-specific generators
7. **Ask LLM regularly to verify schema correctness** of the generated files

✅ Once your `.rac.yaml` files are valid and connected, ask the LLM to scaffold the actual app.

**Example prompt to start:**
```
Could you help me build an employee onboarding system using the RaC folder as my design blueprint?
```

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

