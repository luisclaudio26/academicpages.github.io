---
title: "Rendering engine"
excerpt: "Software implementation of the graphics pipeline<br/><img src='/images/re_cow.png'>"
collection: portfolio
---

This is a software renderer which tries to emulate the OpenGL API, so you will find that
uniform uploading, vertex attributes definition, texture mapping and vertex/fragment shader
programming is very similar to what one would do in OpenGL. It uses
[NanoGUI](https://nanogui.readthedocs.io) for window management and
[TinyObjLoader](https://github.com/syoyo/tinyobjloader) for .OBJ handling.

Make sure to check my [voxel ambient occlusion](https://luisclaudio26.github.io/VAO) project,
which was coded entirely within this lil' software renderer.

[Source code](https://github.com/luisclaudio26/RenderingPipeline)

<img src='/images/re_cow.png'>

_A bronze Cow rendered in software (background) vs. OpenGL rendering (small window in bottom
left). ~24 FPS._

<img src='/images/re_normals.png'>

_The well-known [Breakfast room](http://casual-effects.com/data/) scene rendered using
Normal shading._

<img src='/images/re_voxels.png'>

_The Stanford Bunny model drawn using a raycasting shader for voxel rendering._
