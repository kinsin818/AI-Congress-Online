# AI Congress — Product Overview (public)

The product is **live** at https://aicongressonline.com. This page is the
public-facing overview; the publisher keeps a private release ledger and
deployment records.

## Platform

| Area | What it is |
|---|---|
| Core concept | Ask once, several AIs weigh in, you decide — multi-model chat with cross-verification. |
| File cleaning | CSV / XLSX / JSONL / JSON / PDF (table extraction) / DOCX cleaning and extraction engine with per-run auditable reports. |
| BYOK | Connect your own OpenAI-compatible endpoints; keys stay in your browser. |
| Plans | Guest (no signup trial) / Starter / Pro. Free tier: 10 chat reviews/day + 1 free file cleaning (≤5 MB). Paid: multi-file cleaning, cross-verification ($3/run), B2B data enrichment ($3/run). |
| Distribution | Web SaaS (no app store); live at aicongressonline.com. |

## Public roadmap (abridged)

- Real payment gateway integration (billing flow is already in place and
  covered by tests; a payment provider is being wired in).
- Larger-file tiers and multi-instance scale-out (Redis-based rate limiting and
  usage stats).
- Additional file formats and cleaning rule sets.

## Trust

- Production hardening: Cloudflare front (WAF + Turnstile), HTTPS-only, signed
  API routes, security headers.
- No-key-storage privacy model for BYOK users.
- Every cleaning run produces a human-readable report with operation-by-operation
  breakdown and cross-verification status.

## Repository boundary

This repository intentionally publishes **no source code, no configuration and
no infrastructure details**. If you are evaluating the publisher's engineering
capability, the live product, the screenshots and the portfolio PDF in this
repository are the evidence.