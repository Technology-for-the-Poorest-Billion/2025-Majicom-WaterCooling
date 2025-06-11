---
title: About Our Project
---
## Introduction

This story starts with **Majicom**, a company that provides purified drinking water kiosks in Tanzania that run on low amounts of power sourced from solar panels. Majicom is a not-for-profit organisation aiming to create a cheaper and more eco-friendly source of drinking water in urban areas.

Chilled water has been shown—through user surveys—to be a desirable feature, and that’s where we come in. Our challenge: **advise Majicom on how to cool the water by 5–10°C from ambient**, while still meeting constraints on power, space, and sanitation.

![Majicom Kiosk](images/kiosk.jpg)

## Active and Passive Cooling

When it comes to water cooling methods, we identified two main approaches:

- **Active cooling** – using some sort of heat pump, (like the refrigerant cycle used in fridges).
- **Passive cooling** – using evaporative cooling, where water absorbs heat as it evaporates into surrounding air.

With a large team size and fairly independent cooling solutions, we split into sub-teams. Our team focused on **active cooling**.

## 1) Tank Sizing and Insulation

![Tank Sizing Calcs](images/sizing-calcs.jpg)

### Objective

Determine whether the main energy constraint is due to:
- Heat lost from the water tank, or
- Energy needed to chill water dispensed during peak times.

### Work Done

- Rough calculations of cooling power needed to serve customers during peak hours.
- Estimating tank heat loss from conduction/convection, assuming added insulation.

### Conclusions

If the tank is insulated, heat loss becomes relatively minor compared to the cooling power required during peak demand. Therefore, **focus should be on water throughput cooling**, not tank losses.

## 2) Whole System Modelling

![System Modelling Graphs](images/system-modelling.png)

### Objective

[Insert objective]

### Work Done

[Insert work done]

### Conclusions

[Insert conclusions]

## 3) CFD (Computational Fluid Dynamics)

### Deliverables

* A validation and backup of numerical heat loss results to surroundings, for a tank held at 24C with outside surroundings at 29C.
* Simulations of convection flow for a variety of peltier or traditional coolant pipe methods.
* Humidity variation analysis of convective heat loss based on Tansanian weather conditions. 

### Work Done

Studies were conducted in Solidworks 2024 with appropriate mesh dependancy studies to ensure accurate and timely results.

#### Static Study

![HeatStatic24](https://github.com/user-attachments/assets/dad25432-4ea5-4c58-9f08-43a667aca4d5)

A static heat flow analysis was conducted in Solidworks 2024 to determine heat loss to surroundings from internal water tank analysis.

#### Convective Study

![24CConvective50%Humidity_1](https://github.com/user-attachments/assets/8fffc51a-cf32-423b-ba84-36898f2cd21d)

A convective heat flow analysis was conducted in Solidworks 2024 Fluid Simulation to determine heat loss to surroundings by investigating external air convection within the Kiosk.

#### Humidity Study

![Heat Loss vs  Humidity](https://github.com/user-attachments/assets/01a4badf-4cbd-4b50-87ec-306a9c4584c9)

Heat loss was measured for the convective study against variations in humidity.


### Conclusions

It was found that the static and convective studies matched each other to within 2%, and further reinforced initial python numerical calculations for heat losses to the environment, giving us a context of the power supply that would be needed for this project. The humidity was not found to affect results outside of edge-case scenarios, which will be passed on to Majicom for consideration in their electrical systems.


## 4) Tap Water Cooling

![Pipe Length Graph](images/pipe-length-graph.png)

### Objective

Investigate the feasibility of using cold **incoming tap water** as an auxiliary cooling source.

### Work Done

- Studied tap vs ambient temperatures in tropical regions.
- Assessed feasibility of heat exchangers transferring heat from tank to colder tap supply.
- Explored passive methods like direct pipe immersion.

### Conclusions

Tap water in Tanzania is generally cooler than the desired tank temp, offering potential for pre-cooling. However, small temperature differences (~5°C) mean **large and costly heat exchangers** would be needed. Simpler solutions (e.g., pipe coiling) were also found **too expensive** for meaningful cooling.

## 5) Testing Peltier Cell Cooling

![Peltier Experimental Setup](images/peltier-test.jpg)

### Objective

Can water be cooled **on-demand** during dispensing using Peltier cells?

### Work Done

- Built a circuit using PC cooling parts to test real-world Peltier performance.
- Transferred heat from water → Peltier → air.

### Conclusions

**Peltier cells were too inefficient** to cool water at required rates. To be viable, they would need **additional heat exchangers and high-power fans**, making them too expensive and complex for this application.

## Final Conclusions

### Our Recommendation to Majicom

From our investigations, several clear conclusions were drawn:

- The **only viable option within the existing energy budget** is to cool **smaller tanks**, a solution used commercially and retrofittable to existing kiosks.
- Despite their complexity, **refrigerant-based cooling systems** are significantly more efficient and more appropriate than Peltier-based options.
- **Cooling a whole tank** is viable, especially in the **wet season**, but would require **larger solar panels** and may interfere with passive methods.

## Next Steps

The clearest path to successful implementation involves:

- Purchasing or building a **simple, compact refrigerant-based cooling module**.
- Investigating partnerships with **commercial water chilling system manufacturers**.
- Continuing research into **passive enhancements**, like insulation and spectrally selective coatings.

