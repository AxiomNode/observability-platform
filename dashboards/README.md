# Dashboards

Last updated: 2026-05-03.

## Purpose

Dashboards by service and business domain.

## Scope

## Available

- [`ai-engine-llmops.json`](./ai-engine-llmops.json) — LLMOps panel for `ai-engine` (ADR 0009). Tracks `ai_engine_llm_latency_seconds`, `ai_engine_llm_latency_p95_seconds`, `ai_engine_llm_fallback_total`, `ai_engine_llm_tokens_total{direction}`, `ai_engine_llm_errors_total{kind}`, plus success and retry rate. Imports as a Grafana dashboard JSON; pick a Prometheus datasource at import time.
