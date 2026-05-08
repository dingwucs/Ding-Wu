# AI Paper Reproductions

This repository documents my paper reproductions and research-oriented experiments in **dense retrieval, retrieval-augmented generation, and LLM evaluation**.

The goal of this repository is not only to run existing code, but also to understand core research ideas, build minimal runnable implementations, and write clear experimental observations.

This repository is a work in progress.

---

## Research Areas

I am currently focusing on:

- Dense Retrieval / Information Retrieval
- Retrieval-Augmented Generation
- LLM Evaluation
- RAG Reliability and Evidence Grounding

---

## Reproduction List

| No. | Paper / Topic | Area | Status | What I Aim to Reproduce |
|---|---|---|---|---|
| 01 | HyDE: Hypothetical Document Embeddings | Dense Retrieval | In Progress | Minimal zero-shot dense retrieval pipeline using hypothetical documents |
| 02 | ColBERT | Information Retrieval | Planned | Late interaction retrieval mechanism |
| 03 | RAG Evaluation | LLM Evaluation | Planned | A small evaluation pipeline for evidence-grounded answers |
| 04 | Conflict-Aware RAG | RAG Reliability | Planned | Toy experiments on conflicting retrieved evidence |

---

## Repository Structure

- `01-hyde/`  
  Minimal reproduction of HyDE for zero-shot dense retrieval.

- `02-colbert/`  
  Planned reproduction of late interaction retrieval.

- `03-rag-evaluation/`  
  Planned experiments on evaluating retrieval-augmented generation.

- `shared_utils/`  
  Common utility functions used across reproduction projects.

Each reproduction folder may include:

- `README.md`
- `paper_summary.md`
- `reproduction_report.md`
- `requirements.txt`
- `src/`
- `data/`
- `results/`
- `figures/`

---

## Reproduction Standard

For each paper or topic, I try to include the following components:

### 1. Paper Summary

A concise summary of:

- The research problem
- The core idea
- The method pipeline
- The main experimental setting
- The key contribution

### 2. Minimal Implementation

A small, runnable implementation of the core idea.

The first goal is to reproduce the mechanism, not necessarily the full-scale benchmark results.

### 3. Experimental Results

When possible, I include:

- Toy examples
- Retrieval or generation outputs
- Quantitative comparisons
- Failure cases
- Observations from experiments

### 4. Reproduction Report

Each reproduction report explains:

- What was reproduced
- What was not reproduced
- What assumptions were made
- What difficulties appeared
- What I learned from the experiment

### 5. Possible Extensions

For each paper, I also consider possible extensions, such as:

- Testing on a smaller or different dataset
- Replacing components with newer models
- Running ablation studies
- Applying the idea to RAG or LLM evaluation settings

---

## Current Project: HyDE Minimal Reproduction

The first project focuses on reproducing the core idea of HyDE.

HyDE uses a language model to generate a hypothetical document from a query. Instead of directly embedding the short query, the system embeds the generated hypothetical document and uses it for dense retrieval.

The minimal reproduction compares:

- Direct query embedding retrieval
- Hypothetical document embedding retrieval

The goal is to understand when and why generated hypothetical documents can improve retrieval.

---

## Why This Repository

I use this repository as a structured research learning log.

The purpose is to build a clear path from:

1. Reading papers
2. Understanding the core method
3. Implementing minimal versions
4. Running small experiments
5. Writing observations and limitations

This process helps me develop stronger foundations in machine learning, information retrieval, and research engineering.

---

## Technical Stack

The projects in this repository may use:

- Python
- PyTorch
- NumPy
- scikit-learn
- sentence-transformers
- FAISS or other vector search tools
- Jupyter Notebook
- Cursor / VS Code
- Git / GitHub

---

## Notes

This repository is mainly for learning, reproduction, and research preparation.

Some projects are minimal reproductions rather than full benchmark-level reproductions. When a full reproduction is not possible due to compute, data, or time constraints, I clearly state the limitations in the corresponding reproduction report.
