
<h1 align="center">Parrot AI Linux - Partie 2 : Ajouter un LLM local sans lui faire confiance</h1>

<p align="center">
  <img src="./parrot_design.jpg" alt="Parrot AI Linux" width="500">
</p>

<p align="center">
  Cette deuxième partie de Parrot AI Linux présente l’intégration d’un LLM local tout en conservant l’exécution Linux derrière des contrôles de sécurité déterministes.
</p>

<p align="center">
© 2026 Virginie Lechene 
</p>








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


