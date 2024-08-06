---
layout: post
title:  "Dandelion Wine"
summary: "Technical Artist"
date:   2023-09-07
preview: /assets/postpreview.png
---

![Picture 1](/assets/Dandelion_Wine/DW_front_pic.png)

*Dandelion Wine* is a **Whimsical Slapstick Combat Game** for **Mobile Audiences**, developed in Unity with a 30-person multidisciplinary game team as part of a year-long advanced game project. The game narrative is based on the Roman/Geek mythology, inviting players play as a mischievous glob of wine wreaking havoc at a cult festival, solve puzzles to grow bigger, and build an army of tipsy Winefolk to defeat the ultimate Wine God.

## My Focus

* Applied and fine-tuned Zibra Liquids to create liquid simulation as the main player character
* Created realistic environments and implemented dynamic lighting with fog effects to enhance game realism
* Partnered closely with art and engineering teams to optimize art assets for performace and troubleshoot game texturing and real-time rendering issues


### Technical Art Breakdown

For the best performance of the liquid main character, we need to simulate different behaviours a drop of water ("wine" in the game) could have, including liuquid blob streching when picking up collectibles (surface tension), squashing and sketching in the movements, slowing in and out, etc. 

We utilized Zibra Liquids from the Unity Asset Store to create the main water blob effect. Additionally, we employed various Force Fields with differing strengths and directions to simulate tension forces, achieving a realistic squashing and stretching effect. While Zibra Liquid offers inline controls for adjusting viscosity, density, and metalness of the liquid, I further enhanced the visual appeal by incorporating environmental lighting. These lights were strategically placed to reflect off the blob, imparting a glossy texture reminiscent of wine, which enriched and heightened the realism of the expansive background environments.

![gif 1](/assets/Dandelion_Wine/DW_liquid_gif.gif){:style="display:block; margin-left:auto; margin-right:auto"; alt = "Liquid Simulation in Development Testing"}

Liquid Simulation in Development Testing

![Video 2](/assets/Dandelion_Wine/DW_liquid2.mov)

Liquid Simulation in Live Demonstration of *Dandelion Wine*

![Picture 2](/assets/Dandelion_Wine/DW_older2.png)

![Picture 3](/assets/Dandelion_Wine/DW_older3.png)
A showcase of my lighting work and environment props placement. However, Due to changes in gameplay mechanics and narrative direction later in development, these background setups were ultimately discarded.