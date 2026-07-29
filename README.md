# Atlas Omega

Atlas Omega is an interactive spatial computing research build that combines
hand tracking, real time graphics, and physically responsive visual systems.

The current repository preserves two working WebGL experiments while a more
rigorous uncertainty aware planetary observatory is designed around them.

## What Exists Today

* V2 hand tracking experiment with temporal filtering
* V3 compositor and physics experiment
* MediaPipe hand landmark integration
* Three.js visual environment
* Rapier based physics components
* deterministic demo mode for repeatable review
* forensic notes covering known camera, smoothing, occlusion, replay, and
  rendering limitations

## Why This Project Exists

Atlas explores a question that sits between computer vision and spatial
interfaces:

> How can uncertain perception drive an expressive interactive system without
> pretending that every estimate is correct?

The long term direction is a planetary observatory where observations,
uncertainty, provenance, and rendering remain distinct.

## System Boundary

```text
Observed hand landmarks
          ↓
Temporal filtering and confidence
          ↓
Interaction intent
          ↓
Physics and scene state
          ↓
WebGL rendering
```

The boundary matters because a rendered effect is not evidence that the
underlying perception is correct. Future modules must preserve the distinction
between observation, interpretation, simulation, and presentation.

## Verification

The private source baseline passed its JavaScript syntax check and HTTP smoke
check on 29 July 2026. The V3 demo also rendered successfully in a browser.

This confirms that the legacy experiment runs. It does not claim that the future
scientific observatory is complete or that the preserved perception behavior is
scientifically validated.

## Source Availability

The complete source remains in a private development repository while model,
texture, dataset, and source provenance are reviewed. This public repository is
the project overview and evidence boundary, not a runnable source release.

## Known Gaps

* camera and demo modes do not yet share one reproducible input contract
* confidence and uncertainty are not fully surfaced in the interface
* occlusion and rapid motion can destabilize landmark driven interactions
* replay and deterministic evaluation require stronger separation from rendering
* the planetary observatory modules remain a roadmap, not a completed instrument

## Next Technical Milestones

* define typed observation and uncertainty records
* introduce deterministic replay fixtures
* separate perception, interaction, physics, and rendering modules
* add measurable hand tracking stability benchmarks
* complete provenance and licensing review for every distributed asset

## Research Boundary

Atlas treats the visual demo as an experimental interface, not as scientific
evidence. Future scientific modules must expose source provenance, timestamps,
coordinate frames, uncertainty, and failure states explicitly.

## Rights

No open source license is granted yet. Model, texture, dataset, and source
provenance must be resolved before public redistribution.
