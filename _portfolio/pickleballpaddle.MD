---
title: "Pickleball paddle"
excerpt: "Designing and making a pickleball paddle"
header:
  image: /assets/img/paddle model.png
  teaser: /assets/img/paddle model.png
gallery:
  - url: /assets/img/paddle hollow.JPEG
    image_path: assets/img/paddle hollow.JPEG
    alt: "phone in!"
  - url: /assets/img/paddle grab.JPEG
    image_path: assets/img/paddle grab.JPEG
    alt: "phone on side"
  - url: /assets/img/paddle fracture.JPEG
    image_path: assets/img/paddle fracture.JPEG
    alt: "closeup of TPU"
---

## Criteria for paddles


1. **Design and 3D print a pickleball paddle** that conforms to the 2024 USA Pickleball Official Rulebook. The paddle must be able to survive a game of pickleball. *(1%)*

   My pickleball paddle conforms to all rules and regulations set by the rulebook.

Unfortunately, my paddle did not survive a full game of pickleball.  This may be in part due to the design of the paddle itself, however there were noticeable printing errors such as under extrusion and it not finishing the last 2-3 top layers.  This could be considered main contributor of the paddle fracturing.

2. The pickleball paddle must have:
   - A **printed TPU element** in the handle to improve grip. *(0.5%)*
   - An **interchangeable edge guard** to protect the face of the paddle when contact is made with the ground. *(0.5%)*

   My paddle has both a TPU handle and a TPU edge guard.  The handle was made in OPENSCAD, with dimensions that perfectly fit my hand’s dimensions.  This was then ported to Fusion where I made cutouts so it could slip on to the paddle.  After using it I noticed that the TPU grip was slippery, so I wrapped it with climbing tape to give myself a better grip.
   <img src="https://github.com/1Mattchu/MatthewDeLuna.github.io/blob/main/assets/img/Screenshot 2024-04-23 203652 (Medium).png?raw=true" alt="paddle edge" width="600">


   The edge guard was printed in 3 straight strips, these strips would bend and snap into the paddle’s edge, locking it in place.  This worked better than expected, and the edge guard never moved after snapping into place.
   <img src="https://github.com/1Mattchu/MatthewDeLuna.github.io/blob/main/assets/img/paddle edge.png?raw=true" alt="paddle edge" width="600">
    *A cross-sectional analysis view of my paddle and edge guard.*

3. **Optimize the weight and mass balance** of the pickleball paddle for your gameplay.
   - **Weight** *(0.5%)*:
     - **Lightweight** (<7.3 oz): increased agility and control
     - **Midweight** (7.3 oz - 8.3 oz): optimized power and control
     - **Heavy** (>8.3 oz): maximum power

     My goal for this paddle was to minimize weight as much as possible. After testing wind drag with a similarly sized cardboard cutout, I knew I had to make it as lightweight as possible if I wanted it to remain nimble.  My paddle is only 6 mm thick, with 20% infill.  The sidewalls were printed at 2.4 mm and the top/bottom was printed at .72 mm (The top was less due to printing issues).  These settings worked great to help reduce the total weight of the paddle to something reasonable.  Unfortunately, I don’t have a scale to weigh it, and I do not trust Fusion 360’s weight as it does not properly account for hollowness.  I did compare its weight to a regular pickleball paddle however and it was a very similar weight, albeit slightly heavier.  Overall I’m almost positive that it is in the Midweight to Heavy category, which was expected given the sheer size of it.

   - **Mass balance** *(0.5%)*: [See this article for more details.](https://www.thedinkpickleball.com/paddle-swingweight-performance/)

     I was not sure where I would personally prefer the weight distribution to be so I decided to have this design center balanced and/or slightly head heavy.  In the end, after some tweaking I was able to get the center of gravity ~10mm from the center of the paddle.  I would consider this a very center balanced weight, as its center of gravity is only 2.2% away from its true center.  I noticed that the article mentioned 1/8 inch deviations for “heavyness” points, however due to my paddles longer length and non traditional design, I’m using % deviations.
     <img src="https://github.com/1Mattchu/MatthewDeLuna.github.io/blob/main/assets/img/paddle gravity.png?raw=true" alt="slicer settings" width="600">
*Red is the True middle of the pickleball paddle, green is its center of mass.  Their distance between one another is ~10mm.*

     (Center of gravity distance from true middle / paddle length)*100% 

     (10 mm/457 mm) *100% = 2.2%



#### View my design!
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e6b828f81181514a0?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>
{% include gallery caption="Images!" %}
