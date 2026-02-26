# ESG Carbon RAG Teaching Notebook

In this repository, we build a beginner-friendly Jupyter notebook for a simple RAG (Retrieval-Augmented Generation) workflow in a green finance / ESG context.

Main file:

- `simple_rag_esg_carbon_teaching.ipynb`

What We do in the notebook:

- PDF/text report loading
- Chunking
- Vector database retrieval with `ChromaDB`
- Swappable LLM backends:
  - local lightweight model (default classroom path)
  - DeepSeek API
  - OpenAI / ChatGPT API
- Structured extraction of carbon emissions information from ESG reports

## Notes

- ESG report PDFs are **not included** in this repo.
- Local run logs, vector DB files, and generated outputs are excluded.
- Helper scripts used to generate/execute the notebook are intentionally excluded from version control to keep the repository teaching-focused.
- We tested the notebook with `Python 3.12.10`.
- We pin direct dependencies in `requirements.txt` and provide a full environment snapshot in `requirements.lock.txt`.

## Quick Start

1. We create a Python `3.12.10` environment and install dependencies:

```bash
pip install -r requirements.txt
```

2. We can optionally configure API keys in `.env` using `.env.example`.

3. We place ESG report files under `data/esg_reports/` (the notebook also includes a download helper for the five-company run used in class).

4. We open and run:

```bash
jupyter notebook simple_rag_esg_carbon_teaching.ipynb
```
