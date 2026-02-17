# LOGOS
LOGOS publishes public interfaces (API specifications, SDKs, and operational templates) for integration and evaluation. Core execution and security‑critical components are proprietary and available only via controlled access (NDA/audit).
# LOGOS — Public Interface / Protected Core

LOGOS is an infrastructure-grade L1 system with a **Protected Core** design:
we publish public interfaces and operational guidance for integration and evaluation,
while keeping security-critical internals proprietary.

## What is public here
This repository contains:
- Public documentation (architecture principles, threat model, disclosure policy)
- Public API surface (redacted OpenAPI for integration)
- Non-production infrastructure templates (sanitized)
- Contribution & security reporting process

## What is NOT in this repository
This repository does NOT include:
- Core execution engine / consensus / security-critical internals
- Any production configuration, internal topology, real domains/IPs
- Any secrets (keys, tokens, seed phrases, HMAC/JWT, vaults)
- Any partner-only/internal endpoints

## Protected Core Disclosure
LOGOS publishes public interfaces (APIs, docs, templates) to enable integration and independent
verification of **observable behavior**.

Core execution and security-critical components are proprietary and available only via a controlled
access path (NDA / security review) to protect IP and preserve network security.

➡ NDA / partner access: see `docs/05-partner-nda-process.md`

## Quick links
- Publishing policy: `docs/01-publishing-policy.md`
- Architecture principles: `docs/02-architecture-principles.md`
- API surface: `docs/03-api-surface.md`
- Threat model: `docs/04-threat-model.md`
- Security reporting: `SECURITY.md`

## Status
- Core: operational (proprietary)
- Public interface: stabilizing (this repo)
- Wallet/Explorer: production-grade internally, public packaging is staged
