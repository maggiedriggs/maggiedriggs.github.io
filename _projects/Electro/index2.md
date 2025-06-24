---
layout: post
title: Electromechanical Design
description:  
    Documentation of the projects from my junior design class! The projects highlighted are a Yahtzee shaker, a SolidWorks dyanmic car model, and then that car built out and tested for a class competition. Each blog post highlights the steps to create each item.
skills: 
  - CAD
  - Arduino
  - C
  - Prototyping / 3D Printing

main-image: /project2.jpg
---

---
# Multi-body Dynamic Model
The assigned task was to build and assemble a vehicle that could transport a 1ft aluminum bar 5 feet with maximum acceleration and deceleration without tipping over. The finished Solidworks Simulation is shown below, with the car taking 5.04 seconds to cover 5 feet, with an acceleration of 2.667 ft/s^2. 

The graphs below depict the reaction force vs the acceleration of the car. The reaction force was taken as the force on the mate of the bar's front point with the car's plane. The acceleration is increasing at a constant rate. The point at which the reaction force is zero was taken to be the maximum acceleration, because if the reaction force is zero then that is the exact moment the bar will tip over. The maximum acceleration was taken to be 812.594mm/s^2 or 2.667 ft/s^2. 

This maximum acceleration was then used to find the minimum time that the car could traverse 5 feet (1524mm). It was found if the bar accelerated for 2 seconds at 812.594mm/s^2 and then decelerated for the same amount of time that it could cover 5 feet in 5.04 seconds.

The results are reasonable because in the simulation friction between components, drag, and tolerances are not taken into account, therefore the simulation gives an optimized fast time of 5 seconds. The bar is a foot tall and to go faster than 5 seconds does not logically make sense because the car is small and there will be a moment on the bar as the car moves forward. In reality, it might take more time, maybe 7-9 seconds for the car to travel this distance when taking into consideration all the factors that will put the bar off balance. But 5 seconds with the mentioned assumptions could be plausible as an optimized time

## Header 2  
Use this for the header of each section
### Results
Hello here are results
