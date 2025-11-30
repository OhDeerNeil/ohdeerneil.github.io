+++
date = '2025-11-28T11:08:53+01:00'
draft = true
title = 'Forefront'
tags= ["Games", "C#"]
featured= true
description= "Forefront: a fun chaotic shooter in VR"
cover= "Forefront_KeyArt_3840x2160.png"
weight= 3
+++

### The project:

[Forefront](https://www.youtube.com/watch?v=QQhvyFRlYcs) is a chaotic 32 player shooter, bringing those "only battlefield moments" into VR.
Making players work together in squads to take the objectives, and making sure they use all available gadgets and vehicles to give their team an edge.


**Created with** Unity3D, Blender, Photon Fusion 2

**Developed for** Meta Quest 2/Meta Quest 3, Pico, and Steam VR

### The team:
Created by TriangleFactory, at peak the team was around 35 people.

### My role:
As a programmer, my role existed out of the expected support of main features, to helping out with performance wherever possible, to implementing systems that needed to fit the full picture, with the following being some of the main features I was responsible for:
**Features**
 - Nametag system: allowing players to from a distance get a clear grasp of the other players allegiance.
 - The explosive charge: allowing the throwing of an sticky C4 that could be detonated at the press of a button.

 - LineOfSightObstruction system
 - spotting system
 - Voice chat: bringing over the lessons learned from the vivox implementation in [Breachers](/content/breachers/index.md), making it more robuust and preparing it for future projects
- score system

 - UI rotation systems: creating different systems that allowed the UI to rotate allong correctly with: body rotation, head rotation or stick rotation 
 - UI Priority system: creating a system that could be easily extended, making sure that different UI groups could be created that would only show the highest priority and hide the others.


 - Vehicle UI: implementing the HUD for every vehicle and making them easy to change for future varriations.
 - Killer highlights 
 - improved hit indicators

  - TRC's for the Quest release


Some of the notable support I worked on:

**Bugfixes**
 - hand pose tool
 - ordered spawning
 - memory leaks
 - animation issues
 - zipline camera stutter issue
 - spawn menu generator extension
 - cleanup of the spawn menu UI
 - nametag stutter


**Performance**:
 - jobifying
 - GBAlloc in different system
 - UI optimizations: overdraw, sprite renderers vs canvas

 {{< youtube QQhvyFRlYcs >}}