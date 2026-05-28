---
title: "Case in Po(r)int"
author: "esemv"
description: "A 3D printer that fits inside and print out of a briefcase"
created_at: "2026-03-24"
---

# 24th March 2026

## Logo Designs
| Thoughts | Design |
|----------|--------|
| This design shows both the words clearly and is also easier to make in Word | <img width="555" height="94" alt="Screenshot 2026-05-28 at 7 21 01 AM" src="https://github.com/user-attachments/assets/4a7b6a33-dbcb-4c93-8c50-eed72500a0e9" /> |
| This design focuses more on ‘Point’ rather than ‘Print’ which focuses on the play on words, but it harder to make in Word. | <img width="555" height="137" alt="Screenshot 2026-05-28 at 7 22 00 AM" src="https://github.com/user-attachments/assets/36490ca8-8fd7-480d-a47d-9cf76e4290b4" /> |

I have decided to go with the first design as it is easier to reproduce and gives equal attention to both the titles, so that the play on words is obvious, while the ‘Print’ is still obvious.


# 28th March 2026
There are two types of extrusion systems: Bowden and Direct Drive. In my printer I am leaning towards Bowden due to space constraints, and the fact that using Bowden means that I can embed the extruder itself into the side of the case without it taking up much excess space.

But here are some benefits and drawbacks for Bowden and Direct Drive extruders to consider:
| Type | Advantages | Disadvantages |
|------|--------|--------------|
| **_Bowden_** | • Weight reduction – lightweight meaning increased precision due to small inertia <br>• Print speeds – moving speed can reach up to 200~300mm/s for faster printing speeds <br>• Maintenance – separate nozzle and extruder give easier maintenance | • Stepper motor torque – resistance in the long Teflon tube requires a higher stepper motor torque <br>• Failure – due to the extruder and nozzle needing to be connected via a pneumatic connector and Teflon tube, as opposed to directly, there is a higher chance of failure <br>• Filament wastage – due to the long tubing it is harder to use up all the filament within it causing wastage |
| **_Direct Drive_** | • Loading and retraction – more precise control of the loading and retraction of filament creating a better surface on 3D printed models <br>• Stepper motor torque – the torque requirement is relatively low <br>• Filament changing – it is easier to change filament <br>• Elastic filaments – it has a better performance for elastic filaments | • Maintenance – all the parts are directly connected making it more difficult to disassemble and maintain parts <br>• Weight – the toolhead is heavier meaning printing speeds are generally lower and Bowden extruders |


# 29th March 2026

I am going to go with a Bowden extruder, mainly due to the size constraints as having the extruder separate will help greatly with that so that I can embed it into the case. The disadvantages above are weighable considering the size constraints, but there are some further variable drawbacks that can be mitigated. Here’s how I’ll handle the main drawbacks of the having a Bowden system:

| Disadvantage | Solution/Reconciliation |
|--------------|-------------------------|
| **Flexible filaments** – due to the Teflon tubing, Bowden systems are not as suitable for flexible filament. | By finetuning settings such as retraction, printing speed, and ensuring the filament is properly dried, printing with flexible filaments can be achieved with a Bowden system. |
| **Tube wearing** – repeated retraction can wear down the Teflon tubing, causing melted filament to ooze out of the system | This can be mitigating using a heat break as a buffer between the Teflon tubing and nozzle |
| **Filament wastage** – due to the long tubing it is harder to use up all the filament within it causing wastage | This can be mitigating by making sure the Teflon tubing is as short as possible to reduce wastage, but cannot be completely avoided. |

<img align="right" width="208" height="213" alt="image" src="https://github.com/user-attachments/assets/600e662d-b589-4f4f-8a33-ebb63c527db1" />

I drew an initial concept sketch of the system, mostly focusing on the Z–Axis and X–Axis with general blocking of where the parts will go.

I may end up using linear rods as they will be more space conservative, but I have currently just drawn them in as aluminium-extrusion-like blocks.

I will later draw in more detailed sketches for each of the axes and minor systems to make them more clear and easier to CAD when I have decided on parts.


<br><br>
# 30th March 2026

I researched some of the parts I would need for the ‘toolhead’, although of course the extruder is separate as it’s a Bowden system. Here are the parts I found detailed below:

