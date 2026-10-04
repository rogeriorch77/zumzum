# Security and Abuse Direction

ZumZum's identity flexibility must not become an abuse tool.

## Layered anti-abuse

Signals may include:

- verified email;
- passkey/device trust;
- account age;
- rate limits for new accounts;
- IP/network abuse signals;
- known disposable-email domains;
- repeated account creation patterns;
- unsolicited-message behavior;
- report/block history;
- ZumID/handle rotation frequency.

No single signal should be treated as proof of abuse.

## Identifier rotation

Rotating a ZumID is primarily a privacy/safety feature. Controls should prevent rapid rotation from being used to escape reports or spam limits. Internal Account ID and enforcement history remain stable even when public IDs change.

## Discovery controls

Users should be able to control whether they can be discovered by:

- ZumID;
- handle;
- temporary link;
- mutual contacts/groups;
- other future discovery surfaces.

Blocking a person should be bound to the internal account relationship, not only to a replaceable public ID.

## Strong identity verification

Photo/document/liveness verification may be offered for higher-trust use cases. It should use data minimization, explicit purpose and specialized providers. Verification must not be required for ordinary private messaging unless a future legal/risk requirement makes it necessary.

## Business identity

Business verification should validate the formal business registration and authorized responsible party. In Brazil, the first target is active CNPJ validation; provider and legal implementation remain an explicit research/integration decision.
