---
title: " uFluidic device"
excerpt: "Creating a microfluidic device that can reliably mix 2 separate fluids into a single homogenous mixture"
header:
  image: /assets/img/IMG_0437.JPEG
  teaser: /assets/img/IMG_0437.JPEG
gallery:
  - url: /assets/img/IMG_0352.JPEG
    image_path: assets/img/IMG_0352.JPEG
    alt: "placeholder image 1"
  - url: /assets/img/image000000.jpg
    image_path: assets/img/image000000.jpg
    alt: "placeholder image 2"
#  - url: /assets/img/Cyber-Scooter-3.jpg
#    image_path: assets/img/Cyber-Scooter-3.jpg
#    alt: "placeholder image 3"
---

Introduction to microfluidic devices: In the realm of microfluidics, where the manipulation of small fluid volumes occurs, achieving homogeneous mixing poses a significant challenge. One prominent application demanding such mixing efficiency is in the field of biochemistry, particularly for rapid and accurate reactions in diagnostic assays. The fundamental obstacle lies in the laminar flow regime inherent to microfluidic systems, where fluids flow in parallel layers without significant mixing between them due to low Reynolds numbers. Consequently, traditional methods like stirring or shaking, effective in macro-scale environments, prove ineffective at the micro-scale. Therefore, developing innovative microfluidic mixers becomes crucial to enable efficient blending of reagents, enhancing reaction kinetics, and improving assay accuracy.

**My Design**
To have proper mixing within a microfluidic device, you must maximize the amount of chaotic turbulence experienced by the two fluids.  By far the most efficient way to achive this is to have the fluid loop back into itself, creating massive points of turbulance at select points of the mixing section.  This causes the 2 seperate fluids to quickly mix, and in practice it works incredibly well.  My design ended up looking almost exactly like a tesla valve, which is designed to prevent the flow of water in one direction by -your guessed it- turbulance.

The channel width and depth was 1 mm.  This was chosen as I wanted to maximize printability.  This came with the downside that I was not able to fit in as many turbulant loops, but I was confident that 10 were more than enough to sufficiently mix the two fluids.



**To transform the 3D printed mold into a functioning microfluidic device, follow these steps:**

1. Print and cure the mold using a resin printer, ensuring proper curing to achieve desired structural integrity.

2. Apply a thin layer of parylene to the surface of the cured mold. This deposition process is crucial for rendering the 3D print biocompatible and suitable for subsequent steps in device fabrication.

3. Cast polydimethylsiloxane (PDMS) onto the parylene-coated mold. Ensure thorough coverage of the mold surface with PDMS to replicate the desired microfluidic features accurately.

4. Bond a glass slide to the PDMS cast on the mold. This step establishes a secure bond between the PDMS layer and the glass slide, forming the final microfluidic device.

Following these instructions enables the fabrication of microfluidic devices from 3D printed molds, without the need for specialized cleanroom facilities or extensive post-print treatments. 


**View Our Design!**
<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e24db52f3abc94ff5?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>


~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~


{% include gallery caption="" %}
<a href="https://github.com/1Mattchu/syringe-pump-code/blob/main/SyringeProject.ino" target="_blank">Syringe Pump Code on GitHub</a>
