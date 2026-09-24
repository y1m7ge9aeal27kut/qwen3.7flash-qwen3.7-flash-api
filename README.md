# Qwen3.7 Flash API (qwen3.7-flash / qwen3.7flash) — llm guide with published pricing

> **input $0.0229; cached_input $0.0046; explicit_cached_input $0.0023** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://go.apimart.ai/k-443d21)** · **[Get an API key](https://go.apimart.ai/k-ff3872)**

Everything here refers to **qwen3.7-flash** — also written **qwen3.7flash** or **qwen3.7 flash**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `input` | $0.0229 |
| `cached_input` | $0.0046 |
| `explicit_cached_input` | $0.0023 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $2.2857 |
| 1,000 | $22.8568 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"qwen3.7-flash","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
