# SLM-RAG Structural Prompts

This repository provides the prompt data and prompt templates used in the paper:

**A Controlled Study of Prompt Structure in SLM-Based RAG**

## Overview

This repository contains the instruction data and structural prompt templates used to study prompt-structure sensitivity in small language model (SLM) based retrieval-augmented generation (RAG) for multiple-choice question answering.

The data are designed for controlled experiments in which retrieval evidence is fixed and only prompt structure is varied.

## Repository Structure

### `instructions/`

This directory contains the instruction data constructed from two sources:

- the rule-based emergency-response dataset from the DataFountain competition:  
  https://www.datafountain.cn/competitions/1086
- the C3 dataset:
  https://dataset.org/c3/

Each instruction instance includes:

- the question
- the candidate options
- the gold answer
- the cited supporting evidence
- the correct evidence ID(s)

These data are used to support controlled RAG experiments under fixed-evidence conditions.

### `prompt_template/`

This directory contains **60 prompt templates**.

Each template is named using the combination of:

- `Sx`: input-side structural variant
- `OTx`: output-side structural variant

So each prompt template corresponds to one structural condition defined by an input-side configuration and an output-side configuration.

## Intended Use

This repository is intended for:

- prompt-structure analysis in SLM-based RAG
- controlled evaluation under fixed evidence
- research on input-side and output-side prompt variations
- reproduction of the prompt settings used in the paper

## Citation

If you use this repository, please cite the corresponding paper.

```bibtex
@article{yourpaper,
  title={A Controlled Study of Prompt Structure in SLM-Based RAG},
  author={Author Name and Author Name},
  journal={...},
  year={2026}
}
