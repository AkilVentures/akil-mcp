# Example: business location check

Use this workflow when someone is evaluating a storefront, restaurant, cafe,
retail space, cannabis-adjacent location, liquor-related location, tobacco/vape
location, sidewalk cafe, or other regulated local business.

## Prompt

```text
I am looking at a storefront lease at this address. What public records should
I check before signing?
```

## Best anchor

Start with one of:

- street address
- BBL
- license or application number, if known

## Useful record groups

- tax-lot identity and selected address
- current and historical permits
- inspections and complaints
- food, liquor, tobacco, cannabis, sidewalk cafe, or other license context where
  relevant
- district and nearby public-record context
- time-windowed quality-of-life records

## Good answer shape

```text
Start with the tax lot and selected address.
Then separate building records from operator/license records.
Then show which records returned data, which did not, and what to check next.
```

## Caveats

Akil provides public-record retrieval and context. It does not replace legal,
architectural, expediting, licensing, or code-compliance advice.
