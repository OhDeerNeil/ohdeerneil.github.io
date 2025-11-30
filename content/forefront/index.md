+++
date = '2025-11-28T11:08:53+01:00'
draft = false
title = 'Forefront'
tags= ["Games", "C#"]
featured= true
description= "Forefront: a fun chaotic shooter in VR"
cover= "Forefront_KeyArt_3840x2160.png"
weight= 3
+++

### The project:

[Forefront](https://www.youtube.com/watch?v=QQhvyFRlYcs) is a chaotic 32 player shooter, bringing those "only battlefield moments" into VR.
Making players work together in squads to take the objectives, and making sure they use all available gadgets and vehicles to give their team an edge. Created with an in-house varriant of ECS.


**Created with** Unity3D, Blender, Photon Fusion 2

**Developed for** Meta Quest 2/Meta Quest 3, Pico, and Steam VR

### The team:
Created by TriangleFactory, at peak the team was around 35 people.

### My role:
As a programmer, my role existed out of the expected support of main features, to helping out with performance wherever possible, to implementing systems that needed to fit the full picture, with the following being some of the main features I was responsible for:

**Features**
 - Nametag system: allowing players to from a distance get a clear grasp of the other players allegiance.
 - The explosive charge: allowing the throwing of an sticky C4 that could be detonated at the press of a button.

 - LineOfSightObstruction system: making sure that players can't use their gadgets or guns when these are inside of walls.
 - Spotting system: allowing players to showcase the enemy icons by aiming at them through all weapon variants.

 - Voice chat: bringing over the lessons learned from the vivox implementation in [Breachers](/content/breachers/index.md), making it more robuust and preparing it for future projects
- Score system: making sure the players are awarded their points for the in game activities, allowing our progression system to reward them.

 - UI rotation systems: creating different systems that allowed the UI to rotate allong correctly with: body rotation, head rotation or stick rotation 
 - UI Priority system: creating a system that could be easily extended, making sure that different UI groups could be created that would only show the highest priority and hide the others.
 - Vehicle UI: implementing the HUD for every vehicle and making them easy to change for future varriations.
 - Killer highlights: to communicate to the player who or what killed them.
 - Directional hit indicators: in a similar vein. 

 - Adhering to the TRC's for the Quest release.


Some of the notable support I worked on:

**Performance**:

Because of the scale, we always had to keep the following in mind: 
 - Jobifying systems: using unity's solution to multithread where it made sense
 - GBAlloc: making sure all small garbage allocations are followed up on and kept to a minimum.
 - UI optimizations: overdraw, sprite renderers vs canvas cost, etc.


**Bugfixes**
 - Ordered spawning: because of our inability to receive spawning and depsawning packages in the correct order, we ahd to implement a system that would wait for certain packages to be handled before the rest of the game could work with the new info.
 - Memory leaks: following up on memory leaks that snuck through the cracks and squashing them.
 - Suttering Zipline and nametags: for different reasons, but it boiled down to the order of setting, and getting data, and then making sure this still happened correctly while keeping our optimizations intact.

 - Spawn menu generator extension: allowing artists to bake in a water texture into the spawn map.
 - Cleanup of the spawn menu UI




 {{< youtube QQhvyFRlYcs >}}