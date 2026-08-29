---
title: AI Engineer
date: 2026-08-29
tags: []
notebook: private-shiki-notes
links: []
template: spec
---

# AI Engineer

Knowledge I need to become an AI Engineer
- [] LLM Fundamentals & Orchestration: prompt engineering, structured outputs (JSON/schema enforcing), context window management, and frameworks like LangChain, LlamaIndex, or Vercel AI SDK
- [] LangChain or LlamaIndex
- [] Vector Search & RAG: embeddings, vector databases (Pinecone, Qdrant, PGVector), and Retrieval-Augmented Generation strategies
- [] Local Inference & Hardware Optimization: Quantization formats (GGUF, AWQ), running on-device inference using low-level bindings (llama.cpp, Metal Performance Shaders, CoreML), and managing VRAM/RAM footprints.
- Evaluation & Fine-tuning: Evals (measuring accuracy and latency), PEFT/LoRA fine-tunning for lightweight base models.
- [] Python of course and/or Go

## Where to start, courses

- [] DeepLearning.ai
- [] Libraries & Repos: Explore llama.cpp is on Go/Node/C++, or test Swift bindings like llama.cpp integration wrapper packages.
- [] Community: Hugging Face docs, local models subreddits, and open source Github repositories

## Local Models without Third-Party Servers
Instead of running local servers, or an online server or connecting to OpenAI, or other AI providers I can run local models like Cotypist does.

- [] Embedded C/C++ runtimes: bindings like llama.cpp or ggml allow you to compile the engine directly into your application executable. The app reads model files (.gguf) directly into memory and executes tokens via C/C++ bindings or native FFI without invoking HTTP servers.
- [] Native Frameworks: On Apple platforms, you can compile models to CoreML (using mpsgraph or metal) and execute them natively inside macOS/iOS applications using Swift's native APIs without extra background daemons.

### How Cotypist works

Basically does the following:

- Runs embedding models without a third-party server.
- Runs lightweight local models (such as 3B-parameter models via llama.cpp bindings under the hood) locally on Apple Silicon
- Ties directly into macOS Accessibility APIs to draw ghost text inline across any native application without calling out to external cloud APIs or requiring pre-installed local servers.