# AASTU AWS AI/ML — Week 2 Mini Semantic Search

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Aman21adu/aastu-week2-semantic-search/blob/main/Week2_Mini_Semantic_Search.ipynb)

A simple FAQ semantic search project for the **Week 2 lab**. This repository contains **only Week 2**, not the Week 1 assignment.

## Goal and requirements

- Load FAQ data from **CSV with pandas**.
- **Clean** missing entries, duplicate FAQs and inconsistent whitespace.
- **Chunk** long FAQ texts using a function with word overlap.
- Convert text chunks into embeddings with `sentence-transformers/all-MiniLM-L6-v2`.
- Store embeddings, original passages and metadata using **ChromaDB**.
- Ask a natural-language question and show the **top 3 distinct FAQ matches** with answers.

## Repository files

```text
aastu-week2-semantic-search/
├── Week2_Mini_Semantic_Search.ipynb   # Complete lab notebook
├── faqs.csv                           # Sample FAQ dataset (18 raw rows)
├── requirements.txt                   # Required Python packages
├── README.md                          # This description and instructions
├── .gitignore                         # Excludes .venv and generated Chroma files

```

## Run in Google Colab

1. Click **Open in Colab** above **after** the GitHub repository has been published.
2. Select **Runtime → Run all**.
3. Wait for the embedding model to download on the first run. If a restart is requested after packages install, restart the runtime and run again.
4. Confirm the notebook shows **16 clean FAQs**, **17 chunks**, the **Chroma stored-passages count**, and **3 results** for each example question.
5. Choose **File → Save a copy in Drive**; **Share** the copied notebook with your instructor (Viewer access).
6. Download the executed `.ipynb` from Colab and replace the notebook on GitHub. This preserves the outputs and creates a genuine second commit.

The notebook creates `faqs.csv` inside Colab when the separate repository dataset isn't in Colab's local runtime. No additional CSV upload or API key is needed.

## Run locally

```bash
python -m venv .venv
# Windows PowerShell:
.\.venv\Scripts\Activate.ps1
# On macOS/Linux: source .venv/bin/activate
python -m pip install -r requirements.txt
python -m pip install notebook
jupyter notebook Week2_Mini_Semantic_Search.ipynb
```

## Example queries

1. I forgot how to sign in to my student account.
2. Where can I check my examination marks?
3. I need a copy of my academic transcript.
4. How can my computer join the campus wireless network?
5. I need help picking subjects for next semester.

Each example is designed to retrieve the top 3 closest FAQs in the sample. **The exact ranking and distance depend on the model and runtime; inspect actual executed results.**

## Libraries

`pandas`, `numpy` (used by embeddings), `sentence-transformers`, `chromadb`. The project uses a **local** Chroma vector store; cloud hosting and API keys are not required.

## Limitations

The dataset is synthetic and provided only for training. It is **not an authoritative statement of AASTU policy**. Retrieval ranks related text but cannot guarantee factual correctness or that a relevant answer exists.

## Course reference

Based on the AASTU AI/ML AWS Cohort Week 2 practical notebook: *Data, APIs & Embeddings*.
