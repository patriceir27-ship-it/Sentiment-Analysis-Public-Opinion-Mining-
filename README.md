# Sentiment-Analysis-Public-Opinion-Mining
*A Full End-to-End Data Analytics & Data Science Project*


##  Project Overview

This repository contains a **professional, end-to-end sentiment analysis pipeline** built on large-scale social media text data (~70k posts).  
The project goes beyond basic sentiment classification by:

- repairing **structurally broken data**
- validating noisy sentiment labels
- combining **lexicon-based** and **transformer-based** models
- explaining **why** people feel positive or negative
- translating results into **clear, data-driven insights**

This work follows **industry-grade data analytics standards** and emphasizes **data understanding, correctness, interpretability, and storytelling**.



## 🎯 Objectives

- Understand and repair a **merged / corrupted dataset schema**
- Analyze public sentiment (Positive / Neutral / Negative)
- Validate provided sentiment labels using models
- Identify **sentiment drivers** (keywords, phrases, topics)
- Discover **systematic negativity or positivity by topic**
- Produce insights suitable for **decision-making and reporting**


## Methodology (High-Level)

### Data Understanding
- Diagnosed a **structurally broken dataset**
- Identified **two merged schemas**
- Analyzed missingness mechanisms and bias

### Data Cleaning & Structuring
- Reconstructed semantic columns:
  - `tweet_id`, `topic`, `sentiment_label`, `text`
- Removed exact & near-duplicate posts
- Preserved:
  - `raw_text` (interpretation)
  - `clean_text` (modeling)

 Final dataset: **69,972 clean posts**



###  Exploratory Data Analysis (EDA)
- Topic distribution (e.g. *Borderlands*)
- Sentiment class imbalance
- Text-length diagnostics
- Keyword & n-gram exploration



###  Sentiment Analysis Methodology
**Three-layer strategy**

| Layer | Purpose |
|-----|-------|
| Provided Labels | Initial reference (potentially noisy) |
| VADER | Fast, interpretable baseline |
| RoBERTa (Twitter) | Context-aware, state-of-the-art |

✔ Agreement analysis  
✔ Noise detection  
✔ Confidence scoring  

---

###  Sentiment Pattern Analysis
- Overall public mood
- Topic-wise sentiment ranking
- Negative-rate and mood-index metrics
- (Optional) sentiment trends over time


###  Explaining the “Why”
- Keyword drivers of **negative sentiment**
- Keyword drivers of **positive sentiment**
- Differential term analysis (log-odds)
- Topic modeling (BERTopic / LDA) on complaints



##  Key Outputs

- Clean, validated sentiment labels
- Topic-level sentiment rankings
- Actionable drivers of dissatisfaction & satisfaction
- Reproducible, well-documented pipeline



##  Manual Validation (Human-in-the-Loop)

A stratified audit sample is exported:




