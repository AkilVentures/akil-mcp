# Example: nonprofit due diligence

Use this workflow when someone asks about a nonprofit, fiscal sponsor, vendor,
service provider, grantee, or organization receiving public money.

## Prompt

```text
Run source-backed due diligence on this organization.
```

## Best anchor

Start with one of:

- EIN
- legal organization name
- DBA or known alias

## Useful record groups

- organization lookup and aliases
- IRS 990 profile where available
- NYS nonprofit registry context where available
- award and funding history
- contract and payment records
- federal audit records where applicable
- compliance flags where available
- lobbying or campaign-finance context only when relevant to the question

## Good answer shape

```text
Identify the organization first.
Separate exact matches from possible fuzzy matches.
For every status claim, say which source was checked and whether a record was
found.
```

## Caveats

No record found in one public source is not the same thing as proof that the
underlying fact is false. Nonprofits may be below thresholds that trigger some
audit or filing datasets.
