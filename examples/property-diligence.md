# Example: property diligence

Use this workflow when someone asks about a building, house, tax lot, storefront,
owner, permit status, violation history, sales history, or recorded documents.

## Prompt

```text
Who owns this building, and what public records should I check next?
```

## Best anchor

Start with one of:

- BBL
- address
- borough/block/lot

## Useful record groups

- PLUTO tax-lot identity
- selected address versus tax-lot address
- borough, block, and lot
- recorded owner
- ACRIS recorded documents
- DOF sales
- DOB permits and jobs
- HPD/DOB/OATH violations where relevant
- tax liens, assessments, exemptions, or charges where relevant

## Good answer shape

```text
TAX LOT | BBL 4063230022
Selected address: 220-15 Northern Boulevard
PLUTO tax-lot address: 220-11 Northern Boulevard
Queens (Borough 4) | Block 6323 | Lot 22

Then show owner, building class, land use, records checked, caveats, and next
checks.
```

## Caveats

The recorded owner field is not beneficial ownership, title-chain analysis, or
legal advice. A storefront or alternate address can share a BBL with a different
tax-lot address.
