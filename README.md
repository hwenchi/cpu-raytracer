# CPU Raytracer

![](https://github.com/GalMunGral/cpu-raytracer/blob/main/examples/ex0.jpg?raw=true)

## Rhetorical Design

### Purpose

3D rendering admits two dual formulations: iterate over primitives and determine which pixels each covers, or iterate over pixels and determine which primitive each ray hits first. Rasterization takes the former; ray tracing takes the latter. This project, intended for an audience familiar with rasterization, implements ray tracing on the CPU.

### Strategy

The sequential nature of a CPU implementation makes the performance bottleneck self-evident, motivating [gl-raytracer](https://github.com/GalMunGral/gl-raytracer), which achieves real-time performance by mapping the same computation onto the GPU. Example outputs are included to demonstrate correctness.