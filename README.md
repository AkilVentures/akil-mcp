# Akil Intelligence — NYC Civic Data MCP Server

<p align="center">
  <strong>92 tools · 57 verified data sources · 127M+ records</strong><br>
  Real New York City government data for AI agents and applications.
</p>

<p align="center">
  <a href="https://askakil.ai">Website</a> ·
  <a href="https://askakil.ai/mcp/docs">Tool Documentation</a> ·
  <a href="https://askakil.ai/pricing">Pricing</a> ·
  <a href="https://askakil.ai/privacy">Privacy</a>
</p>

---

## What is Akil Intelligence?

Akil Intelligence is the most comprehensive MCP server for New York City public data. Connect any MCP-compatible AI client and get verified, cross-referenced answers from 57 government data sources — including council funding, city contracts, lobbying records, campaign finance, building violations, property records, nonprofit filings, and more.

**Every answer is verified.** No guessing, no hallucination. Real numbers from real government databases, updated weekly.

## Quick Connect

**Endpoint:** `https://mcp.askakil.ai/mcp`
**Transport:** Streamable HTTP

### Claude Desktop

Add to your `claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "akil-intelligence": {
      "url": "https://mcp.askakil.ai/mcp"
    }
  }
}
```

### Claude Code

```bash
claude mcp add akil-intelligence --transport http https://mcp.askakil.ai/mcp
```

### Cursor

Add to `.cursor/mcp.json`:

```json
{
  "mcpServers": {
    "akil-intelligence": {
      "url": "https://mcp.askakil.ai/mcp"
    }
  }
}
```

### Any MCP Client

Point your client to `https://mcp.askakil.ai/mcp` using Streamable HTTP transport.

## What's Inside

92 intelligence tools organized into 5 pillars:

### 💰 Money (40 tools)
Trace every dollar through NYC government — from budget allocation to vendor payment.

- Grants, contracts, and procurement opportunities
- Agency budgets (adopted, modified, committed)
- Council discretionary funding by member and district
- Mayor, Speaker, Borough President, Comptroller allocations
- Vendor payments and spending trends
- Foundation giving profiles and recipients
- Nonprofit IRS 990 financials

### 🏢 Organizations (9 tools)
Complete dossier on any NYC organization — funding, audits, compliance, certifications.

- Cross-source org lookup (funding + audits + certifications + licenses)
- Federal audit history (material weaknesses, questioned costs)
- M/WBE certification status
- Nonprofit financial trends (multi-year)
- Business license verification

### 👤 People (10 tools)
Track political influence — campaign finance, lobbying, payroll, official contacts.

- Campaign contributions and expenditures (NYC CFB, 2001-2025)
- Lobbying registrations (NYC + NYS)
- Who lobbies which agency or council member
- Citywide payroll records (all agencies)
- Official directory (Green Book)
- Council member profiles (funding + legislation)

### 📍 Places (21 tools)
Complete neighborhood intelligence — violations, complaints, schools, housing, property.

- HPD housing violations and complaints
- DOB building permits and violations
- Property records (858K tax lots, PLUTO)
- School profiles and demographics
- 311 complaints and crime data
- Affordable housing developments
- Restaurant inspections
- Environmental data (air quality)
- Social services and shelter census

### ⚖️ Rules (7 tools)
Track legislation, zoning, regulations, and public hearings.

- Council bills and resolutions (1997-present)
- Land use and zoning (ULURP/ZAP)
- Agency rulemaking
- Public hearings and meetings

## Example Queries

Once connected, ask your AI client:

| Query | What you get |
|-------|-------------|
| "How much government funding has the YMCA received from NYC?" | Cross-referenced awards from 6+ agencies with exact dollar amounts |
| "Who are the top recipients of council discretionary funding?" | Ranked list with amounts, agencies, and fiscal years |
| "Who lobbies the Department of Education?" | Lobbying firms, clients, compensation, and subjects |
| "What HPD violations are open in the South Bronx?" | Class A/B/C violations with addresses, dates, and status |
| "Show me United Way's full profile" | Funding history, audit results, 990 financials, M/WBE status |
| "What NYC funding sources are open for youth programs?" | Active grants, contracts, and RFPs with deadlines |
| "Compare conditions in East Harlem vs Park Slope" | Demographics, complaints, violations, schools side by side |

## Data Quality

- **57 verified sources** — NYC, NYS, and Federal public records
- **127M+ records** indexed and normalized
- **Updated weekly** from live government APIs
- **Cross-referenced** — a single query checks multiple databases
- **Source attribution** — every response cites its sources
- **Gap detection** — tells you what data is missing, not just what exists

## Who Uses Akil

- **Nonprofit leaders** — Track government funding across all agencies
- **Grant writers** — Find opportunities, check eligibility, monitor deadlines
- **Council staff** — District-level intelligence for constituent services
- **Journalists** — Follow the money, cross-reference political connections
- **Lobbyists** — Council member profiles, legislation tracking, competitive landscape
- **Developers** — Build custom civic data tools on our infrastructure

## Pricing

| Tier | Price | Includes |
|------|-------|---------|
| **Free** | $0 | Full access to all 92 tools |
| **Pro** | $79/mo | Real-time alerts, watchlists, exports |
| **Professional** | $199/mo | Deep analysis mode, MCP API key, custom reports |
| **Enterprise** | Custom | Custom AI agents, integrations, white-label |

[View full pricing →](https://askakil.ai/pricing)

## Links

- 🌐 **Product:** [askakil.ai](https://askakil.ai)
- 📖 **Tool Documentation:** [askakil.ai/mcp/docs](https://askakil.ai/mcp/docs)
- 🏢 **Company:** [akilventures.com](https://akilventures.com)
- 🔒 **Privacy:** [askakil.ai/privacy](https://askakil.ai/privacy)
- 📄 **Terms:** [askakil.ai/terms](https://askakil.ai/terms)
- 𝕏 **X/Twitter:** [@akilNYC](https://x.com/akilNYC)

## About

Built by **Akil Ventures, Inc.** — a Delaware corporation building civic intelligence tools for New York City.

## License

MIT
