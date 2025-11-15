# WeightedAI

A small research collective exploring practical AI/ML systems — from semi-supervised learning and semi-supervised trees to domain-specific models and datasets.

This repository contains the source for the **WeightedAI** website, served at:

> https://weightedai.github.io/

The site is intentionally minimal and focuses on a few selected research directions and projects.

---

## Overview

WeightedAI is interested in how models behave under real constraints — data, compute, human time — and how to build interfaces and infrastructure that respect those limits.

On the website you will find:

- A short overview of the group.
- Pointers to selected research projects and code.
- Links to external resources (papers, repos, models, datasets).

The site is a single-page application built with **React** and **Tailwind CSS** via CDNs. There is no build step; it runs as static HTML + JS.

---

## Featured Projects

### SemiDeep

- **Repo:** https://github.com/WeightedAI/semideep  
- **Paper:** “Enhancing Classification with Semi-Supervised Deep Learning Using Distance-Based Sample Weights” (ICMLT 2025)  
- **Summary:**  
  PyTorch implementation of a semi-supervised learning approach that assigns distance-based sample weights. The method improves generalization in settings with limited labeled data, class imbalance, noisy labels, or domain shift by emphasizing training samples that are closer to test samples in feature space.

### SemiCART

- **Repo:** https://github.com/WeightedAI/semicart  
- **Paper:** “Building Semi-Supervised Decision Trees with Semi-CART Algorithm” (IJMLC 2024)  
- **Summary:**  
  Semi-supervised decision tree algorithm that extends CART with distance-based weighting and a modified Gini index. Fully compatible with the scikit-learn API and evaluated on multiple datasets, consistently outperforming standard CART, especially when unlabeled data is abundant.

### Persian OCR (Model & Dataset)

- **Model:** https://huggingface.co/WeightedAI/Persian_OCR  
- **Dataset:** https://huggingface.co/datasets/WeightedAI/Persian_OCR_synth_sentences_100k  
- **Summary:**  
  OCR model and synthetic sentence dataset for Persian text recognition, released on Hugging Face for research and downstream applications.

---

## Tech Stack

The website uses:

- **React 18** (UMD via CDN)
- **ReactDOM 18** (UMD via CDN)
- **Tailwind CSS** (via CDN)
- Plain **HTML/JS** (no build tools, no bundler)

All logic and layout live inside a single [index.html](cci:7://file:///Users/aydin/Space/engineering/Projects/WeightedAI/WeightedAI/index.html:0:0-0:0).

---

## Repository Structure

```text
.
├── index.html      # Single-page React + Tailwind site for weightedai.github.io
└── (optional files below)
    ├── README.md   # This document
    ├── LICENSE     # Project license, e.g. MIT
    └── .gitignore  # Ignore OS/editor/venv artifacts