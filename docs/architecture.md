# Architecture Notes

This document provides enough technical context to evaluate the project without exposing the production implementation.

## 1. Editorial intake

A content job begins with a structured topic, business question or editorial brief rather than an unrestricted generation request. The job retains status as it moves through the production lifecycle.

## 2. Research and source preparation

The workflow prepares source material before drafting. The production system prioritizes authoritative and primary material and treats unverified claims differently from confirmed information.

## 3. AI-assisted drafting

AI supports drafting, restructuring and enrichment. It is used as an editorial production component rather than as an autonomous publisher.

## 4. Quality and factual controls

Drafts pass through checks designed to surface missing attribution, weak sourcing, stale figures, structural problems and other conditions that require revision or human judgement.

## 5. SEO, links and media

SEO metadata, internal-link opportunities and media requirements are prepared as a separate stage so that publication readiness is not determined by text generation alone.

## 6. Human editorial approval

A human editor remains responsible for accepting, revising or rejecting the content before it can advance to publication stages.

## 7. WordPress integration

Approved material is transferred into the publishing environment with structured metadata. The public showcase intentionally omits authentication, endpoints, plugin internals and publishing payloads.

## 8. Pre-publication QA

The workflow verifies required publication elements before final approval. Failed requirements stop progression rather than being silently ignored.

## 9. Review lifecycle

Time-sensitive content can be revisited after publication so that changing economic, company or market information does not remain indefinitely unreviewed.

## Technical patterns demonstrated

- modular workflow stages
- persistent content/job state
- human-in-the-loop approvals
- WordPress/API integration
- structured validation gates
- source-aware AI usage
- SEO workflow integration
- safe stop conditions
- staged testing and release discipline
- migration from fragmented legacy automation toward maintainable services

## Deliberately omitted

- production plugin structure and PHP source
- n8n workflow exports
- request/response schemas
- prompts and editorial instructions
- real endpoints and authentication
- internal content taxonomy
- exact verification rules
- scoring and prioritization formulas
- provider/model configuration
- production data

These implementation details remain private and may be discussed only within an appropriate client engagement.
