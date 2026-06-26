# OpenFable

**Verified output. Open to everyone.**

OpenFable is an open-source verified output engine. It runs multiple AI models in a silent critique loop - generate, verify, fix, deliver - so every response is refined before the user sees it.

No enterprise contract. No gatekeeping. Just models that earn their trust through silent, rigorous verification - every time.

## How It Works

```
User prompt
    |
    v
Mythos (generate) -> Critics (verify) -> Fix if needed -> Deliver
    |
    v
Final output - clean, no trace of the loop
```

The user never sees the verification process. They just get better output.

## Models

| Model | Role | Size |
|-------|------|------|
| Mythos-9B-Unhinged | Generator | 5.0 GB |
| ShellWhisperer | Code critic | 986 MB |
| Eve V2 | Tone/quality critic | 3.4 GB |

All models run on a single GPU (RTX 4090 24GB) via Ollama.

## Quick Start

### Self-host

```bash
# Install Ollama
curl -fsSL https://ollama.com/install.sh | sh

# Pull models
ollama pull FableForge-AI/mythos-9b-unhinged
ollama pull FableForge-AI/shellwhisperer
ollama pull jeffgreen311/Eve-V2-Unleashed-Qwen3.5-8B-Liberated-4K-4B-Merged

# Run
ollama run FableForge-AI/mythos-9b-unhinged
```

### Hosted

Visit [ui.openfable.io](https://ui.openfable.io) for the hosted version.

## Pricing

| Tier | Price | What |
|------|-------|------|
| Eve (Free) | $0 | Free models, daily cap |
| OpenFable | $19/mo | Full verify loop on GPU |
| OpenMythos | $29/mo | Uncensored, full loop |

## Ecosystem

Part of the DAI (Decentralized Autonomous Inference) ecosystem.

## Links

- **Website:** [openfable.io](https://openfable.io)
- **App:** [ui.openfable.io](https://ui.openfable.io)
- **HuggingFace:** [huggingface.co/openfable-io](https://huggingface.co/openfable-io)
- **X/Twitter:** [@openfable_io](https://x.com/openfable_io)

## License

MIT
