# HyDE Minimal Reproduction

This folder contains a minimal reproduction of **HyDE: Hypothetical Document Embeddings for Zero-Shot Dense Retrieval**.

## Goal

The goal of this reproduction is to understand the core idea of HyDE and implement a small runnable retrieval pipeline.

## Core Idea

HyDE first uses a language model to generate a hypothetical document from a query.  
Instead of directly embedding the original query, it embeds the generated hypothetical document and uses it for dense retrieval.

## What I Plan to Reproduce

- Direct query embedding retrieval
- Hypothetical document embedding retrieval
- A small comparison between the two retrieval methods
- Observations on when HyDE helps and when it may fail

## Planned Structure

- `paper_summary.md`: summary of the paper
- `reproduction_report.md`: reproduction process and findings
- `src/`: source code
- `data/`: toy corpus and example queries
- `results/`: retrieval outputs and comparisons

## Status

In progress.
