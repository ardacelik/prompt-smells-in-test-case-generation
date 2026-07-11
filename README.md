# GEM Prompts

Baseline and refactored prompt templates used by GEM, an LLM-based unit test generation pipeline, across its three stages: initial test synthesis, execution-driven self-repair, and mutation-guided oracle strengthening.

Each stage is provided in Python (pytest), Java (JUnit 5), and C++ (GoogleTest) versions, in both the baseline and refactored variants (18 files total). File naming: `<stage>-<language>-<variant>.md`. Each file contains the system prompt and the user prompt; content injected at runtime (source code, test files, diagnostics, mutation feedback, etc.) is denoted by `{{ ... }}` placeholders.
