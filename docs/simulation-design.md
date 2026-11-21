# Simulation Design

## Model
Each simulated traveler follows a node sequence. A segment delay controls the animation progression, and the display adds the completed segment delays to the current segment's interpolated delay.

## Rendering
Canvas draws node markers, path lines, animated packet markers, and cumulative-delay labels. The animation loop uses browser animation frames.

## Caveats
- Delay is used as an animation progression parameter, not as a calibrated physical timing model.
- Coordinates are a drawing layout.
- The simulation does not transmit packets or query devices.

## Next
Make path configuration data-driven, correct/clarify animation timing, and add automated checks for cumulative values.
