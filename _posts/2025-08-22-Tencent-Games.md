---
layout: post
title:  "SWE Intern at Tecent Games(LightSpeed Studio)"
date:   2025-08-22
preview: /assets/LightSpeed_Logo.jpeg
---

**Development** : C++, Lua, Unreal, Git

**Year** : 2025 Summer

## NPC Interaction System

I developed a comprehensive NPC interaction system that integrated the game client with both an AI Chat server and an AI GOAP decision-making server. This allowed players to engage with NPCs through real-time text and voice dialogue, creating more natural and immersive gameplay experiences. To achieve this, I built the entire NPC interaction UI, which supported player input, NPC responses, and stateful conversations that reflected both context and game progression.

On the technical side, I focused heavily on client–server communication. I optimized the data exchange pipeline to reduce latency and prevent message delays, while also resolving several server desynchronization bugs that could disrupt gameplay. I extended the NLP parameter parsing system, enabling the game to automatically recognize and interpret player instructions, convert them into structured data, and forward them to the AI server for execution. This allowed NPCs to dynamically update their behaviors and responses based on player intent, creating a seamless and engaging interaction loop.


## NPC Behavior and State Management

Beyond dialogue, I implemented the core behavior and state logic for NPCs. Their actions — such as recruitment, following the player, engaging in combat, resting, and interacting with the environment — were all driven by decisions from the AI GOAP server. On the client side, I ensured smooth state transitions by maintaining communication channels with the server and synchronizing behavior updates in real time.

As an extension of this system, I designed and implemented a pet NPC subsystem, where players could interact with companion-like NPCs. Features included petting, following, and sitting behaviors, which deepened the emotional connection between the player and their in-game companions. This subsystem also laid the groundwork for future expansions using AI-generated animal models.


## Performance Profiling and Optimization

To maintain a smooth player experience, I proactively conducted performance profiling using Unreal Insights. I identified and analyzed 10+ frame-rate bottlenecks, ranging from inefficient animation updates to redundant communication calls. Working closely with senior engineers, I proposed and implemented fixes that improved frame stability and overall responsiveness of the system. These optimizations ensured that the AI-driven NPC interactions ran reliably without compromising the gameplay experience.
