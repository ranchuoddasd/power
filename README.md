# Network Packet Latency Simulator

A standalone browser simulation that visualizes two packets moving across alternative multi-hop paths while displaying illustrative cumulative segment delay.

**Status:** Educational animation with synthetic topology and fixed sample delay values. It does not measure or generate real network traffic.

## Features

- Canvas-based multi-hop path visualization.
- Two animated paths for comparison.
- Cumulative sample delay labels.
- Pause, resume and reset controls.
- Adjustable animation speed.
- No build tools, backend or external runtime dependencies.

## Run

Open `index.html` in a modern browser. No installation or server is required.

## Project structure

```text
.
├── index.html
├── README.md
└── docs/
    └── simulation-design.md
```

## Simulation model

Each path is an ordered list of nodes. Each adjacent node pair has a sample delay value in milliseconds. The displayed cumulative value is the sum of completed segment delays plus the interpolated portion of the current segment.

Animation speed is a visual progression control. It is deliberately not calibrated to real elapsed network time.

## Limitations

- Paths, node positions and segment delays are fixed sample data.
- Canvas coordinates are diagram positions, not geographic coordinates.
- No ping, traceroute, packet capture, socket traffic or telemetry collection occurs.
- No packet loss, jitter, congestion, routing convergence or queueing behavior is modeled.
- No automated test suite is included.

## Security

The prototype runs locally in the browser and makes no network requests. It contains no credentials or external service integrations.

## Roadmap

1. Load path definitions from validated JSON.
2. Add packet loss, jitter and queueing as clearly defined simulation parameters.
3. Add deterministic simulation tests for cumulative delay.
4. Separate simulation state from canvas rendering.
5. Add accessible textual summaries of path state.

## License

No license is currently provided. Until a license is added, reuse and redistribution are not granted by default.
