# Simulations

A collection of simulations for learning software engineering and distributed systems.

[Open the simulations homepage](https://tharunworks.github.io/simulations/)

## Simulations

| Simulation | Topics | Launch |
| --- | --- | --- |
| S3 Multipart Upload | Part sizes, checksum modes, signatures, and failure scenarios | [Open](https://tharunworks.github.io/simulations/s3-multipart-upload/) |

## Structure

- `index.html`: collection homepage.
- `s3-multipart-upload/index.html`: S3 multipart upload simulation.

## Adding a simulation

1. Create a folder with a URL-friendly name and put its entry page in `index.html`.
2. Add a card linking to it from the root `index.html`.
3. Add it to the table above.
4. Include a link back to `../` in the simulation.

GitHub Pages publishes the root of `main`. The simulations run in the browser; no build step is required.

The original S3 simulator repository and URL remain available.
