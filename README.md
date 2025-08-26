# Awesome Prompt Structure  
> The most authoritative, curated collection of **prompt structuring languages**, **frameworks**, and **tooling** for modern prompt engineering.  
_Last updated: 2025-08-26_

---

## 🚀 Quick Start
1. Pick a **language** or **markup** that fits your stack (see table below).  
2. Combine with a **framework** (CLEAR, CARE, R.O.A.D., etc.) for human clarity.  
3. Use the **tooling** section to test, trace, and deploy at scale.

---

## 📚 Prompt Languages & Markups

| # | Name / Spec | One-line pitch | Core syntax | Parallel / control flow | Modularity | Tooling & debugging | Audience | License |
|---|---|---|---|---|---|---|---|---|
| 0 | **Plain Prompt** (baseline) | Raw string into chat box | Free-form text | None | Copy-paste | Chat history | Everyone | n/a |
| 1 | **(: Smile** | Human-readable emoticon brackets (`(:`, `[=` …) for concise prompts | 5–6 tokens | None | Copy-paste | Human eyeballs | Non-coders, prompt engineers | [MIT](https://github.com/DrThomasAger/smile) |
| 2 | **APPL** | Python-native DSL (`@ppl`, `gen()`) turning prompts into code | Python decorators & classes | **Automatic** async | Python imports, unit tests | Full Python IDE | Python developers | [MIT](https://github.com/thunlp/APPL) |
| 3 | **POML** | “HTML of prompts” – XML tags + CSS for LLM workflows | `<role>` `<task>` … | External orchestration | `<include>`+SDK | VS Code ext, SDKs | Teams outgrowing plain text | [MIT](https://github.com/microsoft/poml-lang) |
| 4 | **PromptML** | YAML-like DSL for multi-turn, tool-calling prompts | YAML front-matter + Markdown | Built-in `loop`, `if` | YAML anchors, `extends` | CLI linter, VS Code ext | DevOps / AI-ops engineers | [Apache-2.0](https://github.com/IBM/promptml) |
| 5 | **DSPy** | “PyTorch for prompts” – declarative modules compiled to optimal prompts | Python signatures + optimizers | Compiled graph; implicit parallel | Modules, optimizers, metrics | PyTorch-style debugging | Researchers & production teams | [MIT](https://github.com/stanfordnlp/dspy) |
| 6 | **Guidance** | Handlebars-like templating with built-in control flow | `{{gen}}`, `{{select}}` | `{{each}}`, `{{if}}` | Partials, imports | Jupyter widgets | Data scientists | [MIT](https://github.com/guidance-ai/guidance) |
| 7 | **LMQL** | SQL-like declarative constraints on LLM outputs | `SELECT` / `FROM` / `WHERE` | Implicit batching | Functions, constraints | VS Code ext, debugger | PL researchers | [MIT](https://github.com/eth-sri/lmql) |

---

## 🧩 Frameworks for Writing Prompts

| Framework | Acronym | Best for | Source |
|---|---|---|---|
| **CLEAR** | Concise, Logical, Explicit, Adaptive, Reflective | General prompt clarity | [UC Davis Library](https://guides.library.ucdavis.edu/genai/prompt) [^17^] |
| **CARE** | Context, Action, Result, Example | Marketing & copy | [ButterCMS](https://buttercms.com/blog/chatgpt-prompt-frameworks/) [^19^] |
| **D.A.R.E.** | Describe, Act, Resonate, Elevate | Creative storytelling | [LinkedIn](https://www.linkedin.com/pulse/mastering-ai-prompt-engineering-six-frameworks-marketers-scott-fiesel-mqmpe) [^13^] |
| **R.O.A.D.** | Recognize, Options, Analyze, Decide | Decision making & strategy | [LinkedIn](https://www.linkedin.com/pulse/mastering-ai-prompt-engineering-six-frameworks-marketers-scott-fiesel-mqmpe) [^13^] |
| **PAR** | Problem, Action, Result | Straightforward problem solving | [ButterCMS](https://buttercms.com/blog/chatgpt-prompt-frameworks/) [^19^] |

---

## 🛠️ Tooling & Debugging Ecosystem

| Category | Tool / Library | Highlights | Link |
|---|---|---|---|
| **IDE & Linters** | VS Code Prompt-Dev Extension Pack | Syntax for POML, PromptML, Smile | VS Code Marketplace |
| **Tracing & Eval** | LangSmith | Deep trace of LangChain runs, eval datasets | [langchain.com/langsmith](https://langchain.com/langsmith) [^14^] |
| **Tracing & Eval** | Maxim AI | Versioning, A/B, human + auto eval for agents | [maximai.io](https://maximai.io) [^14^] |
| **Experiment Tracking** | Weights & Biases Prompts | Track prompt + param combos, dashboards | [wandb.ai](https://wandb.ai) |
| **Open-source CLI** | PromptTools | Local benchmarking, regression tests | [prompttools.readthedocs.io](https://prompttools.readthedocs.io) [^14^] |
| **Visual Debugging** | LIT (Google) | Attention heatmaps, token salience | [ai.google.dev/responsible/docs/alignment/lit](https://ai.google.dev/responsible/docs/alignment/lit) [^15^] |
| **Token Analytics** | tiktoken | Precise GPT token counting | [openai/tiktoken](https://github.com/openai/tiktoken) |
| **Playgrounds** | OpenAI Playground | Interactive temp, top-p, max-tokens sliders | [platform.openai.com/playground](https://platform.openai.com/playground) |
| **Low-code Flow** | Flowise | Drag-and-drop prompt chains & agents | [flowiseai.com](https://flowiseai.com) [^14^] |

---

## 🗂️ Repository Layout


awesome-prompt-structure/
├── README.md                 ← you are here
├── languages/                ← specs & examples for each language
│   ├── (:smile.md
│   ├── appl.md
│   ├── poml.md
│   ├── promptml.md
│   ├── dspy.md
│   ├── guidance.md
│   └── lmql.md
├── frameworks/               ← prompt writing frameworks
├── tools/                    ← tool-specific docs & install guides
└── examples/                 ← runnable demos

---

## 🤝 Contributing

We follow the [Awesome Manifesto](https://awesome.re).  
Please open **issues** for typos or outdated links, and **pull requests** for new languages, frameworks, or tools.

---

## 📄 License

This list is released under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/).  
Individual projects retain their own licenses (see table).

