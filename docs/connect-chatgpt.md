# Connect Akil MCP to ChatGPT

Akil is designed for remote MCP-compatible clients. ChatGPT connector support
may vary by workspace, account type, and product availability.

## Endpoint

```text
https://mcp.askakil.ai/mcp
```

## Setup

1. Open ChatGPT settings or workspace connector settings.
2. Add Akil as a custom MCP connector if custom connectors are available.
3. Paste the Akil MCP endpoint.
4. Complete the Akil authorization flow when prompted.

If custom remote MCP connectors are not available in your ChatGPT environment,
you can still use Akil through other MCP-compatible clients or a custom agent
framework.

## What to expect

Akil returns text plus structured metadata where supported. Modern AI clients
may render parts of the result as tables, maps, charts, citations, or follow-up
actions depending on the client.

## Example prompts

```text
Use Akil to check public records for this BBL.
```

```text
What public money records are tied to this agency and organization?
```

```text
Find records connected to this district over the last year.
```
