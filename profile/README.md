<p align="center">
  <img src="logo.png" alt="Diffusion-Group logo" width="130">
</p>

<h1 align="center">Diffusion-Group</h1>

<p align="center">
  Practical Stable Diffusion tooling for the hardware you already own —<br>
  automatic GPU detection, verified downloads, zero-setup installs.
</p>

<p align="center">
  <a href="https://github.com/jhfuheuiwfh/adaptdiffuse/releases/latest"><img alt="AdaptDiffuse release" src="https://img.shields.io/github/v/release/jhfuheuiwfh/adaptdiffuse?label=AdaptDiffuse&color=2f6fed"></a>
  <a href="https://github.com/jhfuheuiwfh/adaptdiffuse/actions"><img alt="CI status" src="https://img.shields.io/github/actions/workflow/status/jhfuheuiwfh/adaptdiffuse/ci.yml?branch=master&label=CI"></a>
  <a href="https://github.com/jhfuheuiwfh/adaptdiffuse/blob/master/LICENSE"><img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-2ea44f"></a>
  <a href="https://huggingface.co/spaces/PedAI/Adapt-Diffuse"><img alt="Live demo" src="https://img.shields.io/badge/demo-live%20on%20HF-ff9d00"></a>
</p>

---

## Projects

### [AdaptDiffuse](https://github.com/jhfuheuiwfh/adaptdiffuse)

Plug-and-play Stable Diffusion engine with a clean Gradio WebUI. One double-click `launch.bat`, no environment to configure.

- **Runs on your GPU, not on a shopping list** — automatic cascade `NVIDIA CUDA → Vulkan → DirectML → CPU`, with ROCm(HIP) as an explicit option
- **sd-cli first** — one native binary ([stable-diffusion.cpp](https://github.com/leejet/stable-diffusion.cpp)), no PyTorch install
- **Verified downloads** — byte count and SHA-256 checked before anything executes; path-traversal archives rejected
- **Failures are explained** — built-in Diagnóstico panel plus `logs/backend.log` with step, exit code and message
- **Day-to-day use** — checkpoints, LoRA with scale, batch renders and presets in the WebUI

<p align="center">
  <a href="https://github.com/jhfuheuiwfh/adaptdiffuse">Repository</a> ·
  <a href="https://github.com/jhfuheuiwfh/adaptdiffuse/releases/latest">Download</a> ·
  <a href="https://github.com/jhfuheuiwfh/adaptdiffuse#why-adapt-diffuse">Why AdaptDiffuse</a> ·
  <a href="https://huggingface.co/spaces/PedAI/Adapt-Diffuse">Live demo (SD 1.5, free ZeroGPU)</a>
</p>

## How we work

| Principle | What it means in practice |
|---|---|
| Verify before execute | size + SHA-256 on every binary and model we fetch |
| No silent failures | errors surface with exit code and log, never swallowed |
| Zero setup | one script to install, nothing to tune afterwards |
| Hardware-agnostic | old GPU, iGPU or no GPU — it still runs |

## Collaborating

Issues and pull requests are welcome on any public repository. Bug reports are most useful when they include the **Diagnóstico** output or `logs/backend.log`.

New ideas fit here too: inference backends, quantization recipes, UI polish, docs and translations.

---

<p align="center">
  <sub>Diffusion-Group · open source, MIT licensed · built by <a href="https://github.com/jhfuheuiwfh">@jhfuheuiwfh</a></sub>
</p>
