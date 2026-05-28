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

| Part | Specific Name & Link | Image | Notes |
|------|----------------------|-------|-------|
| **_Extruder_** | [MK8 Aluminium Bowden Extruder](https://www.aliexpress.com/item/1005007542803374.htmlhttps://www.aliexpress.com/item/1005007542803374.html)<br>($6.09) | <img width="220" height="220" alt="image" src="https://github.com/user-attachments/assets/79e44c5f-3de6-40b0-ae28-5e44867a63e3" /> | • High quality for a low a price <br>• Durable as it’s made from aluminium <br>• Low profile – good for space conservation <br>• Easy to assemble <br>• Compatible with versatile filament types – PLA, ABS, PETG, TPU |
| **_Motor_** | [Nema 17 Stepper Motor: 17HS4401S XH2.54](https://www.aliexpress.com/item/1005011836286637.html)<br>($16.69) | <img width="220" height="220" alt="image" src="https://github.com/user-attachments/assets/089e2a4f-b3e3-41cb-9281-f64d92a340ce" /> | •	Standard motor used for extrusion <br>• High accuracy – also enhanced by the extruder <br>• Good torque (40-59Ncm) for Bowden extrusion systems <br>• Larger with higher mass than NEMA 14, but necessary for Bowden system |
| **_Teflon Tubing_** | [PTFE Transparent Tubing 2mm ID x 4mm OD](https://www.aliexpress.com/item/1005006242932887.html)<br>($2.93) | <img width="220" height="220" alt="image" src="https://github.com/user-attachments/assets/168b58aa-311d-4476-b6c5-e5dd0aba0729" /> | •	2mm Inner Diameter by 4mm Outer Diameter <br>• Compatible with MK8 Bowden Extruder <br>• Transparent for easy troubleshooting |


# 1st April 2026

I am looking at the parts I will need for the different axes, mostly focusing on Z and X currently as I can look at the bed later.

For the Z Axis here are the parts I’m looking at:

| Part | Specific Name & Link | Image | Notes |
|------|----------------------|-------|-------|
| **_Motor_** | [Nema 17 Stepper Motor: 17HS4401S XH2.54](https://www.aliexpress.com/item/1005011836286637.html)<br>($16.69) | <img width="220" height="220" alt="image" src="https://github.com/user-attachments/assets/089e2a4f-b3e3-41cb-9281-f64d92a340ce" /> | •	Standard motor used for extrusion <br>• High accuracy – also enhanced by the extruder <br>• Good torque (40-59Ncm) for Bowden extrusion systems |
| **_Coupler_** | [NEMA 17 Motor - T8 Lead Screw 5x8x25mm Shaft Coupler](https://www.aliexpress.com/item/4000278519274.html)<br>($4.32 x 2) | <img width="220" height="220" alt="image" src="https://github.com/user-attachments/assets/722826cc-0ba4-4c03-8409-7fc490be31f7" /> | • 5mm x 8mm for motor shaft and T8 lead screw <br>• Cheaper option than integrated lead screw |
| **_Lead Screw_** | [T8 Lead Screw with Nut 300mm](https://www.aliexpress.com/item/1005008618305989.html)<br>($1.45 x 2) | <img width="220" height="220" alt="image" src="https://github.com/user-attachments/assets/5404ac41-18b4-410d-9daa-cfc8532a8a95" /> | •	Length TBC once entire system is planned <br>•	T8 is standard size for Z Axis systems <br>• Removes need for linear rails and belt tensioning |
| **_Linear Rods_** | | | • |
| **_Linear Bearings_** | | <img width="220" height="220" alt="image" src="https://github.com/user-attachments/assets/4f2559e5-3238-4fd0-8b22-f829e035cc62" /> | • |

I did some sketches of the Z Axis to visualise ready to 3D model it in Fusion. I have tried to keep the size profile to a minimum so that it all fits well into the case. Here are the sketches:

> [!NOTE]
> Need to insert sketches

<img align="right" width="296" height="250" alt="image" src="https://github.com/user-attachments/assets/8c4cdb3b-2a6f-4782-8a2a-7254bcdf01c5" />

I have found this image very helpful in looking at the different axes motion systems. It mostly uses linear rods too, which is helpful in visualising how that can fit into my system. And it also helps me remember which is X and which is Y :expressionless:.

I also did end up looking at some parts for the Y Axis just to make the dimensions a bit clearer for things like linear rods.
