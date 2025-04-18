### 1 . Example overview  

| Example | Size&nbsp;(tokens) | Under‑the‑hood model / system |
|---------|-------------------|-------------------------------|
| **A** | **16 192** | *ChatGPT Deep Research* |
| **B** | **4 956** | *Manus AI* |
| **C** | **7 890** | *Gemini Deep Research* |
| **D** | **2 301** | *Claude Deep Research* |
| **E** | **9 351** | *Claude 3.7* + **BioMCP** + Sequential‑Thinking loop + Web Search |

**BioMCP tool suite used in Example E**  
- *Clinical‑trial*: `trial_searcher`, `trial_protocol`, `trial_locations`, `trial_outcomes`, `trial_references`  
- *Literature*: `article_searcher`, `article_details`  
- *Genomics*: `variant_searcher`, `variant_details`  
- *Meta*: `sequential_thinking`, generic web search  

---

### 2 . What the three judges agreed on  

| Example | Consensus strengths (all judges) | Recurring concerns (all/most judges) |
|---------|----------------------------------|--------------------------------------|
| **E** | Widest scope across modalities; rigorous evidence tables; clear structure; explicit self‑critique | A few factual slips (e.g., dostarlimab approval), dense for non‑specialists |
| **A** | Extremely detailed on immunotherapy/targeted agents; rich citations; accurate & up‑to‑date | Thin on radiation/surgical advances; long paragraphs hurt readability |
| **C** | Exhaustive depth (includes gene/virus therapy); many tables; strong sourcing | Very technical prose; minor approval mis‑statements; heavier to navigate |
| **B** | Readable, well‑organized high‑level survey; touches niche areas (AI, PDT) | Shallower evidence, fewer citations, less depth on biomarkers & gene therapy |
| **D** | Concise executive summary; easy to digest | Least comprehensive; sparse citations; several key emerging areas omitted |

---

### 3 . Judge‑by‑judge ranking  

| Example | Claude 37 | Gemini 2‑5 Pro | OpenAI o3 | **Average rank** |
|---------|-----------|---------------|-----------|------------------|
| **E** | 1 | 1 | 1 | **1.00** |
| **A** | 2 | 2 | 2 | **2.00** |
| **C** | 4 | 3 | 3 | 3.33 |
| **B** | 3 | 4 | 4.5 | 3.83 |
| **D** | 5 | 5 | 4.5 | 4.83 |

*(OpenAI tied B & D for 4th; tie counted as 4.5.)*

---

### 4 . Final forced ranking (majority + average‑rank tie‑break)  

1. **Example E** – unanimous #1 for breadth, evidence rigour, and structure  
2. **Example A** – consistent #2 for depth and accuracy despite narrower scope  
3. **Example C** – very comprehensive but denser and with a few accuracy slips  
4. **Example B** – clear overview yet lacks supporting depth/citations  
5. **Example D** – most readable but sacrifices coverage and evidence  
