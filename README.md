<div align="center">

# Vynex

### Developer infrastructure for unified access to frontier LLMs.

One OpenAI-compatible endpoint for **GPT, Claude, Gemini, DeepSeek, Qwen & GLM** —
keep your existing OpenAI SDK, change only the `base_url`.

</div>

---

## What we build

**[Vynex API](https://llm-api.vynexcloud.com/)** — a unified LLM gateway that exposes a
single OpenAI-compatible `/v1` endpoint. Developers call every major frontier model
family from one API key and one base URL, and switch models by changing the `model`
field. No new SDK, no integration rewrite.

- **Model families**: OpenAI (GPT-5.x), Anthropic (Claude Opus/Sonnet/Haiku 4),
  Google (Gemini 3.x / 2.5), DeepSeek, Qwen, Zhipu GLM
- **Features**: streaming, function/tool calling, embeddings, structured output
- **Pricing**: transparent, per-token, pay-as-you-go

## Quick start

```python
from openai import OpenAI

client = OpenAI(
    api_key="sk-...",
    base_url="https://llm-api.vynexcloud.com/v1",
)

# Same call works for Claude, Gemini, DeepSeek — just change the model name
response = client.chat.completions.create(
    model="gpt-5.4",
    messages=[{"role": "user", "content": "Hello!"}],
)
```

## Links

- 🌐 [Website](https://llm-api.vynexcloud.com/)
- 📖 [Documentation](https://llm-api.vynexcloud.com/docs/)
- 💰 [Pricing](https://llm-api.vynexcloud.com/pricing)
- 🔑 [Get an API key](https://llm-api.vynexcloud.com/register)
- 💻 [SDK & examples](https://github.com/vynexlimited/vynex-api-sdk)

## Repositories

| Repo | Description |
|---|---|
| [`vynex-api-sdk`](https://github.com/vynexlimited/vynex-api-sdk) | Official SDK, quick-start guides & runnable examples |

<div align="center">

**[Get your API key →](https://llm-api.vynexcloud.com/register)**

</div>
