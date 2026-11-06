# Simulations

A collection of simulations for learning software engineering and distributed systems.

[Open the simulations homepage](https://tharunworks.github.io/simulations/)

## Simulations

| Simulation | Topics | Launch |
| --- | --- | --- |
| S3 Multipart Upload | Part sizes, checksum modes, signatures, and failure scenarios | [Open](https://tharunworks.github.io/simulations/s3-multipart-upload/) |

| Manifest Quest | HLS manifests, bitrate selection, buffering, CDN cache hits and S3 request flow | [Open](https://tharunworks.github.io/simulations/manifest-quest/) |
| Online Chess: Consistency vs Availability | Multi-device conflicting moves, CAP, stale replica reads, partitions, failover and fencing | [Open](https://tharunworks.github.io/simulations/chess-cap/) |

## Chess CAP note

A player using two devices can submit competing moves. For example, Alice's laptop submits `e2e4` to Server A while her phone submits `d2d4` to Server B. During a network partition, independently writable servers can each believe it is White's turn and acknowledge conflicting moves. The simulation demonstrates this issue, a single-authoritative-writer design, stale asynchronous PostgreSQL reads, and unsafe failover.

## Structure

- `chess-cap/index.html`: stepwise chess CAP simulation and learning notes.
- `manifest-quest/index.html`: streaming and manifest simulation.
- `index.html`: collection homepage.
- `s3-multipart-upload/index.html`: S3 multipart upload simulation.

## Adding a simulation

1. Create a folder with a URL-friendly name and put its entry page in `index.html`.
2. Add a card linking to it from the root `index.html`.
3. Add it to the table above.
4. Include a link back to `../` in the simulation.

GitHub Pages publishes the root of `main`. The simulations run in the browser; no build step is required.

The original S3 simulator repository and URL remain available.
