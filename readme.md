# Welcome to WGPU Tutorial
I am following [sotrh's learn-wgpu tutorial](https://sotrh.github.io/learn-wgpu/).

## Status
I am just about to start: [A controller for our camera](https://sotrh.github.io/learn-wgpu/beginner/tutorial6-uniforms/#a-controller-for-our-camera).

## Dependencies
Dependency | Use
--- | ---
anyhow | Simplifies error handling.

## Glossary
Word | Definition
--- | ---
BindGroup | Describes a set of resources and how they can be accessed by a **shader**.
PipelineLayout | Contains a list of `BindGroupLayout`'s the **pipeline** can use.
Uniform | A blob of data that is available to every invocation of a set of shaders.

## Issues with tutorial
In the [Using the uniform in the vertex shader](https://sotrh.github.io/learn-wgpu/beginner/tutorial6-uniforms/#using-the-uniform-in-the-vertex-shader) code snippet, the line 
```
var<uniform> camera: Camera;
```
should be
```
var<uniform> camera: CameraUniform;
```