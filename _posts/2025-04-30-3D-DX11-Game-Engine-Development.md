---
layout: post
title:  "3D DX11 Game Engine Development"
summary: "ITP485 Individual Project"
date:   2025-04-30 
preview: /assets/others/ITP485PostPreview.png
---

<video controls width="800">
  <source src="/assets/others/ITP485Video.mp4" type="video/mp4">
  <source src="video.webm" type="video/webm">
  This browser does not support HTML video.
</video>

**Development** : C++, DX11

**Year** : 2025

As part of an advanced game engine architecture course, I designed and implemented a custom 3D game engine from the ground up using DirectX 11. This project gave me hands-on experience with low-level graphics APIs, engine subsystems, and optimization techniques commonly used in professional game development.

<hr>

# Rendering and Core Systems

I built a SIMD-optimized math library for efficient vector and matrix calculations, which significantly accelerated linear algebra operations critical for rendering and animation. The engine’s rendering pipeline supports textures, materials, and shaders, with a custom caching system to minimize redundant GPU calls and improve frame stability. I also implemented post-processing effects such as Bloom to enhance visual fidelity.

Throughout development, I relied on graphics debuggers provided by Visual Studio to analyze GPU draw calls, inspect frame buffers, and trace shader behavior. These tools were essential for diagnosing pipeline errors, verifying render passes, and ensuring correctness when optimizing performance.

<hr>

# Rendering & Lighting
Beyond building the base rendering pipeline in DirectX 11, I implemented a lighting system to give scenes more depth and realism.
## Lighting Models
* Implemented multiple per-pixel lighting models in HLSL, including Lambert and Phong shading.
* Added support for normal mapping to simulate fine surface detail under dynamic lighting.
* Extended the system with rim-lighting and half-Lambert shading, which are useful for stylized effects and non-photorealistic rendering.
## Light Sources
* Supported point lights and directional lights, with the ability to handle multiple active lights in a scene.
* Designed a constant buffer layout to pass light parameters (position, color, intensity) efficiently to the GPU.

This work gave the engine the ability to render lit, textured objects with customizable material properties, establishing a strong foundation for future features like shadows, deferred rendering, and PBR workflows.

<hr>

# Animation and Inverse Kinematics

On the animation side, I implemented a complete skinning and blending system to handle skeletal animations and transitions between states. To improve efficiency, I introduced a multithreaded job scheduling system that distributes animation updates across worker threads, reducing CPU bottlenecks during heavy scenes.

I also integrated inverse kinematics (IK) algorithms, which allowed characters’ joints and limbs to adapt dynamically to the environment. For example, feet automatically align to uneven terrain and arms can target specific objects, resulting in more natural and believable poses compared to traditional forward kinematics alone. Debugging IK and skinning required a combination of custom engine debug visualizers and step-by-step inspection in the graphics debugger to track matrix transformations in real time.

<hr>

# Multithreaded Job System
To maximize CPU utilization and reduce frame stalls, I implemented a general-purpose multithreaded job system for the engine. This subsystem distributes work across multiple worker threads and allows heavy tasks to execute in parallel, rather than blocking the main game loop.
## Architecture:
* A Job Manager oversees a global Job Queue, where lightweight tasks (jobs) are submitted
* Multiple worker threads continuously pull jobs from the queue, executing them independently
* The system supports dependencies and synchronization, ensuring that jobs complete in the correct order without race conditions
## Animation Use Case
* Animation: parallelized skinning, blending, and inverse kinematics updates across multiple characters
* Physics: batched AABB collision checks executed as parallel jobs to speed up scene queries
* Resource Management: handled background asset loading and cache updates (textures, shaders, materials) without stalling the render thread

By extending the job system beyond animation, I built a scalable framework that improved the performance of multiple engine subsystems by parallel processing, making the engine more robust and closer in architecture to production-grade game engines.
