# EpistemicDistil
 
Research code for studying **uncertainty collapse in sequence-level knowledge distillation (SeqKD)** for large language models.
 
This repository accompanies the paper:
 
**Distilling answers, discarding uncertainty: Uncertainty collapse in sequence-level knowledge distillation**  
ICLR 2027 (under review)  
https://openreview.net/forum?id=KQYh1Ku6GP
 
## Overview
 
Sequence-level knowledge distillation transfers teacher-generated responses to smaller student models. This project investigates how distillation can reduce semantic uncertainty and weaken hallucination detection, even when predictive accuracy changes little.
 
The repository contains code for:
 
- Sequence-level knowledge distillation
- Semantic entropy and uncertainty estimation
- Answer correctness and hallucination-detection evaluation
- Analysis of uncertainty distributions and experimental results
 
## Repository Structure
 
```text
src/
├── distillation/   # Distillation pipeline
├── uncertainty/    # Semantic uncertainty estimation
├── evaluation/     # Evaluation utilities
├── analysis/       # Result analysis
└── utils/          # Shared utilities
```
 
## Installation
 
Install the Python dependencies:
 
```bash
pip install -r requirements.txt
```
 
## Usage
 
The main distillation entry point is:
 
```bash
python -m src.distillation.run --help
```
 
Configure model and dataset settings in `src/utils/config.py` before running experiments. Large-model experiments require suitable compute resources and model access.
 
## Paper
 
Tao, Y., Ren, Y., Yu, J. L., Gal, Y., & Li, L. (2026). *Distilling answers, discarding uncertainty: Uncertainty collapse in sequence-level knowledge distillation*. ICLR 2027, under review.
 
https://openreview.net/forum?id=KQYh1Ku6GP
