---
title: "Voxel ambient occlusion"
excerpt: "Raytraced ambient occlusion using voxels<br/><img src='/images/vao_breakfastroom_ao.png'>"
collection: portfolio
---

This was my final project for the Computer Graphics course as an MSc. student at UFRGS.
The goal was to experiment how voxel representations of a scene can be used to
compute effects typically used in raytracing engine, ambient occlusion being the simplest
I could come up with.

It works by computing a voxel representation of the scene (inspired by the work of
[Crassin et al](http://maverick.inria.fr/Membres/Cyril.Crassin/thesis/)), then inside
the fragment shader we shoot rays from the mesh and try to intersect them with the
voxelized version of the scene to compute a Monte Carlo approximation to the ambient
occlusion integral.

Everything runs in software using my own [rendering engine](https://luisclaudio26.github.io/portfolio/realtime/).

[Source code](https://github.com/luisclaudio26/RenderingPipeline)

<img src='/images/vao_sibenik_noao.png' width="350"> <img src='/images/vao_sibenik_ao.png' width="350">

<img src='/images/vao_breakfastroom_noao.png' width="350"> <img src='/images/vao_breakfastroom_ao.png' width="350">

<img src='/images/vao_bedroom_noao.png' width="350"> <img src='/images/vao_bedroom_ao.png' width="350">

_Some [well known scenes](http://casual-effects.com/data/) rendered using local, diffuse
illumination with (left) and without (right) our ambient occlusion effect._
