---
title: "Syringe Pump"
excerpt: "DIY syringe pump capable of 1ul / min flow"
header:
  image: /assets/img/syringePump1.jpeg
  teaser: /assets/img/syringePump1.jpeg
gallery:
  - url: /assets/img/syringePump1.jpeg
    image_path: /assets/img/syringePump1.jpeg
    alt: "Real-life syringe pump"
  - url: /assets/img/syringePump2.jpeg
    image_path: /assets/img/syringePump2.jpeg
    alt: "Syringe pump side view"
  - url: /assets/img/syringePump3.jpeg
    image_path: /assets/img/syringePump3.jpeg
    alt: "Syringe pump top-down view"
---

# 3D Printed Syringe Pump

This syringe pump project was a group project where we built a cost-effective solution for precise liquid dispensing using 3D printing and readily available components. The pump is capable of customizable flow rates and is built with modularity in mind for easy adjustments.

## Features

- Adjustable flow rates ranging from 0.5 mL/min to 5 mL/min.
- Arduino-powered system with user-friendly code.
- Portable design with a water-resistant enclosure.
- Physical limit switches to prevent overextension.
- Multi-color LED indicators for status monitoring:
  - Green: Operating
  - Red: Stopped
  - Blue: Reverse mode

## Off-the-Shelf Parts Needed

| Part Name               | Quantity |
|-------------------------|----------|
| Arduino Mega            | 1        |
| NEMA 17 Stepper Motor   | 1        |
| Power Supply (12V)      | 1        |
| LM8UU Linear Bearings   | 2        |
| Linear Rod (8mm x 200mm)| 2        |
| Lead Screw TR8x8        | 1        |
| Limit Switch            | 1        |
| Potentiometer           | 1        |
| RGB LED                 | 1        |
| Push Buttons            | 2        |

## 3D Printed Parts Needed

| Part Name               | Quantity |
|-------------------------|----------|
| Motor Mount             | 1        |
| Carriage                | 1        |
| End Support             | 2        |
| Box Bottom              | 1        |
| Box Lid                 | 1        |

## Interactive Model

<iframe src="https://vanderbilt643.autodesk360.com/shares/public/SH512d4QTec90decfa6e6972764160d20dbe?mode=embed" width="640" height="480" allowfullscreen="true" webkitallowfullscreen="true" mozallowfullscreen="true"  frameborder="0"></iframe>

## Code

The Arduino code used for this syringe pump is available on [HERE](https://github.com/wal627/Syringe-Pump/blob/main/Syringe_pot.ino).

## Gallery

{% include gallery caption="Images of the syringe pump in the flesh" %}
