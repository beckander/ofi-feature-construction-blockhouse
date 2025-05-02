# OFI Feature Construction – Blockhouse Interview

This repository contains my implementation of a case study task involving Order Flow Imbalance (OFI) signal construction from limit order book (LOB) data.

## Features Implemented

1. **Best-Level OFI** — Tracks imbalance at the top of the book
2. **Multi-Level OFI** — Measures pressure across 10 levels of the LOB
3. **Integrated OFI** — Aggregates multi-level OFI via PCA
4. **Cross-Asset OFI** — LASSO regression modeling return of one asset based on others' OFIs

## Files

- `ofi_feature_construction.ipynb`: Jupyter notebook with full code implementation and comments
- `ofi_answers.pdf`: Written answers to conceptual questions in LaTeX

## Notes

The provided dataset included only a single asset (`AAPL`). To demonstrate the cross-asset regression pipeline, I generated synthetic additional assets (`FAKE1`, `FAKE2`) by duplicating the AAPL order book data. The code automatically exits that step if true multi-asset data is unavailable within the given dataset.

Anderson Beck
