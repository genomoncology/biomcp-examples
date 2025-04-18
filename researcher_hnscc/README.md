# Emerging Treatment Strategies for Head & Neck Cancer  
*BioMCP‑Examples • Researcher HNSCC*

---

## Original Question  
**“What are the emerging treatment strategies for head and neck cancer?”**

---

## Researchers & Example Files

| Letter | Model / Workflow | Answer |
|-------:|------------------|--------|
| **A** | ChatGPT Deep Research | [`example_a.md`](./example_a.md) |
| **B** | Manus AI | [`example_b.md`](./example_b.md) |
| **C** | Gemini Deep Research | [`example_c.md`](./example_c.md) |
| **D** | Claude Deep Research | [`example_d.md`](./example_d.md) |
| **E** | Claude 3.7 + **BioMCP** + Sequential‑Thinking + Web Search | [`example_e.md`](./example_e.md) |

> **Background docs for Manus AI** live in  
> [`manus_ai_background/`](./manus_ai_background/) – 20 + source files it cited.

---

## “LLM‑as‑Judge” Prompt  

> **TASK:** Compare, contrast, and force‑rank EXAMPLES A–E.  
>  • Create a rubric that *prioritises* **accuracy, clarity, and comprehensiveness**.  
>  • Add 3–5 additional comparison aspects.  
>  • Grade each example in tables, call out significant inaccuracies or omissions, and provide a final ranked list with reasoning.

The full judge prompt (above) was given verbatim to three large‑language models acting as reviewers. Their write‑ups live in **`evals/`**:

| Judge | File |
|-------|------|
| Claude 3.7 | [`evals/claude_37.md`](./evals/claude_37.md) |
| Gemini 2.5 Pro | [`evals/gemini_2_5_pro.md`](./evals/gemini_2_5_pro.md) |
| OpenAI o3 | [`evals/openai_o3.md`](./evals/openai_o3.md) |
| *o3 summary* | [`evals/summary_o3.md`](./evals/summary_o3.md) |

Each judge independently built its own rubric, scored the five answers, highlighted factual slips, and produced a forced ranking.

---

## TL;DR of the Judge Consensus ★

1. **Example E** — Widest scope, best structure, but note minor approval mis‑statements (dostarlimab).  
2. **Example A** — Deep immuno/targeted coverage & citations; lighter on radiation/surgical advances.  
3. **Example C** — Extremely comprehensive (incl. gene/virus therapy); dense prose, a few minor slips.  
4. **Example B** — Readable overview; shallower evidence & fewer citations.  
5. **Example D** — Concise executive summary; least comprehensive overall.

*(See individual eval files for the full scoring tables.)*

---

### How to Re‑run or Extend This Study

1. Bring up a BioMCP agent (see the root repo README).  
2. Feed it the original question or tweak as desired.  
3. Compare your new answer with the examples here—feel free to add yours!

Pull requests with fresh examples, alternate judging frameworks, or new biomedical questions are welcome. 🚀

### Note: YouTube Video Run is Different

I recorded a video of this same question with the same prompt, but given
the stochastic nature of LLMs, the response is different. 

You can watch the video here:
[https://youtu.be/tBGG53O-7Hg](https://youtu.be/tBGG53O-7Hg)

And you can read the response of that video run here:
[./biomcp_doc_2/example_e_v2.md](./biomcp_doc_2/example_e_v2.md)