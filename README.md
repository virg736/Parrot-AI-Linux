r
# Parrot AI Linux — Part 2: Adding a Local LLM Without Trusting It

Part 2 of **Parrot AI Linux** focuses on integrating a local LLM while keeping Linux execution behind deterministic security controls.


## Tech Stack

`Linux` · `Parrot OS` · `Python` · `pytest` · `Git` · `llama.cpp` · `Qwen2.5` · `GGUF` · `Local LLM` · `Policy Engine`

The architecture separates the LLM from direct system execution through:

- Structured action proposals
- A deterministic Policy Engine
- `ALLOW / DENY / CLARIFY` decisions
- Controlled Linux command execution
- Regression tests for security behavior

This version integrates **Qwen2.5 locally through llama.cpp**, demonstrates a real LLM hallucination, hardens the output contract, and finishes with **17 passing tests**.

## Core Principle

> **The LLM proposes. The Policy Engine decides. Linux executes only what is allowed.**

## Video

🎥 **I Gave My Linux AI Agent an LLM — But Can It Be Trusted?**

[Watch on YouTube](YOUR_YOUTUBE_LINK)


## Tools & Technologies

- **Linux / Parrot OS** — development and execution environment
- **Python** — core agent logic and security controls
- **pytest** — automated testing and security regression tests
- **Git** — version control and development history
- **llama.cpp** — local LLM inference
- **Qwen2.5 0.5B Instruct (GGUF)** — local language model
- **Policy Engine** — deterministic `ALLOW / DENY / CLARIFY` decisions
- **Structured Action Proposals** — controlled interface between the LLM and Linux
- **subprocess** — controlled Linux command execution
- **Local LLM Server** — local communication between the agent and the model


