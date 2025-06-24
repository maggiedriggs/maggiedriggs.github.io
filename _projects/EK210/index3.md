---
layout: post
title: EK 210 - Desk Lamp
description:  A group of four and I was tasked to produce desk lamp for people with limited motor skills and light sensitivity to meet their needs. When browsing different stores like Home Depot, Amazon, or Target, the most common desk lamp is one with a standard light setting and an on/off switch. Users with limited fine motor skills may struggle to operate these types of controls, and the client prefers blue light to be emitted in the morning, and red light in the evening.
skills: 
- Circuitry
- Laser Cutting
- CNC Milling
- Soldering
- Arduino & Interfacing
main-image: /Screenshot 2025-06-23 at 9.44.50 PM.png
---

---
# Steps of Project
Used for the title (already generated automatically at the top)
## Planning
We first listed all of our objectives and constraints and made a project priority matrix. From there, we decided "be safe, illuminate desk, accessible for gross motor functions, and caters to light sensitivity" we our four most important objectives.
Then, we made a morph chart to gather ideas for the means to our objectives. The goal is to lay everything out on the table with no judgments.
{% include image-gallery.html images="210Planningchart.png" height="400" %}   
## Bill of Materials
Once we had ideas for how we wanted to achieve our objectives, we had to order parts and make a Bill of Materials. There are so many options for each element, and we had to consider how each part would connect and how much current the system would draw. We decided on a gooseneck bad, a resistor pad sensor, an RTC to tell time, and a RGBW LED strip.
{% include image-gallery.html images="210Budget.png" height="400" %}   
## Power Budget & Circuitry
The RGBW LED strip requires 12V and 3.3W, so we decided on a 10W power supply to power the LED strip and all other elements. We wanted to ensure that we had at least double the amount of current that we would actually need, as to not blow anything up. The power budget was essential because it made us know exactly what each element was drawing from the power source.  
The picture showcases the circuit we made, with the mosfets controlling the LED strip, and taking in commands from the Arduino.
{% include image-gallery.html images="210Circuitry.png" height="400" %}   
## Housing
We decided on a gooseneck arm so that the lamp is easily adjustable. Some problems aroused once we got all of our parts. The gooseneck had a weird thread size and was too large for the taps we had in the school's machine shop, and we didn't know how we would connect the gooseneck to the lamp shade.  
So, the first thing I did was go to the machine shop and tap a new hole in the center of the gooseneck and use sheet metal to create a hinge between the gooseneck and shade.
{% include image-gallery.html images="210Planningchart.png" height="400" %}   
## CNC Milled Base
Next, I made a base on Solidworks and then used Gibbscan to create the tool path for the CNC to mill. I used HDPE as it was cheap and easy to mill, and the base had a lot of surface area so that the lamp is more stable.
{% include image-gallery.html images="210CNC Base.HEIC" height="400" %}   
## Laser Cut Walls and Lid
I made a DMF file on Solidworks of the walls and lid for the base. I engraved the group's names and an intuitive instruction of where to press on the box and accounted for all the holes. I used CorelDraw and cut the pieces out.
{% include image-gallery.html images="210Base.png" height="400" %}   
## 3D Printed Hinges
I used PLA on a Makergear to print out some hinges, as ordering them would not be quick enough. The hinges ended up being crunchy, so I would change the settings on them if I revised this lamp.
{% include image-gallery.html images="210Hinge.HEIC" height="400" %}   
## Redo Shade and Gooseneck Connection
The sheet metal snapped, so I needed to make a more sturdy connection. I got a 30 60 90 triangle, and milled and tapped a hole in it to fit the gooseneck, and then milled out any metal that would get in the way of the socket part of the screw. Then, I redid the sheet metal bend on top of the triangle so it had extra stability. Then I put back in the pop rivets and called that part good!
{% include image-gallery.html images="210Connection.png" height="400" %}   
## Testing
To ensure that our product was working as we planned it to, we ran tests on the intensity of the light and the color temperature. We found that the lux decreases as distance increases, but that at 30 inches away the light is still sufficient to read. Our objective to light a 60 by 30 inch desk is within this scope.
{% include image-gallery.html images="210Intensity.png" height="400" %}   
## Color Temperature
We programmed the arduino to change which color of LEDs are on throughout the day, and used photography software to measure the color temperature emitted. We found that in the morning, our lamp does radiate blue light, and at night it changes to warm light.
{% include image-gallery.html images="210Planningchart.png" height="400" %}   
## Conclusions
We then presented our lamp to the professors and to the client, and got to keep our lamp! It was fun to go through all the steps of a prompt to a full functioning product!
{% include image-gallery.html images="210Planning.png" height="400" %}   
## Embedding images 
### External images
{% include image-gallery.html images="https://live.staticflickr.com/65535/52821641477_d397e56bc4_k.jpg, https://live.staticflickr.com/65535/52822650673_f074b20d90_k.jpg" height="400"%}
<span style="font-size: 10px">"Starship Test Flight Mission" from https://www.flickr.com/photos/spacex/52821641477/</span>  
You can put in multiple entries. All images will be at a fixed height in the same row. With smaller window, they will switch to columns.  

### Embeed images
{% include image-gallery.html images="project2.jpg" height="400" %} 
place the images in project folder/images then update the file path.   
