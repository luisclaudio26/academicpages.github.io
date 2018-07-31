---
title: "Voxel ambient occlusion"
excerpt: "Raytraced ambient occlusion using voxels<br/><img src='/images/vao.png'>"
collection: portfolio
---

This was my final project for the Computer Graphics course as an MSc. student at UFRGS.
The goal was to compute a voxel representation of the scene (inspired by the work of
[Crassin et al](http://maverick.inria.fr/Membres/Cyril.Crassin/thesis/)), then inside
the fragment shader we shoot rays from the mesh and try to intersect them with the voxelized
version of the scene to estimate the ambient occlusion of the given fragment. Everything
was done in software using my own [rendering engine](https://luisclaudio26.github.io/portfolio/realtime/).

[Source code](https://github.com/luisclaudio26/RenderingPipeline)

<img src='/images/vao_sibenik_noao.png'> <img src='/images/vao_sibenik_ao.png'>

<img src='/images/vao_breakfastroom.png'>

<img src='/images/vao_bedroom.png'>
