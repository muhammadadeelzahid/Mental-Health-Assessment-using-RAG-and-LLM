# Adaptive Retrieval-Augmented Generation for Psychological Assessment

This project presents an approach to performing automated psychological assessments (e.g., GAD-7) using Reddit user content, embedding models, and a large language model (LLM). Reddit posts are embedded and adaptively retrieved for each diagnostic item, then passed to a prompt-driven LLM which scores user responses accordingly.

## Overview

- Reddit users are selected from mental health-related subreddits.
- Posts and comments are embedded using **SentenceTransformers**.
- An adaptive K* retrieval method is used to select contextually relevant posts for each diagnostic item.
- Prompts are constructed for the **Mistral-7B-Instruct-v0.2** model to score each item based on retrieved evidence.
- Final scores align with standardized assessments (GAD-7, etc.).
