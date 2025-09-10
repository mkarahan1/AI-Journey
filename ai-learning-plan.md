# AI & LLM Learning Journey Plan

## Phase 1 --- Foundations (2 weeks)

Goal: Get comfortable with Python ML basics + Transformers, build
confidence with simple projects.

### Week 1

-   Basics refresher: Python typing, pathlib, virtualenv, Jupyter in VS
    Code.\
-   Pandas + Numpy for text data (load, clean, tokenize).\
-   **Project 1:** Spam/SMS Classifier (Logistic Regression with
    scikit-learn).\
-   Push to GitHub: notebook, `README.md`, data link, results
    screenshot.

### Week 2

-   Hugging Face intro: `pipeline`, `transformers`.\
-   Prompt engineering basics (zero-shot, few-shot).\
-   **Project 2:** Sentiment CLI app with DistilBERT.\
-   **Mini-Notebook:** Prompt Cookbook (test prompt patterns).\
-   Push to GitHub.

------------------------------------------------------------------------

## Phase 2 --- Deep Dive Track (4 weeks)

Focus: **LLMs + Retrieval (RAG)**

### Week 3

-   Embeddings: cosine similarity, FAISS/Chroma.\
-   **Project 3:** Semantic Search over PDFs/texts.\
-   Push: small CLI for `python search.py "query"`.

### Week 4

-   Build a basic Retrieval-Augmented Generation (RAG) pipeline.\
-   **Project 4:** RAG v0 (retrieve → prompt → answer with citations).\
-   Add a test set (5--10 Q&A pairs).\
-   Push + README with example Q&A.

### Week 5

-   Evaluation: precision, recall@k, answer accuracy.\
-   **Project 5:** RAG Eval Harness → produce metrics and HTML report.\
-   Push: include `eval/` dataset + report screenshots.

### Week 6

-   Fine-tuning basics: LoRA on a small instruction dataset.\
-   **Project 6:** Finetune TinyLlama or Phi-2 on a toy dataset.\
-   Push: notebook + base vs finetuned comparison.

------------------------------------------------------------------------

## Phase 3 --- Small Apps (3 weeks)

Build "apps" on top of what you learned.

### Week 7

-   **Project 7:** RAG API with FastAPI (endpoint: `/ask`).\
-   Add streaming output + logs.\
-   Push with Dockerfile for easy run.

### Week 8

-   **Project 8:** Structured Extraction (resume/invoice → JSON with
    pydantic schema).\
-   Add retry-with-schema logic.\
-   Push with test cases.

### Week 9

-   **Project 9:** Mini-Agent (calculator, notes, search stub).\
-   Limit to N steps, log traces.\
-   Push final demo + GIF/video in README.

------------------------------------------------------------------------

## Ongoing Habits

-   End each week: record a **90-sec screen capture demo**.\
-   Document: what worked, what failed, and next steps.\
-   Push everything to GitHub (1 repo with `projects/XX-name`).

------------------------------------------------------------------------

## Repo Template

    ai-journey/
      projects/
        01-spam-classifier/
        02-sentiment-cli/
        03-semantic-search/
        04-rag-v0/
        ...
      common/
        utils.py
      README.md

------------------------------------------------------------------------

## Stretch Goals

-   Add a **simple frontend** (Streamlit/Gradio) for RAG API.\
-   Deploy to **Render/Heroku/Hugging Face Spaces**.\
-   Try **LangChain vs LlamaIndex** for RAG orchestration.\
-   Build a **personal knowledge assistant** on your notes.
