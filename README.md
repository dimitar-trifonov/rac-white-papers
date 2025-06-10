# Requirements-as-Code (RaC) White Papers

This repository contains a growing collection of **practically grounded white papers** that define and explore the **Requirements-as-Code (RaC)** approach — a structured, declarative, and tech-agnostic method for improving software development in the age of Large Language Models (LLMs).

## 💡 What Is RaC?

**RaC** emerged from hands-on experience building AI-assisted software and discovering the limitations of pure prompt-based workflows. It introduces an **extra abstraction layer** that improves collaboration, traceability, and reliability when working with LLMs to create real-world applications.

 > _Think of RaC as if it is a recipe that helps the LLM cook your app._

Rather than being the result of a research grant or academic initiative, these white papers capture real developer insights — refined into a reusable framework.

---

## 📄 Papers Included

| White Paper # | Title                                   | Description |
|---------------|-----------------------------------------|-------------|
| 1             | `RaC Foundation`                        | Defines the RaC approach, its file structure, logic model, and practical benefits. |
| -             | `get-started.md`                        | System prompt for starting a RaC project in Bolt.new or Cursor with ready folder structure. |
| *(Upcoming)*  | `RaC for Business Systems`              | How RaC can structure workflows, roles, and non-code processes. |
| *(Upcoming)*  | `RaC and Self-Evolving Systems`         | Vision paper for reflexive systems, RaC-as-a-Service, and agent-augmented logic editing. |

---

## 📂 Structure

```bash
.
├── 01-rac-foundation.md
├── get-started.md
├── 02-business-systems.md         # (planned)
├── 03-self-evolving-systems.md    # (planned)
├── LICENSE
└── README.md
```

Each `.md` file is a standalone white paper meant to be read in full or referenced modularly.

---

## 🚀 Who This Is For

These papers are designed for:

- Developers and builders using LLMs in real-world workflows
- Product teams exploring AI-native prototyping methods
- Designers and PMs looking for structured ways to communicate logic
- Toolmakers building the next generation of AI-coding platforms

---

## ⚡ Quick Start

To begin using RaC in **Bolt.new**, **Cursor**, or any LLM-based IDE:

1. Open your project folder in the tool.
2. Create a `rac` folder inside your project.
3. Paste the `get-started.md` file into the `rac` folder.
4. Ask the LLM to assist you with building your specific app.

📌 **Example First Prompt**:

```
Could you help me to build a cooking recipe catalog app, following instructions in the rac folder?
```

The LLM will guide you through collecting requirements and generating `.rac.yaml` files for:

- `state/`
- `events/`
- `logic/`
- `ui/`
- `tests/`
- `bindings/`

✅ Once your requirements are structured as RaC files, **ask the AI IDE to build your app** — using the declarative logic you've defined.

---

### 🧠 Best Practices

1. **Build the app incrementally.**
2. If the app includes a UI, **start with a design system**:
   - Prompt: `"Build a design system for my app and show it in a Design System page."`
3. Then build the app **page by page**, e.g.:
   - Prompt: `"Build the app home page."`

For more structure and reusable guidance, see: [get-started.md](./get-started.md)

---

## 🔄 Related Repositories (planned)

---

## 📜 License

MIT License — open to all, attribution appreciated.

---

> _“RaC is not about replacing developers — it’s about making software feel more like dialogue and less like translation.”_
