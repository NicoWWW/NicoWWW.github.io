---
layout: post
title:  "Dandelion Wine"
summary: "Technical Artist"
date:   2024-05-01
preview: /assets/Dandelion_Wine/DW_preview2.jpg
---

![Picture 1](/assets/Dandelion_Wine/DW_preview.png)

*Dandelion Wine* is a Whimsical Slapstick Combat Game for Mobile Audiences, developed in Unity with a 30-person multidisciplinary game team as part of a year-long advanced game project. The game narrative is based on the Roman/Geek mythology, inviting players play as a mischievous glob of wine wreaking havoc at a cult festival, solve puzzles to grow bigger, and build an army of tipsy Winefolk to defeat the ultimate Wine God.

**Platform** : Mobile

**Engine** : Unity

**Year** : 2023-2024

<hr>

## My Focus

* Applied and fine-tuned Zibra Liquids to create liquid simulation as the main player character
* Developed advanced shaders and VFX with HDRP, implementing custom particle systems, environmental lighting and fog effects
* Partnered closely with art and engineering teams to optimize art assets for performace and troubleshoot game texturing and real-time rendering issues
 

### Technical Art Breakdown

For the best performance of the liquid main character, we need to simulate different behaviours a drop of water ("wine" in the game) could have, including liuquid blob streching when picking up collectibles (surface tension), squashing and sketching in the movements, slowing in and out, etc. 

We utilized Zibra Liquids from the Unity Asset Store to create the main water blob effect. Additionally, we employed various Force Fields with differing strengths and directions to simulate tension forces, achieving a realistic squashing and stretching effect. While Zibra Liquid offers inline controls for adjusting viscosity, density, and metalness of the liquid, I further enhanced the visual appeal by incorporating environmental lighting. These lights were strategically placed to reflect off the blob, imparting a glossy texture reminiscent of wine, which enriched and heightened the realism of the expansive background environments.

<div style="text-align: center;">
         <img width="800" src="/assets/Dandelion_Wine/DW_liquid_gif.gif">
</div>

<p style="text-align: center;">
    Liquid Simulation in Development Testing
</p>

<div style="text-align: center;">
         <img width="800" src="/assets/Dandelion_Wine/DW_liquid2_gif.gif">
</div>

<p style="text-align: center;">
    Liquid Simulation in Live Demonstration of <i>Dandelion Wine</i>
</p>

<p style="text-align: center;">
    
</p>

![Picture 4](/assets/Dandelion_Wine/lighting1.png)

![Picture 5](/assets/Dandelion_Wine/lighting2.png)

<p style="text-align: center;">
    Lighting ane environment rendering for the game.
</p>

![Picture 2](/assets/Dandelion_Wine/DW_older2.png)

![Picture 3](/assets/Dandelion_Wine/DW_older3.png)

<p style="text-align: center;">
    A showcase of my lighting work and environment props placement. However, Due to changes in gameplay mechanics and narrative direction later in development, these background setups were ultimately discarded.
</p>
