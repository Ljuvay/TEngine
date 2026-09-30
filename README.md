# TEngine

A custom game engine built from scratch in C++ and OpenGL to explore real-time rendering, engine architecture, and graphics programming.

Built by [Dylan Kauffman](https://github.com/Ljuvay), Clemson University CS '27.

## Last Updated

**August 2026**

### Recent Changes

- Implemented basic shadow mapping (refinement in progress)
- Reworked Resource Manager into a modular system
- Added structured Forward Rendering pipeline
- Implemented Blinn-Phong lighting (up to 8 dynamic lights)
- Added ImGui integration for runtime debugging and scene controls
- Improved renderer abstraction and render queue organization
- Added Texture system with multi-texture support
- Implemented height-based terrain texture blending (sand, grass, rock, snow)
- Added debug renderer abstraction for debug grid

<img width="1918" height="1123" alt="TEngine rendering terrain with height-based texture blending" src="https://github.com/user-attachments/assets/7d1342a5-256a-45ba-a4a4-4eda66bce2a4" />

## Features

- Forward Rendering Pipeline
- Scene Management System
- Resource Management System
- Render Queue Architecture
- Object instantiation
- CPU/GPU Mesh Separation
- ImGui Debug Tools
- Blinn-Phong Lighting (up to 8 dynamic lights)
- Shadow Mapping (basic implementation, being refined)
- Chunk-Based Terrain Generation
- Input Abstraction
- Texture System (multi-texture, height-based blending)
- Height-Based Terrain Texture Blending
- Debug Renderer

## Engine Architecture

The current rendering pipeline follows a forward rendering approach.

Scene objects are submitted to a render queue before being processed by the renderer, and meshes are split into CPU and GPU representations.

Current goals:

- Clear separation of engine systems
- Maintainable resource ownership
- Extensible rendering pipeline
- Easy graphics experimentation

## Known Issues

- Shadow mapping is functional but has artifacts. The current light structure and shader setup limit its quality, and I plan to rework them as part of the lighting refactor.

## How I'm Learning

I started with learnopengl.com and now work through *Real-Time Rendering* by Akenine-Möller, Haines, and Hoffman, building a mental roadmap of topics and implementing them in the engine as I need them. I also learn from articles and videos that break down specific effects, and from discussions with other developers in the Graphics Programming Discord.

## Goals

`[-]` = In Progress | `[x]` = Done | `[ ]` = Planned

- [x] Scene Management
- [x] Debug Grid
- [x] Basic Heightmap Terrain
- [x] Basic Blinn-Phong Lighting
- [x] Texture System
- [x] Height-Based Terrain Texturing
- [-] Shadow Mapping (working, needs refinement)
- [ ] Material System
- [ ] Frustum Culling
- [ ] Terrain LOD
- [ ] Deferred Rendering
- [ ] Vulkan Renderer
- [ ] more to come...

## Major Refactors

`[-]` = In Progress | `[x]` = Done | `[ ]` = Planned

- [x] MR-01 - Basic Cleanup from class projects, ~~basic scene abstraction~~
- [x] MR-02 - Proper Input handler cleanup
- [x] MR-03 - Renderer abstraction and renderObjects
- [x] MR-04 - Re-do Resource Managers for cleanliness
- [x] MR-05 - ImGui Integration
- [-] MR-06 - Engine Cleanup and Editor Tooling
- [ ] MR-07 - Safety Checks and exception handling
- [ ] more to come...

## Long-Term Vision

TEngine is the foundation for a game I hope to build eventually, working title **Turbulent**. It's a long-term idea inspired by games I played through high school and college, like Rust and Escape From Tarkov. I love them, but they demand a lot of time, so I'd like to make something in that spirit that fits busier schedules. For now, the focus is on the engine itself and learning graphics programming.

## Built With

- C++
- OpenGL
- GLFW
- GLM
- GLAD
- CMake

## Find Me

[YouTube - Dev Logs & Demos](https://www.youtube.com/@Luvayy)

---

*"When every action has a purpose, every action has a result" - Gregg Plitt*
