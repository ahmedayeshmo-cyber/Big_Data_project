
## Overview

This project implements an **end-to-end big data pipeline** for detecting AI-generated Arabic abstracts using Apache Spark. The pipeline handles batch processing for model training and streaming for real-time inference, all within a Lambda architecture pattern.

**Key achievements:**
-  95.38% accuracy on test set (Logistic Regression)
-  Real-time streaming inference with Structured Streaming
-  Scalability benchmark: near-linear speedup up to 16 partitions
-  Arabic NLP preprocessing (diacritic removal, stemming, stopwords)

## Dataset

- **Source:** [KFUPM-JRCAI/arabic-generated-abstracts](https://huggingface.co/datasets/KFUPM-JRCAI/arabic-generated-abstracts) (Hugging Face)
- **Size:** 41,940 abstracts (after flattening)
- **Classes:** Human-written vs. AI-generated (Allam, Jais, Llama, OpenAI)
- **After preprocessing:** 36,525 rows

