# Connect Akil MCP to Codex or custom agents

Akil is a remote MCP server. Developer and partner integrations should treat it
as a hosted endpoint, not as a local package to run.

## Endpoint

```text
https://mcp.askakil.ai/mcp
```

## Authorization

Interactive users can authorize through the client when the MCP connection is
created.

Backend jobs and partner integrations can send an approved API key as a bearer
token:

```text
Authorization: Bearer <AKIL_API_KEY>
```

Do not hard-code API keys in source code. Store them in your runtime secret
manager or environment configuration.

## Minimal connection shape

```json
{
  "url": "https://mcp.askakil.ai/mcp",
  "transport": "streamable-http",
  "headers": {
    "Authorization": "Bearer <AKIL_API_KEY>"
  }
}
```

Only include the authorization header if you are using an approved backend API
key. Interactive OAuth clients should let the user sign in through the client.

## Developer workflow

1. Connect the endpoint.
2. Let the agent discover tools and guide resources.
3. Start with an anchor when possible: address, BBL, EIN, agency, district,
   license, or time window.
4. Ask for the specific record set or workflow.

## Example

```text
Use Akil to evaluate this location for a food business. Start with address,
tax-lot identity, permits, inspections, liquor/cafe/license context, and recent
quality-of-life records.
```
