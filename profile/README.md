# reverberage

Composable, MCP-native AI toolkits for text, audio, image, and video. Build pipelines. Not monoliths.

## What is reverberage?

reverberage is a hub-and-satellite ecosystem of independent Python packages. Each satellite does exactly one thing — audio in, text out; claim in, verdict out — and can be used standalone or composed into multimodal pipelines.

Built on Alibaba Cloud's Qwen model family. Running on 103M tokens of free quota.

## Repositories

| Satellite | Modality | What it does |
|-----------|----------|-------------|
| [**hub**](https://github.com/reverberage/hub) | meta | Docs, roadmap, scaffold scripts, orchestration |
| [**n3rverberage**](https://github.com/reverberage/n3rverberage) | engine | Provider abstraction, MCP servers, A2A hub, memory |
| [**transcriber**](https://github.com/reverberage/transcriber) | audio → text | AI-powered audio/video transcription |
| [**verify**](https://github.com/reverberage/verify) | text → text | Claim verification engine |

## Roadmap

| Phase | Satellite | Model | Status |
|-------|-----------|-------|--------|
| Tier 1 | **transform** | qwen3-coder-plus | planned |
| Tier 1 | **see** | qwen3.7-plus | planned |
| Tier 1 | **hear** | qwen3.5-omni-plus | planned |
| Tier 1 | **speak** | cosyvoice-v3.5-plus | planned |
| Tier 2 | **summarize** | qwen3.6-flash | planned |
| Tier 2 | **translate** | qwen-mt-plus | planned |
| Tier 2 | **extract** | qwen3-coder-plus | planned |
| Tier 2 | **reason** | qwq-plus | planned |

See the full [roadmap](https://github.com/reverberage/hub/blob/main/docs/roadmap.md).

## Getting started

```bash
pip install rvrb-transcriber
rvrb-transcriber audio.mp3
```

Each satellite follows the [Satellite Protocol v2](https://github.com/reverberage/hub/blob/main/docs/satellite-protocol-v2.md) — hatchling build, typer CLI, Pydantic v2 models, MCP-native, Python 3.11+.

## Contributing

See [CONTRIBUTING.md](https://github.com/reverberage/.github/blob/main/CONTRIBUTING.md).

## License

Apache-2.0
