# Example: spatial query

Use this workflow when the question is about a place rather than a single
entity: district, borough, neighborhood, ZIP code, precinct, school district,
radius, polygon, corridor, or address surroundings.

## Prompt

```text
What changed in this district over the last year?
```

## Best anchors

Start with one of:

- selected map boundary
- address or coordinate
- BBL
- radius
- polygon
- corridor
- time window

## Useful record groups

- boundary facts
- representative or officeholder context
- 311 and quality-of-life records
- housing or building condition records
- public money and capital projects
- permits, licenses, or regulated-location context when the question is
  business-oriented

## Good answer shape

```text
Name the selected scope.
Name the time window.
Start with bounded counts or summaries.
Only pull row-level records when the user asks for detail.
```

## Caveats

Large spatial datasets should always be bounded by scope and time. Empty
results should say which source and filters were checked.
