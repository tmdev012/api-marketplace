# API Marketplace

> Self-hosted API marketplace — register APIs, manage keys (JWT/OAuth2), rate limiting, usage analytics, developer portal with auto-generated docs.

[![FastAPI](https://img.shields.io/badge/FastAPI-0.100+-green)]()
[![JWT](https://img.shields.io/badge/Auth-JWT+OAuth2-blue)]()
[![Redis](https://img.shields.io/badge/Rate_Limit-Redis-red)]()

## Architecture

```
Developer Portal ──▶ API Registration ──▶ Key Management
                                              │
Consumer ──▶ API Gateway ──▶ Auth (JWT) ──▶ Rate Limit ──▶ Backend
                │                                              │
                ▼                                              ▼
         ┌──────────┐                                  ┌──────────┐
         │  Usage   │                                  │ Response │
         │ Tracking │                                  │ + Cache  │
         └──────────┘                                  └──────────┘
                │
                ▼
         ┌──────────┐
         │ Billing  │──▶ Invoice per API key per month
         └──────────┘
```

## Pricing Tiers

| Tier | Rate Limit | Price | Features |
|------|-----------|-------|----------|
| Free | 100 req/day | R0 | Basic auth, community support |
| Pro | 10K req/day | R299/mo | Priority routing, analytics dashboard |
| Enterprise | Unlimited | R2,999/mo | SLA, dedicated support, custom domains |

## Revenue

White-label marketplace **R10,000 setup + R2,000/month**. Or host your own APIs and charge per call. Every API call is tracked and billable.

---
*MIT License*
