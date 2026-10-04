# Identity and Trust

ZumZum should separate technical account identity from public contact identity.

## Identity layers

```text
Account
  |
  +-- Internal Account ID (immutable, private)
  |
  +-- ZumID (public, rotatable)
  |
  +-- @handle (human-readable alias, optional)
  |
  +-- temporary invite/contact links (revocable)
```

### Internal Account ID

A permanent internal identifier used by the platform. It is never intended to be shared publicly and does not change when the user rotates a ZumID or handle.

### ZumID

A public contact identifier that can be copied, shared or represented as a QR code. Users can regenerate it without losing conversations, groups, contacts, verification state or account history.

Rotation must be rate-limited to reduce fraud and spam. The old ZumID stops accepting new contact requests after rotation. Pending requests and old invite links can optionally be revoked at the same time.

### @handle

A readable alias such as `@rogerio` or `@docesdamaria`. Handles may be free in generated/basic form and paid when the user wants a short/custom/premium identity.

Paying for a handle never makes the account verified.

### Temporary contact links

Users should be able to create revocable links with limits such as:

- expires in 1 hour / 24 hours / 7 days;
- expires after N uses;
- valid until manually revoked.

This is useful for livestreams, public posts and events where sharing a permanent contact identifier is undesirable.

## Account bootstrap

Preferred initial direction:

- unique account identity;
- verified email for recovery/contact;
- passkey strongly preferred, potentially required for higher-trust actions;
- device/risk signals;
- new-account anti-spam limits.

Disposable-email domain detection can be one risk signal, but it must not be the only defense because disposable domains change constantly.

## Verification

Verification means authenticity/trust, not subscription status.

Possible future levels:

- basic account: email/passkey and standard platform controls;
- trusted account: established account/device history and low-abuse reputation;
- verified identity: stronger identity verification, potentially document + selfie/liveness through a specialized provider.

Raw biometric/document data should be minimized and preferably processed by a dedicated identity provider. ZumZum should retain only what is necessary to prove the verification result, subject to legal/privacy review.

## Non-negotiable principle

**Features can be purchased. Trust must be earned or verified.**
