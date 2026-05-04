# Authentication

Akil supports two common access patterns.

## Interactive user authorization

Use this when a person connects Akil from an AI client such as Claude, ChatGPT,
Codex, or another MCP-compatible workspace.

The client opens the Akil authorization flow, the user signs in, and the client
receives access for that session.

## API keys for backend integrations

Use this when a trusted backend, scheduled job, or partner application needs to
call Akil without an interactive user in the loop.

Send the approved key as a bearer token:

```text
Authorization: Bearer <AKIL_API_KEY>
```

Do not paste real keys into GitHub issues, public examples, browser console
snippets, or shared chat transcripts.

## Access model

Access may be reviewed, rate-limited, or scoped depending on the use case.
Contact [hello@akilventures.com](mailto:hello@akilventures.com) for partner or
developer access.

## Sensitive data

Akil is designed around public records. Users should still avoid submitting
private credentials, private notes, or sensitive personal documents unless they
understand how their chosen AI client handles that data.
