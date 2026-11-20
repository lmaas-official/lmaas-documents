# Pricing

Last checked: 2026-11-12 (Japanese original) / Source: https://lmaas.io/#pricing (English), https://lmaas.io/ja#pricing (Japanese)

Customers **outside Japan** are billed in **US dollars**, and customers **in Japan** in **Japanese yen** (both excluding tax). Prices may change. Please check the pricing table on the official site for the latest amounts.

## Plans (customers outside Japan, USD)

| Plan | Model size | GPU | Monthly | Annual | Initial fee |
|---|---|---|---|---|---|
| Personal | up to 4B class | Shared GPU | $400 | $4,320 | $600 |
| Starter | up to 8B class | Shared GPU | $660 | $7,128 | $980 |
| Starter Plus | up to 8B class | Dedicated GPU | $2,250 | $24,300 | $3,380 |
| Business | up to 24B class | Shared GPU | $1,380 | $14,904 | $2,000 |
| Business Plus | up to 32B class | Dedicated GPU | $3,500 | $37,800 | $4,688 |

- Customers outside Japan can apply as businesses only.

## Plans (customers in Japan, JPY)

| Plan | Monthly | Initial fee | Annual |
|---|---|---|---|
| Personal | ¥64,000 | ¥96,000 | ¥691,200 |
| Starter | ¥105,000 | ¥158,000 | ¥1,134,000 |
| Starter Plus | ¥355,000 | ¥540,000 | ¥3,834,000 |
| Business | ¥218,000 | ¥320,000 | ¥2,354,400 |
| Business Plus | ¥560,000 | ¥750,000 | ¥6,048,000 |

The plan contents (model size, GPU, number of users, etc.) are the same in both currencies.

## Common notes

- "4B", "8B", "24B" and "32B" are AI model sizes (number of parameters: 4, 8, 24 and 32 billion). Larger numbers tend to mean higher performance, but use more computing resources.
- Annual payment is 10% less than 12 months of the monthly price.
- The minimum term is 90 days from the start of the contract.
- For larger AI models such as the 70B class, or other individual requests, please contact us through the contact form.

## Main differences between plans

| Plan | Best for | Users | Training runs (per 30 days) | Saved training versions | Storage | Available models (approx.) |
|---|---|---|---|---|---|---|
| Personal | Small businesses and professionals; easy to start | Up to 1 | 5 | Up to 3 | 50GB | 100+ |
| Starter | Standard choice for customers handling confidential information | Up to 3 | 5 | Up to 5 | 100GB | 200+ |
| Starter Plus | The same as Starter, without sharing the GPU | Up to 10 | 5 | Up to 5 | 100GB | 200+ |
| Business | Business-grade quality with 24B-class models | Up to 10 | 8 | Up to 7 | 200GB | 200+ |
| Business Plus | Customers who need a dedicated GPU and a separated environment | (see the pricing table on the official site) | 10 | Up to 10 | 500GB | 3,000+ |

- "Available models" is a rough figure: the number of models in the catalog that can be used on the plan, rounded down to the nearest 100. It changes over time.
- If you run out of training runs, you can add more at $5 (excluding tax, customers outside Japan) or ¥800 (excluding tax, customers in Japan) per run. Added runs are valid only within the 30-day period in which they were purchased and do not carry over to the next period.
- The 30-day training periods are counted from the start of your use (the day your environment was created). They are separate from billing periods; annual plans also use 30-day periods.

## Shared GPU vs. dedicated GPU

| Type | How it works | Response time (rough guide) |
|---|---|---|
| Shared GPU (Personal, Starter, Business) | One GPU is shared by multiple customers and requests are processed in order. Each customer's AI model is switched in as needed | A few seconds at the fastest. It may take a few minutes when models are being switched or when processing takes time |
| Dedicated GPU (Starter Plus, Business Plus) | The GPU is used by your company alone | Lower latency. However, the AI goes into standby after a period of no use, and the first response after resuming may take longer |

Response times are a rough guide and are not guaranteed.

## Example models

| Plan | Examples |
|---|---|
| Personal | Alibaba Cloud: Qwen3 4B / Google: Gemma 3 4B |
| Starter, Starter Plus | Alibaba Cloud: Qwen3 8B / Meta: Llama 3.1 8B |
| Business | Alibaba Cloud: Qwen3 14B / Google: Gemma 3 12B |
| Business Plus | Alibaba Cloud: Qwen3 32B / Google: Gemma 3 27B |

These are examples of representative models. The models actually available may change over time.

## Payment

- Monthly or annual (paid in advance)
- At the time of application, you can choose credit card payment or bank transfer
- Bank transfer is available only for customers in Japan (payment in Japanese yen). Transfer fees are borne by the customer
- Customers outside Japan pay by credit card
