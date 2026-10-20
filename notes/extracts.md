# Source extracts — homelab LLM stack talk

Short quotes captured verbatim from primary sources (official release notes / official download pages). One entry per confirmed fact.

## Fact 1 — Ubuntu Server LTS (current standard download)

> "Ubuntu 26.04.1 LTS
> The latest LTS version of Ubuntu Server. LTS stands for long-term support — which means five years of free security and maintenance updates, extended to up to 15 years with Ubuntu Pro."

Source: https://ubuntu.com/download/server

## Fact 2 — Ollama (current stable version + headline change)

> "v0.40.6
> ## What's Changed
> * win: prevent orphaned runners by @dhiltgen in https://github.com/ollama/ollama/pull/18500
> * gguf: add the q2_0 tensor and file types by @jmorganca in https://github.com/ollama/ollama/pull/18967"

Source: https://github.com/ollama/ollama/releases/tag/v0.40.6

## Fact 3 — llama.cpp (current stable build + headline change)

> "llama.cpp v0.7.0 adds the LiliCorr speculative decoding technique and MTP for GLM5-Next, a new GPU cache for MoE experts kept in host memory (`--moe-cache-mib`, up to ~2.2x decode speedup when experts are offloaded), and a large batch of new models..."

> "New GPU cache for host-memory MoE experts (`--moe-cache-mib`): experts run on the GPU from an LRU cache, up to 2.2x faster decode [#29887]"

Source: https://github.com/ggml-org/llama.cpp/releases/tag/v0.7.0
