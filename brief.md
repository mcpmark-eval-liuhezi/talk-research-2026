# Homelab LLM Stack — Fact Sheet (2026 lightning talk)

Every version below was verified against a primary source (official release notes or official download page) on 2026-10-20. Source URLs are listed alongside each fact. If a version number changes before the talk, re-check the source link rather than trusting this file.

## The stack

| Component | Current stable / standard version | Headline change in latest release | Primary source |
|---|---|---|---|
| Ubuntu Server LTS | **26.04.1 LTS** | — (LTS release; 5 years of security/maintenance updates, up to 15 with Ubuntu Pro) | https://ubuntu.com/download/server |
| Ollama | **v0.40.6** | `win: prevent orphaned runners` (plus `gguf: add the q2_0 tensor and file types`) | https://github.com/ollama/ollama/releases/tag/v0.40.6 |
| llama.cpp | **v0.7.0** | New GPU cache for host-memory MoE experts (`--moe-cache-mib`): up to 2.2x faster decode when experts are offloaded | https://github.com/ggml-org/llama.cpp/releases/tag/v0.7.0 |
| vLLM | **v0.32.0** | Structured decisions and generic parsers — new `POST /v1/systemone` endpoint plus checkpoint-driven `hf` tool/reasoning parsers (814 commits from 363 contributors, 121 new) | https://github.com/vllm-project/vllm/releases/tag/v0.32.0 |

## Notes for the slides

- **Ubuntu Server**: the standard download on the official server page is Ubuntu 26.04.1 LTS (Intel/AMD 64-bit, ~3 GB ISO). 26.10 is the current interim release, not the standard LTS download. The previous LTS still supported is 24.04.5.
- **Ollama**: v0.40.6 is the latest non-draft, non-prerelease tag. Its changelog is a short bulleted list; the first item (Windows orphaned-runner fix) is the lead change. Released 2026-10-16.
- **llama.cpp**: v0.7.0's headline is the new GPU cache for MoE experts kept in host memory (`--moe-cache-mib`), which gives up to ~2.2x decode speedup when experts are offloaded. Note the server's default port also changed from 8080 to 9931 — worth mentioning if you demo the server live. Other highlights: LiliCorr speculative decoding, MTP for GLM5-Next.
- **vLLM**: v0.32.0 leads with structured decisions and generic parsers (the new `/v1/systemone` endpoint, and `hf` tool/reasoning parsers that read the checkpoint's `response_template`). Also noteworthy for a homelab audience: low-precision KV cache support has expanded, and Python 3.10 support was dropped in this release.

## Full quote-level provenance

Verbatim source extracts for each fact were committed to `notes/extracts.md` and then removed once this brief was finalised; the git history of this repository preserves the original extract text and its source URL per fact. Browse the commit history to see them.
