# BioMCP‑Examples

A companion repository of **worked examples** that demonstrate how
the [BioMCP](https://github.com/genomoncology/biomcp) toolkit can be used (and
tested) by a variety of large‑language‑model "personas".

Each example poses a real biomedical question, records several independent
answers produced by different LLM systems, and includes third‑party judgment
runs so you can compare quality side‑by‑side.

## Why keep these examples?
- Build a public, reproducible corpus for benchmarking BioMCP and future MCP‑compatible agents.
- Provide ready‑made testbeds for debugging new tools, prompts, or evaluation pipelines.
- Offer concrete reference material for presentations and tutorials. 

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

## Adding a new experiment

Pull requests welcome! Please follow the MIT license and respect citations.

Create a folder at the repo root (e.g. `my_new_question/`) with:
    - `README.md` – describe the question, prompt, model settings, etc.
    - One or more `example_?.md` files with the raw model outputs.
    - Optionally an `evals/` sub‑folder with judge outputs.


## Experiments

| ID                   | Primary Question / Task                                                  | BioMCP capabilities exercised                                                                                                                             | Folder                                  |
|----------------------|--------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------|
| **researcher_hnscc** | *“What are the emerging treatment strategies for head and neck cancer?”* | PubMed & ClinicalTrials.gov search, evidence aggregation, Sequential‑Thinking outer loop, tool chaining; judged by Claude 3.7, Gemini 2.5 Pro & OpenAI o3 | [researcher_hnscc](./researcher_hnscc/) |

*More rows to come – feel free to add yours!*

______________________________________________________________________

### License

This repository is released under the MIT License (see `LICENSE`).

### Maintainers

[@imaurer](https://github.com/imaurer) • GenomOncology Engineering
