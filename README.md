# ESG Carbon RAG Teaching Notebook

This repository contains a beginner-friendly Jupyter notebook for teaching a simple RAG (Retrieval-Augmented Generation) workflow in a green finance / ESG context.

Main file:

- `simple_rag_esg_carbon_teaching.ipynb`

What students learn:

- PDF/text report loading
- Chunking
- Vector database retrieval with `ChromaDB`
- Swappable LLM backends:
  - local lightweight model (default demo path)
  - DeepSeek API
  - OpenAI / ChatGPT API
- Structured extraction of carbon emissions information from ESG reports

## Notes

- ESG report PDFs are **not included** in this repo.
- Local run logs, vector DB files, and generated outputs are excluded.
- Helper scripts used to generate/execute the notebook are intentionally excluded from version control to keep the repository teaching-focused.

## Quick Start

1. Create a Python environment and install dependencies:

```bash
pip install -r requirements.txt
```

2. (Optional) Configure API keys in `.env` using `.env.example`.

3. Place ESG report files under `data/esg_reports/` (the notebook also includes a download helper for the tested company reports).

4. Open and run:

```bash
jupyter notebook simple_rag_esg_carbon_teaching.ipynb
```

