# Migration from Other Messengers

A new messenger has a major adoption barrier: users already have years of contacts, groups and history elsewhere. ZumZum should reduce the feeling of starting from zero.

## Preferred migration model

Where technically and legally allowed, prefer user-controlled exports rather than credential scraping or unofficial access to another service account.

Potential imports:

- contacts;
- conversation exports;
- group names/metadata where available;
- media/files included by the user's export;
- timestamps;
- business customer lists and labels when supported by an official export format.

## Provenance

Imported history must remain distinguishable from native ZumZum messages. The UI/data model should be able to represent that a message originated from an external import rather than pretending it was sent through ZumZum.

## Safety

- never ask users for another messenger's password;
- never depend on scraping private APIs as a core migration strategy;
- parse imports defensively;
- scan/archive imported files according to security policy;
- let users choose what to import;
- provide deletion/rollback of an import where feasible.

## Business opportunity

Migration is especially valuable for businesses: importing customer context can lower the switching cost before the business starts using ZumZum + RUNA as its primary communication workflow.
