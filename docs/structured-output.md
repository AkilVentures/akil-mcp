# Structured output

Akil responses are designed for both human-readable answers and agent-friendly
follow-up work.

Depending on the workflow and client, a response may include:

- text summary
- source and freshness notes
- reusable anchors
- table-oriented records
- map-ready geometry or coordinates
- chart-ready counts or time series
- suggested next checks

## Common anchors

| Anchor | Use |
|--------|-----|
| `BBL` | Tax lot, property, permits, deeds, sales, tax records, violations |
| `EIN` | Nonprofit filings, audits, awards, organization checks |
| `Agency` | Budgets, contracts, payments, rules, hearings |
| `District` | Place-based government, funding, complaints, conditions |
| `License` | Regulated business status, applications, inspections |
| `Time window` | Keeps large datasets bounded and usable |

## How agents should use the output

1. Preserve the anchor returned by the first call.
2. Reuse it in follow-up calls instead of restarting from text search.
3. Respect source and time-window caveats.
4. Treat empty results as a finding, not as proof that the underlying fact is
   false.
5. Ask narrower follow-up questions when a broad source times out or returns too
   much data.

## Example answer shape

```text
Tax lot: BBL 4063230022
Selected address: 220-15 Northern Boulevard
PLUTO tax-lot address: 220-11 Northern Boulevard
Queens (Borough 4) | Block 6323 | Lot 22

Records checked:
- Tax-lot identity
- Owner field
- Suggested next checks: permits, violations, recorded documents
```
