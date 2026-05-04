# Connect Akil MCP to Claude

Akil is a hosted MCP server. You do not need to install this package to use it
from Claude.

## Endpoint

```text
https://mcp.askakil.ai/mcp
```

## Claude.ai

1. Open Claude settings.
2. Go to connectors or custom connectors.
3. Add a custom MCP connector.
4. Paste the Akil MCP endpoint.
5. Complete the Akil authorization flow when prompted.

Once connected, ask normally. Claude can discover Akil tools, read guide
resources, and call the right public-record workflows.

## Claude Desktop or local MCP clients

Use a streamable HTTP MCP configuration pointing at the hosted endpoint:

```json
{
  "mcpServers": {
    "akil": {
      "url": "https://mcp.askakil.ai/mcp"
    }
  }
}
```

Client support for remote MCP and OAuth varies. If your client cannot complete
the browser authorization flow, use an approved API key as a bearer token.

## Good first prompts

```text
I am looking at a storefront lease. What records should I check before signing?
```

```text
Who owns this building, and what permits or violations should I check next?
```

```text
Show public funding and contracts tied to this organization.
```
