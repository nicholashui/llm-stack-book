# LLM 技術棧 — 從矽晶到代理

繁體中文譯本。原著 [Prakash Kagitha](https://github.com/prakashkagitha/llm-stack-book)，*The LLM Stack: From Silicon to Agents*（2026），依 [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.zh_TW) 授權翻譯。

[![Deploy](https://github.com/nicholashui/llm-stack-book/actions/workflows/deploy.yml/badge.svg)](https://github.com/nicholashui/llm-stack-book/actions/workflows/deploy.yml)
[![Code tests](https://github.com/nicholashui/llm-stack-book/actions/workflows/test.yml/badge.svg)](https://github.com/nicholashui/llm-stack-book/actions/workflows/test.yml)
[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

這是一本由底層講起的大型語言模型技術棧指南：從 GPU 矽晶與數值，經過 Transformer 與訓練，到推論服務、代理、檢索、評測與安全。程式碼、公式與產品名稱保留英文。用語鎖在 [`translation/TERMS.md`](translation/TERMS.md)。目錄、網站介面與前言已譯；其餘章節逐章譯出。

**閱讀譯本：** https://nicholashui.github.io/llm-stack-book/

**英文原書：** https://prakashkagitha.github.io/llm-stack-book/

- **134 chapters** across 14 parts (foundations → transformer → pretraining → kernels → post-training → RL infra → inference → agents → RAG → multimodal → evaluation → production → interpretability/safety → appendix)
- **690 hand-built SVG figures and animations**, theme-aware and reduced-motion safe
- **CI-tested code** — every runnable code block is assembled into `tests/` and executed on CPU in CI ([`test.yml`](.github/workflows/test.yml)); ~50 real bugs were caught and fixed this way
- **Runnable notebooks** — one **Colab-openable** notebook per chapter in [`notebooks/`](notebooks/README.md), built from the CI-verified code: read the chapter, run it in your browser
- A companion **interview prep** track at [`/interview/`](https://nicholashui.github.io/llm-stack-book/interview/)

## Repository layout

| Path | What it is |
|------|------------|
| `content/` | The book source — Markdown, one folder per part |
| `figures/` | Standalone HTML/SVG figures, expanded into pages via `{{fig:NAME}}` markers |
| `assets/` | Stylesheets and static assets |
| `build.py` | Static-site builder (Markdown → HTML) |
| `book.json` / `interview.json` | Table of contents and metadata for the two collections |
| `scripts/` | Authoring, QA, and figure-generation tooling |
| `site/` | Build output (not tracked on `main`; deployed to the `gh-pages` branch) |

## Building locally

```bash
pip install -r requirements.txt
python3 build.py          # renders content/ + figures/ into site/
cd site && python3 -m http.server 8000   # then open http://localhost:8000
```

## Deployment

Pushing to `main` triggers [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml),
which installs the pinned dependencies, runs `build.py`, and publishes `site/` to
GitHub Pages. No manual deploy step is needed — just edit, commit, and push.

## Contributing

Corrections and improvements are welcome — see [CONTRIBUTING.md](CONTRIBUTING.md).
Report errors via the **Errata** issue template.

## License & citation

Licensed under [**CC BY 4.0**](LICENSE) — share and adapt freely, even commercially, with attribution.

```bibtex
@book{kagitha_llm_stack_2026,
  title  = {The LLM Stack: From Silicon to Agents},
  author = {Kagitha, Prakash},
  year   = {2026},
  url    = {https://prakashkagitha.github.io/llm-stack-book/},
  note   = {Open web textbook, CC BY 4.0}
}
```
