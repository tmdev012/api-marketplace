# ADR-001: Self-Hosted API Gateway Over AWS API Gateway

## Status: Accepted | Date: 2026-02-10

## Decision
Build self-hosted API gateway rather than using AWS API Gateway.

## Why
- AWS charges per million requests + data transfer
- Self-hosted = fixed cost (server only), unlimited requests
- Full control over auth, rate limiting, analytics
- Can white-label and resell
