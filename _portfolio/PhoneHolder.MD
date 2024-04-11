---
title: "Bike Phone holder"
excerpt: "Designing a functional phone holder for my bike"
header:
  image: /assets/img/IMG_1263.jpg
  teaser: /assets/img/IMG_1263.jpg
gallery:
  - url: /assets/img/PliersCompare.jpeg
    image_path: assets/img/PliersCompare.jpeg
    alt: "comparison"
  - url: /assets/img/PliersDisect.jpeg
    image_path: assets/img/PliersDisect.jpeg
    alt: "dissection"
  - url: /assets/img/IMG_1256.gif
    image_path: assets/img/IMG_1256.gif
    alt: "working"
---

A description of top-down modeling and how it was leveraged in this
assignment.
▪ Rationale behind your design
▪ Assembly instructions
▪ Material choice

### Top-Down Modeling

Top-down modeling is an approach in design where you start with the overall concept or higher-level features of a product and then gradually refine the details. It's like building a house from the roof down. In Fusion 360, this means creating the main structure or assembly first, then adding individual components and refining them as needed. This method allows for better control over the design process and ensures that all parts of the product work together seamlessly.

**My design is composed of 3 main parts:**

1. **The Clamp:** Attaches to the bike handle.
2. **The Rotating Joint:** Controls the angle of the phone.
3. **The Holder:** Uses a threaded rod and clamps to screw together and hold the phone in place.

#### To Assemble:

Follow the image provided. You will need:

- 3 M5 heatset inserts
- 6 M5x10 screws
- 1 M5x25 screw
- 4 M5 nuts

You will need to place 2 heatset inserts in the rotating ball connecting to the threaded rod, and one at the bottom of the post, connecting it to the top handle clamp.

*This design is made of both PLA and TPU.* The TPU was specifically chosen to help grip onto the handlebars. PLA is typically not the best choice for a functional product such as this phone holder. However, I am lazy and it works well enough. I also like to baby my stuff, so there should never be a situation where my bike gets left in an environment hot enough to melt PLA.

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Print-in-place mechanisms are one of the special things about FFF printing that nearly all other manufacturing methods fail to produce. Incorporating moving hinges, joints, and linkages in a single print opens the doors to a plethora of new design options. Add in the ability to do multi-material prints, and the options open even further. Print-in-place designs are commonly seen in general hobbyist designs, where the aim is to eliminate the assembly process. This can be especially helpful in batch printing or high volume printing, where assembly times can quickly add up. Print-in-place designs can also be handy as they allow prints to be unfurled to lengths longer than the build plate.

When designing and making multi-material print-in-place devices, materials matter. PLA is a great all-around plastic to use, as its warpage is very low, keeping accurate tolerances and great overhangs. ASA is another good option if you need a stronger part, but its increased warpage can cause separate components to stick to each other. ABS is similar to ASA but with an even worse warpage. TPU is a great secondary filament to use for multi-material printing, adding flexible parts to the design, whether for function or comfort. However, it tends to struggle when adhering to PLA, and for that reason, it's recommended to add dog bones or other intermediate patterns to help prevent the TPU from detaching from the PLA. TPU does not have this issue with ABS or ASA, as it bonds very well.

## Design and Iterative Process

When coming up with ideas for my pliers, I knew I wanted to design something that was a challenge and that I would realistically use in a given environment. Parallel pliers immediately piqued my interest as they had multiple moving parts, and they were completely unique to anything I had seen before.

While drawing up the design on paper, I was worried that it was going to be a challenge to print. The overhangs on the print spanned centimeters, and any bridge failure would result in the pliers not functioning. So with that in mind, my first design was a proof of concept, just to see if I could get it to print. This first design worked great; it had limited motion (multiple known design mistakes) but the overhangs printed perfectly.

With that in mind, I began to work on my second iteration, this one hopefully being the final design. These pliers were going to be fully parametric, allowing the user to change things such as jaw length and tolerance. Keeping all parts of the design parameterized without adding unnecessary parameters became a challenge, and having to calculate the pliers' range of motion based on these parameters became harder and harder as the design process went on. 

One of the most time-consuming dimensions I had to come up with was 
<tt>2 * (asin((Jaw_Width / 2) / (sqrt(2) * (0.5 * (Jaw_open_width + Jaw_Width)))))</tt> 
This calculation defines the arc traced by the left jaw as it closes, in respect to the left handle. I also made a base physics model in Fusion, to test and verify that the movement and dimensions would work in real life.

Finally, when it came to adding the springy part of the design, I went through a few design choices, most of which didn't stick. I did find inspiration from [Nguyen Duc Thang’s](https://www.youtube.com/user/thang010146/about) work on mechanical mechanisms, The one in particular I referenced was from his tensioned pliers: adding tension springs to connect the ends of the jaws to the handles. This ended up working in a very interesting way. At first, it functioned very poorly, with the TPU permanently stretching out after a few uses and the pliers failing to open up any reasonable amount due to their own resistance to opening. However, after repeatedly opening and closing the pliers, the resistance to open them was significantly reduced, allowing the TPU to open the jaws a far greater amount.

Prepping the files for printing was another challenge; the large overhangs meant that many settings were tuned inside the slicer for the printers. Cura has some amazing overhang experimental settings, but unfortunately, I had to fumble around in Super Slicer to get things the way I wanted them.
The Settings "Extra perimeters On overhangs" as well as "Extrusion direction Reverse on odd" made measurable improvements in overhang quality.
<img src="https://github.com/1Mattchu/MatthewDeLuna.github.io/blob/main/assets/img/SlicerSettings.png?raw=true" alt="slicer settings" width="600">


### View The Design!
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6efbce02b5a7c83498?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

### Relevant Specifications of the Pliers

- Useable Jaw length: 30 mm
- Max jaw opening: 17 mm
- Max overall length: 165 mm
- Max handle opening: 125 mm


{% include gallery caption="Iterations and final print of the pliers." %}
