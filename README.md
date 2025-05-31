# awesome-dify-agents
> A community-curated collection of **Dify** chatflows, agent workflows, and DSL templates – all in handy `.yml` files.

[![Stars](https://img.shields.io/github/stars/shamspias/awesome-dify-agents?style=social)](https://github.com/shamspias/awesome-dify-agents/stargazers)
[![License](https://img.shields.io/github/license/shamspias/awesome-dify-agents)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## What is Dify?

[Dify](https://github.com/langgenius/dify) is an open-source LLM application platform that combines **agentic workflows, RAG pipelines, model management, and observability** in one UI/SDK, letting you go from prototype to production fast. :contentReference[oaicite:0]{index=0}  
Its **DSL** (a YAML-based standard) lets you export or import entire app configurations, including prompts, nodes, and model parameters. :contentReference[oaicite:1]{index=1}

---

## Purpose of this repository

1. **Preserve**: Back up interesting chatflows & workflows in version control.  
2. **Discover**: Browse ready-made agents, RAG examples, tool integrations, and UI tweaks.  
3. **Learn**: Compare design patterns, node chains, and prompt engineering tricks.  
4. **Reuse**: Fork, import, and adapt flows into your own Dify instance in seconds.

---

## Directory structure

```

flows/
├─ agents/          # autonomous or multi-agent examples
├─ chatbots/        # conversational flows
├─ rag/             # retrieval-augmented generation setups
├─ integrations/    # 3rd-party API or plugin demos
└─ utilities/       # helper nodes, memory tools, etc.

```

Each sub-folder contains one or more `*.yml` DSL files plus a short `README` describing:

* **Goal** – what the flow does  
* **Models tested** – e.g. GPT-4o, Claude 3, Gemini 1.5  
* **Special nodes** – file upload, call-function, eval, etc.  
* **Screenshot / diagram** (optional)  

---

## Quick start

1. **Clone** this repo or download only the flow you need.  
2. In your Dify dashboard choose **⋯ › Import DSL file** and select the `.yml`. :contentReference[oaicite:2]{index=2}  
3. Configure model keys or dataset IDs if required.  
4. Hit **Run** and iterate!

---

## Contributing 🤝

Got a neat Dify experiment? **PRs are welcome!**

1. Fork → new branch  
2. Place your YAML under the correct folder  
3. Add a brief markdown description + attribution links  
4. Ensure the file imports cleanly in the current stable Dify release  
5. Open a pull request — we’ll review ASAP.

See **CONTRIBUTING.md** for coding style, naming conventions, and linting tips.

---

## Roadmap

- [ ] CI check that every flow imports without error  
- [ ] Auto-generate a gallery page with screenshots  
- [ ] Tag flows by model family & complexity  
- [ ] Weekly “flow spotlight” in Discussions

---

## License

All original content is **MIT**. Individual flows may include third-party work; where applicable, licenses and attribution are noted in their folders.

---

## Acknowledgements

Huge thanks to the [Dify](https://dify.ai/) team and all community members sharing their creativity. ✨
