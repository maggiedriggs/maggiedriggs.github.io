---
layout: post
title: Yahtzee Cartesian Motion System
description:  
    The assignment was to make a 2.5 degrees of freedom system to perform a task of choice. In a team of 4, it was decided to create Yahtzee, where the dice are picked up and vibrated to simulate rolling dice. 
skills: 
  - Interfacing MKS Base Board
  - 3D Printing
  - Milling
  - Laser Cutting
  - G-code
  - Stepper Motors
  - Belts & Pulleys
  - Sheet Metal Bending

main-image: /Pin.png
---

---
## Video

Before the details of the whole project, the final product is shown below in a video!
{% include youtube-video.html id="yCkTwwxNkDw" autoplay= "true"%}

## Ideas
First, ideas had to be hashed out to find an efficient way to maneuver the dice and how to roll the dice. The idea to use a pie-server type of handle to pick up the dice, which scapes along the floor of the project and scoops up the dice, hitting a metal piece that is the same shape as the end of the pie-server piece was decided upon. The picture below depicts the first sketch of the product.

{% include image-gallery.html images="1sketch.png" height="400" %} 

## Pulley System
The next step after this was to get one degree of freedom working with a stepper motor and pulley system. The servo needed to be held in place with a 3D printed holder and the other end to hold the pulley. A carriage in the middle would move with the pulley to be connected to another side. The dimensions of the rod and servo were taken so that a 3D printed element could fit them accurately. Below are the drawings of some dimensions. 
{% include image-gallery.html images="2Drawing.png" height="400" %} 
The first draft of one arm of the components is shown below
{% include image-gallery.html images="3Prototypes.png" height="400" %} 
For the first degree of freedom, the 3D printed red stepper motor was not thick enough, so a new one was prototyped (bottom right picture). The white pulley on the other side matched the height of the stepper motor, and fit well. The carriage required more prototyping, as the grooves on the belt were difficult to get a snug fit on and finding the right proportions to let the pulley slide through easily. Below are some of the carriage renditions. The grooves of the parts needed to be exact and any support included in the printed parts would be hard to remove, so instead of PLA, SLA printers were utilized with dissolvable supports.
{% include image-gallery.html images="4Other.png" height="400" %} 
## Fixing Problems
Once one side of the project was fine-tuned correctly, another set was printed for the other side of the project and the team met to discuss next steps and delegate tasks. The notes from the meeting are shown below. The scooper was decided to be made out of sheet metal as it would absorb the vibrations well and is easy to bend into the desired shape. The walls were also decided to be sheet metal, and the base was made out of acrylic. 
{% include image-gallery.html images="5Todo.png" height="400" %}
The base was laser-cut to fit the length of the scooper and the desired width of the assembly. L-brackets were bent and drilled and tapped into the metal bars on the side to attach to the platform. It was important that 
a) the ground was level
b) the two metal bars were in parallel so that the carriages moved smoothly without an angle 
To ensure this happened, calipers, vices, and levelers were utilized.
Below are the L-brackets and the floor aligned correctly.
{% include image-gallery.html images="6idk.png" height="400" %} 
Next, the pie-server scooper was made using a shear, cornering tool, and bending tools. The aluminum is flexible, which is ideal for vibrations. A 3D-printed holder for the servo vibration was printed, but later deemed unnecessary as it absorbed vibration from the servo. The vibration of the servo was made by using glue and a bolt that was off-centered, creating a moment arm (we initially cut out a 1" cylinder of aluminum to attach to the servo but were thankfully told that that much weight at the end of the servo would be massive before we tested it out).
{% include image-gallery.html images="7scooper.png" height="400" %} 
## Putting Everything Together
Next, the middle bar is screwed in with a study L-joint and the walls for the scooper are bent out as well. Soon after, it was decided that the sheet metal for the walls was too sharp, and that construction paper would do the job just as well, while safer. The corner part was kept as sheet metal as it was necessary to have a stiff edge for the scooper to hit. 
In testing the rolling of the dice, the dice tended to roll all over the floor due to their chaotic nature. To solve this problem, a 3D-printed funnel was created at the top of the corner metal part to guide the dice to drop only near the front of the project. The scooper will move over to the top of the funnel, and vibrate to knock off the dice.
The edge of the aluminum was also found to be too blunt of an edge, so construction paper was taped to the edge to smooth the transition.
{% include image-gallery.html images="8wholething.png" height="400" %} 
Lastly, the servo was moved to the back of the scooper so that the dice didn't hit it, and then all that was left was testing and coding the project. Repeteir Host was utilized to give G-code commands to the stepper motors and servo via a MKS Base v1.6 board. 
Once the project was working, it was presented to the professor and class and explained what the purpose was of the project. The project worked reliably and was used mostly with scrap sheet metal/rods and with 3D printed elements. 
If the project were to be repeated, the funnel and corner piece could have been fit more exactly to the scooper, which would improve the reliability of the project. 
Overall, it was a fun project that works and can simulate rolling dice! If you use it enough you might get a Yahtzee.
{% include image-gallery.html images="9meandroberto.png" height="400" %} 
