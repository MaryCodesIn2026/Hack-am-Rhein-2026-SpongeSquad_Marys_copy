# Wrapper and integration

Home for Achim's work bringing the SpongeSquad modules together.

This folder contains the complete latest state consolidated from the fork's `feature/street-lab-ui` branch:

- `docs/ARCHITECTURE.md` — product spine, module boundaries and integration contract;
- `prototypes/sponge-street/` — original standalone explainer;
- `street-workspace/` — latest React, TypeScript and Phaser Street Lab.

That source already includes the structured street-world work and subsequent UI improvements, so older overlapping branch versions are not duplicated.

## Integration boundary

Andy's hot-spot finder remains unchanged on `feature/hot-spot-map`. The intended seam is:

```text
CandidateArea
→ example StreetScenarioSeed
→ Street Lab
→ explanation and comparison
```

Integration must not turn illustrative area scores into measured street geometry, soil or drainage facts.
