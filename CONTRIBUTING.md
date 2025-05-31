# Contributing to Awesome-Dify-Agents 🤖✨

First off—thanks for taking the time to contribute!  
This project grows only through community creativity, so your bug reports, feature ideas, and new **Dify** flows are all hugely appreciated.

---

## 📑 Table of Contents
1. [Ground Rules](#ground-rules)
2. [How to Contribute](#how-to-contribute)
3. [Adding a New Flow](#adding-a-new-flow)
4. [Style Guide](#style-guide)
5. [Local Testing](#local-testing)
6. [Pull-Request Checklist](#pull-request-checklist)
7. [Code of Conduct](#code-of-conduct)
8. [License](#license)

---

## Ground Rules

- **Be respectful**. We value inclusive and constructive discussions.
- **Search first**. Check the [issues](../../issues) and existing PRs to avoid duplicates.
- **Small PRs > big PRs**. Incremental changes are easier to review and merge.
- **Keep it public-domain friendly**. Prefer open-source models, datasets, and APIs where possible.

---

## How to Contribute

| 🛠 Type | Recommended Path |
| ------ | ---------------- |
| **Bug report** | Open an issue → _Bug Report_ template |
| **Feature request / idea** | Open an issue → _Feature Request_ template |
| **Improve docs** | Fork → edit Markdown → PR |
| **Add or update a flow** | Follow the steps in [Adding a New Flow](#adding-a-new-flow) |
| **Refactor / tooling** | Open an issue first to discuss scope |

---

## Adding a New Flow

1. **Fork** the repo and create a new branch  
   ```bash
   git checkout -b feat/my-awesome-flow
   ```

2. **Place your `.yml`** under the correct top-level folder:

   ```
   flows/
   ├─ agents/
   ├─ chatbots/
   └─ chatflows/
      ├─ rag/
      ├─ integrations/
      └─ utilities/

   
   ```

   > If none fits, propose a new folder in your PR description.
3. **Name the file** with lowercase and dashes, e.g. `pdf-summarizer.yml`.
4. **Add a mini-README** inside the same folder:

   * What the flow does (one-liner)
   * Required models & keys
   * Screenshot or Mermaid diagram (optional)
5. **Test import** on the latest stable Dify release. The flow should:

   * Import without errors ✔️
   * Contain no hard-coded secrets 🔑
   * Produce a sensible response with default settings 🧪
6. **Commit** both YAML and README:

   ```bash
   git add flows/<folder>/pdf-summarizer.yml flows/<folder>/README.md
   git commit -m "feat: add pdf summarizer flow"
   ```
7. **Push & open a PR**. Use the **“Flow Submission”** PR template and fill in all fields.

---

## Style Guide

| Aspect         | Convention                                             |
| -------------- | ------------------------------------------------------ |
| **File names** | `kebab-case.yml`                                       |
| **YAML keys**  | Use Dify DSL defaults; avoid camelCase extras          |
| **Comments**   | Prefix with `#` and keep concise                       |
| **Markdown**   | Follow GitHub-flavored MD, wrap at 100 chars           |
| **Images**     | `.png` or `.webp`, ≤ 500 KB, commit in the same folder |
| **Commits**    | Conventional Commits (`feat:`, `fix:`, `docs:` …)      |

---

## Local Testing

```bash
# 1. Clone your fork
git clone https://github.com/<you>/awesome-dify-agents && cd awesome-dify-agents

# 2. (Optional) Enable pre-commit hooks
pip install pre-commit && pre-commit install

# 3. Lint the repo
pre-commit run --all-files
```

> **Tip:** Need a quick Dify sandbox? Use the `docker-compose.yml` from the upstream Dify repo and mount your flow folder for rapid import/export.

---

## Pull-Request Checklist

* [ ] My branch is up-to-date with `main`.
* [ ] The flow/YAML imports without errors in Dify v**X.Y.Z**.
* [ ] No secrets, proprietary data, or paid model IDs are included.
* [ ] Added a short README & (optional) screenshot.
* [ ] All markdown links work.
* [ ] I’ve run `pre-commit` (if installed) and fixed any issues.

---

## Code of Conduct

We follow the **[Contributor Covenant v2.1](https://www.contributor-covenant.org/version/2/1/code_of_conduct/)**.
By participating, you agree to uphold these guidelines. If you suffer or witness unacceptable behavior, please open a confidential issue or email the maintainers.

---

## License

By contributing, you agree that your submissions are released under the repository’s MIT license, unless stated otherwise in the specific flow folder. If your flow depends on third-party code or data, include the appropriate license notice in its subfolder.

---

*Thank you for helping build the best open-source catalog of Dify agents and workflows!*
