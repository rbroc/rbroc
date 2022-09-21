---
title: "Text transformer for context-aware encoding"
description: "This project focuses on training transformer encoders whose representations incorporate information about higher-order context, i.e., characteristics of the author and/or the pragmatic context. We feed models a target sequence and a number of 'context' sequences (i.e., text from the same author, or from the same subreddit) as a single example, and train models on a variant of MLM where the MLM head is fed the combination of token-level representations of the input sequence and an aggregate representation of context sequences. \n  \n
We experiment with three DistilBERT-inspired architectures: a bi-encoder (where context and target are fed to two separate encoders), a 'batch' encoder (single encoder with added context aggregation and target-context combination layers) and a hierarchical encoder (applying attention across [CLS] tokens in between standard transformer layers to integrate information across contexts and target sequence). The benefits of this training protocol are evaluated both by comparing their MLM performance with no-context MLM training and to random-context training, as well as on extrinsic tasks.  \n  \n 
This project is still in progress.  \n  \n"
repo: "ctx_transformers"
tags: ["NLP", "transformers", "DistilBERT", "TensorFlow", "huggingface", "ML"]
weight: 3
draft: false
---
