# Open Source and Product Boundary

Status: product/source strategy. Licensing is intentionally still pending.

ZumZum is intended to have a public, community-friendly surface without publishing the complete production business and trust stack.

The working model is **selective open-core**: open the parts where transparency, interoperability and community contribution create value; keep strategic production capabilities private where publishing them would make the complete service unnecessarily reproducible or weaken abuse defenses.

## Intended public surface

Candidate public components include:

- product and architecture documentation;
- protocol and interoperability specifications;
- public clients where practical;
- SDKs and integration contracts;
- plugin/extension interfaces;
- import/export tooling;
- identity formats and public API schemas;
- examples and reference implementations that do not expose production-sensitive logic.

Public components should be useful enough for developers to understand, integrate with and extend ZumZum.

## Intended private surface

Production-private components may include:

- complete production backend/core services;
- production infrastructure and deployment topology;
- secrets, credentials and operational configuration;
- detailed anti-abuse/fraud heuristics, thresholds and detection logic;
- internal trust/reputation systems;
- moderation and internal administration tooling;
- billing and commercial operations;
- private analytics and operational intelligence;
- proprietary data pipelines;
- RUNA and TUK internals that are not separately published.

Privacy and security must not depend on hiding broken cryptography or an insecure protocol. Public-facing security designs should remain reviewable where transparency improves safety; operational abuse defenses can still keep sensitive detection details private.

## Competitive principle

The public repository should make ZumZum easier to trust, integrate with and contribute to. It should not be a turnkey copy of the complete hosted business.

The durable advantage is expected to come from the network, product experience, brand, infrastructure, reliability, RUNA integration, business operations, trust/safety systems and the broader AERA ecosystem rather than from obscurity alone.

## Licensing

This repository is public, but a public repository is not automatically open source in the licensing sense.

No broad repository-wide license should be added until the public/private component boundaries are stable enough to choose licenses deliberately. Different public components may eventually use different licenses if that better protects the open-core strategy.

Until then, licensing remains an explicit product/legal decision rather than an accidental default.
