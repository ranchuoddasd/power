# Simulation Design

## Purpose
Demonstrate packet progression across a multi-hop path and show how per-segment delay values contribute to a cumulative illustrative value.

## Model
- Each path is an ordered list of node identifiers.
- Each adjacent node pair maps to a sample delay in milliseconds.
- A packet tracks its current segment, fractional progress and completed delay.
- Cumulative delay is completed segment delay plus the interpolated delay on the active segment.
- When a packet reaches the final node, the visual cycle resets.

## Controls
- **Pause / Resume:** stop or continue visual progression.
- **Reset:** return both packets to the start and resume.
- **Animation speed:** change visual progression rate without changing the configured sample delay values.

## Rendering
Canvas draws the topology, node labels, packet markers and cumulative sample-delay labels. The animation loop uses requestAnimationFrame and caps large frame deltas to reduce jumps after a suspended tab.

## Caveats
- Animation speed is not a physical timing model.
- Sample delay values are not measurements.
- The prototype does not transmit packets or query network devices.
- It does not model packet loss, jitter, queueing or congestion.

## Future work
Load validated path data from JSON, add deterministic tests for cumulative calculations, and keep simulation logic independent from rendering.
