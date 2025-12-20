---
date: "2025-11-28T11:08:53+01:00"
draft: false
Title: "Forefront"
tags: ["Games", "Unity", "Triangle Factory"]
featured: true
timeline: true
description: "Massive 32-player battles with semi-destructive environment all on standalone VR"
jobdescription: "As a programmer, I implemented core-systems, making sure performance was respected, and helped up-keeping the technical health of the project."
cover: "Forefront_KeyArt_3840x2160.png"
weight: 3
---

### The project:

[Forefront](https://www.youtube.com/watch?v=QQhvyFRlYcs) is a chaotic 32-player shooter, bringing those "only in Battlefield moments" into VR.
Making players work together in squads to take the objectives, and making sure they use all available gadgets and vehicles to give their team an edge. Created with an in-house variant of ECS.


**Created with** Unity3D, Photon Fusion 2, Vivox

**Developed for** Meta Quest 2/Meta Quest 3, Pico, and Steam VR


### My role:
As a programmer, my role consisted of implementing systems fitting the full picture of the project, with the following listing being some of the main features I was responsible for or co-responsible for, making sure performance was respected wherever possible, and bugfixing and upkeeping the technical health of the project.


**Features**
 - Nametag system: allowing players to get a clear grasp of the other players' allegiance from a distance.
 - The explosive charge: allowing the throwing of a sticky C4 that could be detonated at the press of a button.

 - Line of Sight Obstruction system: making sure that players can't use their gadgets or guns when these are inside walls.
 - Spotting system: allowing players to showcase the enemy icons by aiming at them through all weapon variants.

 - Voice chat: bringing over the lessons learned from the Vivox implementation in [Breachers](/content/breachers/index.md), making it more robust and preparing it for future projects.
- Score system: making sure the players are awarded their points for the in-game activities, allowing our progression system to reward them.

 - UI rotation systems: creating different systems that allowed the UI to correctly rotate along with body rotation, head rotation, or stick rotation.
 - UI Priority system: creating an easily extendable system that would show the highest priority UI of different UI groups.
 - Vehicle UI: implementing the HUD for every vehicle and making it easy to change for future variations.
 - Killer highlights: to communicate to the player who or what killed them.
 - Directional hit indicators: in a similar vein as the Killer highlights, helping player feedback. 

 - Adhering to the [TRC's](https://developers.meta.com/horizon/resources/publish-quest-req) for the Quest release.


#### Some of the notable support I worked on:

**Performance**:

Because of the scale, we always had to keep the following in mind: 
 - Job systems: using Unity's solution to multithread where it made sense.
 - GBAlloc: making sure all small garbage allocations are followed up on and kept to a minimum.
 - UI optimizations: overdraw, sprite renderers vs canvas cost, etc.
 - Keeping network traffic to a minimum.


**Bugfixes**
 - Ordered spawning: because of our inability to receive spawning and depspawning packages in the correct order, we had to implement a system that would wait for certain packages to be handled before the rest of the game could work with the new info.
 - Memory leaks: following up on memory leaks that snuck through the cracks and squashing them.
 - Suttering Zipline and nametags: for various reasons, but it boiled down to the order of setting, getting data, and then making sure this still happened correctly while keeping our optimizations intact.

 - Spawn menu generator extension: allowing artists to easily implement a water texture into the spawn map.
 - Cleanup of the spawn menu UI


 {{< youtube id=QQhvyFRlYcs class=youtube-link >}}