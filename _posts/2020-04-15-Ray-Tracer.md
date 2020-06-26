---
layout: post
title:  "Ray Tracer"
author: Hanfei Chen
subtitle: "GLSL/C++"
categories: 
image: assets/images/ray-tracer.jpg
---

A ray tracer renders life-like images based on some physical rules for lights. I implemented a recursive ray tracer that uses the Blinn-Phong lighting model and supports reflections, refractions, shadows and anti-aliasing. I also implemented cube environment mapping to add skyboxes to the rendered scenes.

To make the rendered images more life-like, I added Monte-Carlo ray tracing to my ray tracer. In short, Monte-Carlo samples rays randomly across some area in space, and creates awesome effects like soft shadows, glossy reflection and depth of field.

Besides the ray tracer itself, I also added the feature to create animations and particle systems. By ray-tracing each frame, we get a wonderful short animation!
