---
title: "Syringe Pump"
excerpt: "Our teams Syringe pump is designed to be as human friendly as possible, outfitted with and LCD screen, multiple selection buttons and a turn-knob."
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

The Syringe Pump designed by our team (Machine Maestros) serves the purpose of delivering precise and accurate amounts of fluid. This homemade syringe pump offers economic benefits while ensuring greater ease of mechanical repairability and programmability. The design involves a stepper motor coupled to a lead screw, converting angular motion to linear motion for controlled fluid delivery. Design requirements include creating parts for syringe interaction, electronic component protection, and additional features like momentary buttons and an LCD for enhanced functionality. The syringe pump's mechanics employ a linear actuator mechanism with stabilizers accommodating various syringe diameters. The enclosure features buttons, switches, and an LED for user interaction, and the design protects against water intrusion. Programmed on an Arduino using C++, the syringe pump incorporates an LCD screen and user friendly controls. Operating limits include a maximum flow rate of approximately 100mL per minute and a minimum volume of 0.1 mL. Overall, the Syringe Pump is a cost-effective, customizable, and versatile solution for precise fluid delivery in diverse applications.

| Component                        | Details                                                |
|----------------------------------|--------------------------------------------------------|
| NEMA 17 Stepper Motor            | Model: NEMA 17                                        |
| Syringes                         | Compatible with 10 mL and 20 mL syringes               |
| Linear Actuator Mechanism        | 2040 Aluminum Extrusion               |
|                                  | 8mm Pitch Lead Screw                                  |
| Electronic Components            | Arduino Uno                                           |
|                                  | 2004 LCD Display                                      |
|                                  | 2 Pushbuttons                                        |
|                                  | Rotary Encoder                                       |
|                                  | Latching Switch                                      |
|                                  | RGB LED                                              |
|                                  | Stepper Motor Drivers (A4988)                |
|                                  | 12V/24V Meanwell PSU                                     |
| Fastening and Hardware           | Various screws for assembly                          |
|                                  | Limit Switch       |

**Operation Instructions:**

1. **Setup:**
   - Use the two momentary buttons to move the plunger presser far back enough for the length of the syringe with its plunger extended.
   - Place the back part of the syringe in the slot on the back barrel stabilizer.
   - Adjust the presser with the momentary buttons as needed.

2. **Initial Positioning:**
   - Advance the plunger presser until it makes contact with the syringe using the forwards and backwards buttons.

3. **Pumping:**
   - Press both buttons simultaneously to slowly advance the plunger.
   - Use the knob and button on the screen to set the syringe size and select the operation mode.
   - Two options for operation mode: If "ml/min" is selected, specify a flow rate, and toggle the switch to start and stop pumping. If "ml" is selected, specify the amount to pump in ml, and press the rotary encoder button to start pumping. The pump will stop automatically once the required volume is pumped.

4. **Safety Features:**
   - If the limit switch is pressed during operation, the pump will warn the user of low fluid and move backward into a safe position, resetting itself.
   - A reset button on the screen allows for program reset if the syringe size needs to be changed.

5. **Syringe Replacement:**
   - Switch out the syringe as desired.

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e916eb197ccabd1d6?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

{% include gallery caption="" %}
<a href="https://github.com/1Mattchu/syringe-pump-code/blob/main/SyringeProject.ino" target="_blank">Syringe Pump Code on GitHub</a>
