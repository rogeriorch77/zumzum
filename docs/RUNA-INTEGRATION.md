# RUNA Integration

RUNA can become a native intelligence layer inside ZumZum without turning every conversation into an AI conversation.

## Personal use

Possible explicit interactions:

- `@Runa translate this to French`;
- summarize a long conversation when the user requests it;
- explain a message or technical term;
- draft a reply;
- organize information the user explicitly asks RUNA to process.

RUNA should not silently read or act on private chats merely because it exists in the platform.

## Business use

RUNA Sales can help a verified business with:

- customer-service responses;
- catalog/product questions;
- lead qualification;
- handoff to human staff;
- office-hours behavior;
- bounded follow-up;
- approved automation and integrations.

The business policy layer remains distinct from the model itself.

## Channel independence

The long-term architecture can let the same business RUNA workflow serve:

```text
ZumZum
WhatsApp (approved external integration)
Web chat
other approved channels
        |
        v
      RUNA
        |
 business policy / tools / intelligence
```

This reduces product dependence on any single external messaging channel while preserving the channels customers already use.

## Privacy boundary

RUNA access should be explicit and scoped. Model providers, TUK and tools receive only the context required for the approved task. Platform credentials never enter model-visible content.
