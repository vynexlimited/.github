<div align="center">

# Vynex

### One OpenAI-compatible endpoint for every frontier model.

Call GPT, Claude, Gemini, DeepSeek, Qwen and GLM from a single `/v1` endpoint.
Keep your existing OpenAI SDK — just change the `base_url`.

</div>

---

## What is Vynex API?

**Vynex API** is a unified, OpenAI-compatible LLM API gateway. One API key, one
`base_url` gives you access to every frontier model family — no SDK rewrites,
no per-provider integration.

```python
from openai import OpenAI

client = OpenAI(
    api_key="sk-...",
    base_url="https://llm-api.vynexcloud.com/v1",
)
# Same call works for GPT, Claude, Gemini, DeepSeek, Qwen, GLM:
client.chat.completions.create(model="claude-opus-4-8", messages=[...])
```

## Models available

| Family | Flagship models |
|--------|-----------------|
| OpenAI | `gpt-5.5`, `gpt-5.4`, `gpt-5.4-mini`, `gpt-5.4-nano` |
| Anthropic | `claude-opus-4-8`, `claude-sonnet-4-6`, `claude-haiku-4-5-20251001` |
| Google | `gemini-3.1-pro-preview`, `gemini-3-pro-preview`, `gemini-2.5-pro`, `gemini-2.5-flash` |
| Open | `deepseek/deepseek-v3.2`, `qwen3.5-plus`, `GLM-5` |

Streaming, function/tool calling, and structured output are supported across all families.

## Links

- 🌐 [Website](https://llm-api.vynexcloud.com/)
- 📖 [Documentation](https://llm-api.vynexcloud.com/docs/)
- 💰 [Pricing](https://llm-api.vynexcloud.com/pricing)
- 🔑 [Get an API key](https://llm-api.vynexcloud.com/register)
- 📦 [SDK & Examples](https://github.com/vynexlimited/vynex-api-sdk)

## Repositories

| Repo | Description |
|------|-------------|
| [`vynex-api-sdk`](https://github.com/vynexlimited/vynex-api-sdk) | Public SDK & code examples (Python, Node.js, curl) |

<div align="center">
<sub>Transparent per-token pricing · OpenAI-compatible · Global access</sub>
</div>
