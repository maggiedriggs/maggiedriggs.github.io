---
layout: post
title: Electromechanical Design
description:  
    The assigned task was to build and assemble a vehicle that could transport a 1ft aluminum bar 5 feet the fastest. First, testing done in Solidworks, and then building and competing with that model.
skills: 
  - CAD
  - Arduino
  - C
  - Prototyping / 3D Printing

main-image: /car.png
---

---
# Multi-body Dynamic Model

## Embedding youtube video
{% include youtube-video.html id="LWTgxja2jng" autoplay= "true"%}


The assigned task was to build and assemble a vehicle that could transport a 1ft aluminum bar 5 feet with maximum acceleration and deceleration without tipping over. The finished Solidworks Simulation is shown below, with the car taking 5.04 seconds to cover 5 feet, with an acceleration of 2.667 ft/s^2. 

The graphs below depict the reaction force vs the acceleration of the car. The reaction force was taken as the force on the mate of the bar's front point with the car's plane. The acceleration is increasing at a constant rate. The point at which the reaction force is zero was taken to be the maximum acceleration, because if the reaction force is zero then that is the exact moment the bar will tip over. The maximum acceleration was taken to be 812.594mm/s^2 or 2.667 ft/s^2. 

{% include image-gallery.html images="Reaction Force.png" height="400" %} 

This maximum acceleration was then used to find the minimum time that the car could traverse 5 feet (1524mm). It was found if the bar accelerated for 2 seconds at 812.594mm/s^2 and then decelerated for the same amount of time that it could cover 5 feet in 5.04 seconds.

{% include image-gallery.html images="Accel.png" height="400" %} 

The results are reasonable because in the simulation friction between components, drag, and tolerances are not taken into account, therefore the simulation gives an optimized fast time of 5 seconds. The bar is a foot tall and to go faster than 5 seconds does not logically make sense because the car is small and there will be a moment on the bar as the car moves forward. In reality, it might take more time, maybe 7-9 seconds for the car to travel this distance when taking into consideration all the factors that will put the bar off balance. But 5 seconds with the mentioned assumptions could be plausible as an optimized time

# Class Competition -> Built Car 
Using the maximum acceleration found in the Multi Body Dynamic Model, we built and programmed a car that would accelerate 5 feet forward, and then reverse without knocking a 1 ft bar off of it. 
{% include youtube-video.html id="2qUsUAp-97U" autoplay= "false"%}
The car was made with a motor with a Lego gear that drives the axle of the front wheels of the car. Code was written and uploaded to an Arduino, and the wheels were 3D printed with the tire printed with TPU so that they were flexible, and the inner axle of the wheel was printed in PLA. The car's base was laser cut with the needed holes, and the motor holder was 3D printed. 
{% include image-gallery.html images="Gear360.png" height="400" %} 

The calculated acceleration was implemented into the Arduino code by using the analogWrite command to increase the rpm in a for loop at the desired rate. The Arduino code is shown in the last picture. 

## Results
In total it took the car about 9 seconds to go 5 feet, and then go back the other direction. This was larger than the estimated amount be 5 seconds.
{% include image-gallery.html images="Code360.png" height="400" %} 
