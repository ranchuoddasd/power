# Network Packet Latency Simulator

A standalone browser animation demonstrating packets moving through a multi-hop path while cumulative latency changes along each segment.

**Status:** Static simulation. The path, segment delays, and locations are illustrative; this is not a real packet capture or network measurement.

## Features
- Canvas-based packet movement across a multi-hop path.
- Two animated paths for visual comparison.
- Per-segment delay values and cumulative latency labels.
- Simple standalone HTML; no build tooling required.

## Run
Open `index.html` in a modern browser.

## Project files
- `index.html` — animation, topology coordinates, sample latency data, and rendering loop.

## Limitations
- Fixed sample path and delay values.
- Canvas coordinates do not represent geographic positions.
- UI buttons are demonstration placeholders.
- No actual network traffic, probes, or telemetry are generated.
- Animation speed is illustrative and does not model latency in real time.

## Roadmap
- Configure path nodes and delays through JSON.
- Add pause, reset, and playback-speed controls.
- Add a legend and clear latency calculation explanation.
- Test segment timing and cumulative latency calculations.

## Security
No external services, credentials, or network requests are required by the prototype.

## License
No license is currently provided. Until one is added, reuse and redistribution are not granted by default.
