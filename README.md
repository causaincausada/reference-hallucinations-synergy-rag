# Reference Hallucinations in LLM-Generated Systematic-Review Writing

Code and artifacts for the paper:

**Quantifying Reference Hallucinations in LLM-Generated Systematic-Review Writing: Effects of Retrieval and Hard Grounding in the SYNERGY Benchmark**

## Overview

This repository contains the notebook, result bundles, and exported analysis files used to study reference hallucinations in LLM-generated systematic-review writing under three conditions:

- `A_NO_RAG`
- `B_RAG`
- `C_RAG_STRICT`

The main comparison in the revised analysis focuses on:

- `gemini-3.1-pro-preview`
- `gemini-3-flash-preview`

Both were evaluated under the same overall retrieval design and scoring pipeline.

## Important notes

### Colab kernel restart
During execution, the Colab kernel restarted in the middle of the experiment.  
For that reason, the notebook includes recovery/resume cells used to restore state and continue the run.

### Gemini 2.5 Pro
`gemini-2.5-pro` was attempted, but it was not included in the main comparative analysis for the RAG-based conditions because of an API-level incompatibility between tool use and enforced structured JSON output.

As a result, keeping Gemini 2.5 Pro in the main comparison would not have been a fair model comparison.  
The main reported comparison therefore focuses on Gemini 3.1 Pro Preview and Gemini 3 Flash Preview.

## Repository contents

- `Cisti_2026_robust_revision_clean_run_3.ipynb` — main experiment notebook
- `experiment_bundle.zip` — raw and processed outputs
- `paper_writing_package_31_vs_flash.zip` — condensed tables, charts, and summaries for writing support

## Reproducibility
This repository is intended to support transparency and reproducibility of the reported experiments.  
Some cells are specifically included to recover execution state after interruption.

## Citation
If you use this repository, please cite the associated paper.
