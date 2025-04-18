# BioMCP‑Examples

A companion repository of **worked examples** that demonstrate how the [BioMCP](https://github.com/genomoncology/biomcp) toolkit can be used (and tested) by a variety of large‑language‑model "researcher" personas.  Each example poses a real biomedical question, records several independent answers produced by different LLM systems, and includes third‑party judgment runs so you can compare quality
side‑by‑side.

> **Why keep these examples?**
> * Build a public, reproducible corpus for benchmarking BioMCP and future MCP‑compatible agents.
> * Provide ready‑made testbeds for debugging new tools, prompts, or evaluation pipelines.
> * Offer concrete reference material for presentations and tutorials.

## Repository layout

```
biomcp-examples/
│  README.md          ← you are here
│  LICENSE            ← MIT, same as BioMCP
└─ researcher_hnscc/  ← one experiment (HNSCC treatment strategies)
   ├─ example_*.md    ← answers produced by different models
   ├─ evals/          ← judgment runs by Claude 3.7, Gemini 2.5 Pro, OpenAI o3
   └─ README.md       ← experiment‑specific notes
```

## Quick start

```bash
# 1  Clone both repos side‑by‑side
$ git clone https://github.com/genomoncology/biomcp.git
$ git clone https://github.com/genomoncology/biomcp-examples.git

# 2  Install BioMCP (fast path using uv)
$ cd biomcp
$ uv pip install -e .

# 3  Open any example and reproduce a run (see the experiment README)
$ cd ../biomcp-examples/researcher_hnscc
$ make reproduce   # (example target; adjust per experiment)
```

> **Tip:** The [`@modelcontextprotocol/inspector`](https://www.npmjs.com/package/@modelcontextprotocol/inspector) GUI is handy for poking around BioMCP tools interactively while you explore these examples.

## Adding a new experiment

1.  Create a folder at the repo root (e.g. `my_new_question/`).
2.  Inside, add:
    * `README.md` – describe the question, prompt, model settings, and anything noteworthy.
    * One or more `example_?.md` files – the raw model outputs.
    * Optionally an `evals/` sub‑folder with judge outputs.
3.  Update the **Experiments table** in the root `README.md` (see next section).

Pull requests welcome! Please follow the MIT license and respect source citations.

## Experiments

| ID | Primary Question / Task | BioMCP capabilities exercised | Folder |
|----|-------------------------|--------------------------------|--------|
| **researcher_hnscc** | *“What are the emerging treatment strategies for head and neck cancer?”* | PubMed & ClinicalTrials.gov search, evidence aggregation, Sequential‑Thinking outer loop, tool chaining; judged by Claude 3.7, Gemini 2.5 Pro & OpenAI o3 | [researcher_hnscc](./researcher_hnscc/) |

*More rows to come – feel free to add yours!*

---

### License

This repository is released under the MIT License (see `LICENSE`).

### Maintainers

[@imaurer](https://github.com/imaurer) • GenomOncology Engineering


