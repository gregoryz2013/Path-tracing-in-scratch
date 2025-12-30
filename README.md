# Ray Casting, Ray Tracing, and Path Tracing in Scratch

## Overview

This repository contains three separate Scratch projects demonstrating the core concepts of **ray casting**, **ray tracing**, and **path tracing**. Each file represents a standalone implementation focused on a specific rendering technique.

The goal of this repository is educational: to show how modern rendering principles can be approximated inside the limitations of the Scratch environment.

The project also includes a **3D FBM (Fractal Brownian Motion)** noise implementation adapted from Blender’s open‑source codebase.

---

## Project Structure

```
/raycasting.sb3   – Basic ray casting implementation
/raytracing.sb3   – Ray tracing with lighting and reflections
/pathtracing.sb3  – Stochastic path tracing renderer
```

Each file is independent and can be opened and executed separately.

---

## Controls

| Key               | Action                                          |
| ----------------- | ----------------------------------------------- |
| **W / A / S / D** | Camera movement                                 |
| **Arrow Keys**    | Fine camera rotation and orientation adjustment |
| **I**             | Start rendering                                 |

---

## Ray Casting

The ray casting implementation provides the foundation for all other techniques.

Features:

* Per-pixel ray projection
* Scene intersection testing
* Basic depth perception

This stage does not simulate lighting or reflections. It is primarily used to visualize geometry and camera behavior.

---

## Ray Tracing

The ray tracing implementation extends ray casting by introducing:

* Surface lighting evaluation
* Reflection rays
* Basic material response

This version simulates direct illumination and reflective surfaces, allowing for more realistic results compared to simple ray casting.

---

## Path Tracing

The path tracing implementation uses stochastic sampling to approximate global illumination.

Key characteristics:

* Randomized ray directions
* Multiple light bounces
* Progressive light accumulation
* Noise reduction through averaging

Due to Scratch limitations, the implementation is simplified but follows the same conceptual model used in modern path tracers.

---

## 3D FBM Noise

The renderer uses **3D Fractal Brownian Motion (FBM)** for procedural variation.

Details:

* Based on Blender’s open-source noise implementation
* Adapted to Scratch constraints
* Multiple octaves with frequency and amplitude scaling
* Used for surface variation and shading

This significantly improves visual complexity compared to simple random noise.

---

## Tone Mapping

A basic tone mapping operator is applied to convert high dynamic range lighting into displayable color values.

Purpose:

* Prevent overexposure
* Preserve contrast
* Maintain visual readability

The tone mapping is intentionally simple and optimized for clarity rather than physical accuracy.

---

## Notes and Limitations

* Performance is limited by Scratch’s execution model
* Rendering is not real-time
* Accuracy is secondary to clarity and educational value
* Designed for experimentation and learning

---

## Purpose

This repository demonstrates how core rendering techniques can be implemented in a constrained environment. It is intended for:

* Learning ray-based rendering concepts
* Understanding path tracing fundamentals
* Exploring procedural noise
* Experimenting with rendering pipelines in Scratch

