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

> "llama.cpp v0.7.0 adds the LiliCorr speculative decoding technique and MTP for GLM5-Next, a new GPU cache for host-memory MoE experts (`--moe-cache-mib`, up to ~2.2x decode speedup when experts are offloaded), and a large batch of new models..."

> "New GPU cache for host-memory MoE experts (`--moe-cache-mib`): experts run on the GPU from an LRU cache, up to 2.2x faster decode [#29887]"

Source: https://github.com/ggml-org/llama.cpp/releases/tag/v0.7.0

## Fact 4 — vLLM (current stable version + headline change)

> "# v0.32.0
> ## Highlights
> This release features 814 commits from 363 contributors (121 new)!
> * **Structured decisions and generic parsers**: the new `POST /v1/systemone` endpoint answers `choice`, `noul` and `score` questions over a structured state (#59299), is served by default (#60677, #60696), and also runs on `Cloudflare/clef-omni` (#61064), `LiquidAI/d1-3B` (#60676) and DiffusionGemma (#60466)."

Source: https://github.com/vllm-project/vllm/releases/tag/v0.32.0
